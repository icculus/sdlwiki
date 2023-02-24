====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_SemPost =

Atomically increment a semaphore's value and wake waiting threads.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_SemPost(SDL_sem * sem);
</syntaxhighlight>

== Function Parameters ==

{|
|'''sem'''
|the semaphore to increment
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_CreateSemaphore]]
:[[SDL_DestroySemaphore]]
:[[SDL_SemTryWait]]
:[[SDL_SemValue]]
:[[SDL_SemWait]]
:[[SDL_SemWaitTimeout]]

----
[[CategoryAPI]]

