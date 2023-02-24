====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_AtomicGetPtr =

Get the value of a pointer atomically.

== Syntax ==

<syntaxhighlight lang='c'>
void* SDL_AtomicGetPtr(void **a);
</syntaxhighlight>

== Function Parameters ==

{|
|'''a'''
|a pointer to a pointer
|}

== Return Value ==

Returns the current value of a pointer.

== Remarks ==

'''''Note: If you don't know what this function is for, you shouldn't use
it!'''''

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_AtomicCASPtr]]
:[[SDL_AtomicSetPtr]]

----
[[CategoryAPI]], [[CategoryAtomic]]

