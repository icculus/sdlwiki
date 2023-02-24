====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_RWwrite =

Write to an [[SDL_RWops]] data stream.

== Syntax ==

<syntaxhighlight lang='c'>
Sint64 SDL_RWwrite(SDL_RWops *context,
                   const void *ptr, Sint64 size);
</syntaxhighlight>

== Function Parameters ==

{|
|'''context'''
|a pointer to an [[SDL_RWops]] structure
|-
|'''ptr'''
|a pointer to a buffer containing data to write
|-
|'''size'''
|the number of bytes to write
|}

== Return Value ==

Returns the number of bytes written, which will be less than
<code>num</code> on error; call [[SDL_GetError]]() for more information.

== Remarks ==

This function writes exactly <code>size</code> bytes from the area pointed
at by <code>ptr</code> to the stream. If this fails for any reason, it'll
return less than <code>size</code> to demonstrate how far the write
progressed. On success, it returns <code>num</code>.

On error, this function still attempts to write as much as possible, so it
might return a positive value less than the requested write size. If the
function failed to write anything and there was an actual error, it will
return -1. For streams that support non-blocking operation, if nothing was
written because it would require blocking, this function returns -2 to
distinguish that this is not an error and the caller can try again later.

[[SDL_RWwrite]] is actually a function wrapper that calls the
[[SDL_RWops]]'s <code>write</code> method appropriately, to simplify
application development.

It is an error to specify a negative <code>size</code>, but this parameter
is signed so you definitely cannot overflow the return value on a
successful run with enormous amounts of data.

== Version ==

This function is available since SDL 3.0.0.

== Code Examples ==

<syntaxhighlight lang='c++'>
SDL_RWops *rw = SDL_RWFromFile("hello.txt", "w");
if(rw != NULL) {
    const char *str = "Hello World";
    size_t len = SDL_strlen(str);
    if (SDL_RWwrite(rw, str, 1, len) != len) {
        printf("Couldn't fully write string\n");
    } else {
        printf("Wrote %d 1-byte blocks\n", len);
    }
    SDL_RWclose(rw);
}
</syntaxhighlight>

== Related Functions ==

:[[SDL_RWclose]]
:[[SDL_RWFromConstMem]]
:[[SDL_RWFromFile]]
:[[SDL_RWFromMem]]
:[[SDL_RWread]]
:[[SDL_RWseek]]

----
[[CategoryAPI]], [[CategoryIO]]

