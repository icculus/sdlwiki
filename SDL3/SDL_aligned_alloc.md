====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_aligned_alloc =

Allocate memory aligned to a specific value 

== Syntax ==

<syntaxhighlight lang='c'>
SDL_MALLOC void* SDL_aligned_alloc(size_t alignment, size_t size);
</syntaxhighlight>

== Function Parameters ==

{|
|'''alignment'''
|the alignment requested
|-
|'''size'''
|the size to allocate
|}

== Return Value ==

Returns a pointer to the aligned memory

== Remarks ==

If <code>alignment</code> is less than the size of <code>void *</code>,
then it will be increased to match that.

The returned memory address will be a multiple of the alignment value, and
the amount of memory allocated will be a multiple of the alignment value.

The memory returned by this function must be freed with
[[SDL_aligned_free]]()

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_aligned_free]]

----
[[CategoryAPI]]

