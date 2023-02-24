====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
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

This function is available since SDL 2.0.2.

== Related Functions ==

:[[SDL_AtomicCASPtr]]
:[[SDL_AtomicSetPtr]]

----
[[CategoryAPI]]

