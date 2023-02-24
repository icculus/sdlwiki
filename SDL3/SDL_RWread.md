====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_RWread =

Read from a data source.

== Syntax ==

<syntaxhighlight lang='c'>
Sint64 SDL_RWread(SDL_RWops *context, void *ptr, Sint64 size);
</syntaxhighlight>

== Function Parameters ==

{|
|'''context'''
|a pointer to an [[SDL_RWops]] structure
|-
|'''ptr'''
|a pointer to a buffer to read data into
|-
|'''size'''
|the number of bytes to read from the data source.
|}

== Return Value ==

Returns the number of bytes read, 0 at end of file, -1 on error, and -2 for
data not ready with a non-blocking context.

== Remarks ==

This function reads up <code>size</code> bytes from the data source to the
area pointed at by <code>ptr</code>. This function may read less bytes than
requested. It will return zero when the data stream is completely read, or
-1 on error. For streams that support non-blocking operation, if nothing
was read because it would require blocking, this function returns -2 to
distinguish that this is not an error or end-of-file, and the caller can
try again later.

[[SDL_RWread]]() is actually a function wrapper that calls the
[[SDL_RWops]]'s <code>read</code> method appropriately, to simplify
application development.

It is an error to specify a negative <code>size</code>, but this parameter
is signed so you definitely cannot overflow the return value on a
successful run with enormous amounts of data.

== Version ==

This function is available since SDL 3.0.0.

== Code Examples ==

<syntaxhighlight lang='c++'>
SDL_RWops *rw = SDL_RWFromFile("test.bin","r");
if (rw != NULL) {
    extern Uint8 buf[256];
    SDL_RWread(rw, buf, sizeof (buf), 1);
    SDL_RWclose(rw);
}
</syntaxhighlight>

Read a complete file in memory (assuming size can be detected) (from [https://gitlab.com/wikibooks-opengl/modern-tutorials/blob/master/common-sdl2/shader_utils.cpp OpenGL WikiBook]):
<syntaxhighlight lang='c++'>
char* file_read(const char* filename) {
	SDL_RWops *rw = SDL_RWFromFile(filename, "rb");
	if (rw == NULL) return NULL;

	Sint64 res_size = SDL_RWsize(rw);
	char* res = (char*)malloc(res_size + 1);

	Sint64 nb_read_total = 0, nb_read = 1;
	char* buf = res;
	while (nb_read_total < res_size && nb_read != 0) {
		nb_read = SDL_RWread(rw, buf, 1, (res_size - nb_read_total));
		nb_read_total += nb_read;
		buf += nb_read;
	}
	SDL_RWclose(rw);
	if (nb_read_total != res_size) {
		free(res);
		return NULL;
	}

	res[nb_read_total] = '\0';
	return res;
}
</syntaxhighlight>

== Related Functions ==

:[[SDL_RWclose]]
:[[SDL_RWFromConstMem]]
:[[SDL_RWFromFile]]
:[[SDL_RWFromMem]]
:[[SDL_RWseek]]
:[[SDL_RWwrite]]

----
[[CategoryAPI]], [[CategoryIO]]

