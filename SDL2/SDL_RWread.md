====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_RWread =

Read from a data source.

== Syntax ==

<syntaxhighlight lang='c'>
size_t SDL_RWread(SDL_RWops *context,
                  void *ptr, size_t size,
                  size_t maxnum);
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
|the size of each object to read, in bytes
|-
|'''maxnum'''
|the maximum number of objects to be read
|}

== Return Value ==

Returns the number of objects read, or 0 at error or end of file; call
[[SDL_GetError]]() for more information.

== Remarks ==

This function reads up to <code>maxnum</code> objects each of size
<code>size</code> from the data source to the area pointed at by
<code>ptr</code>. This function may read less objects than requested. It
will return zero when there has been an error or the data stream is
completely read.

[[SDL_RWread]]() is actually a function wrapper that calls the
[[SDL_RWops]]'s <code>read</code> method appropriately, to simplify
application development.

Prior to SDL 2.0.10, this function was a macro.

== Version ==

This function is available since SDL 2.0.10.

== Related Functions ==

:[[SDL_RWclose]]
:[[SDL_RWFromConstMem]]
:[[SDL_RWFromFile]]
:[[SDL_RWFromFP]]
:[[SDL_RWFromMem]]
:[[SDL_RWseek]]
:[[SDL_RWwrite]]

----
[[CategoryAPI]]

