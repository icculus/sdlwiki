====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_SemValue =

Get the current value of a semaphore.

== Syntax ==

<syntaxhighlight lang='c'>
Uint32 SDL_SemValue(SDL_sem * sem);
</syntaxhighlight>

== Function Parameters ==

{|
|'''sem'''
|the semaphore to query
|}

== Return Value ==

Returns the current value of the semaphore.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_CreateSemaphore]]

----
[[CategoryAPI]]

