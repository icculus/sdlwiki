====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_SemTryWait =

See if a semaphore has a positive value and decrement it if it does.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_SemTryWait(SDL_sem * sem);
</syntaxhighlight>

== Function Parameters ==

{|
|'''sem'''
|the semaphore to wait on
|}

== Return Value ==

Returns 0 if the wait succeeds, <code>[[SDL_MUTEX_TIMEDOUT]]</code> if the
wait would block, or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Remarks ==

This function checks to see if the semaphore pointed to by <code>sem</code>
has a positive value and atomically decrements the semaphore value if it
does. If the semaphore doesn't have a positive value, the function
immediately returns [[SDL_MUTEX_TIMEDOUT]].

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_CreateSemaphore]]
:[[SDL_DestroySemaphore]]
:[[SDL_SemPost]]
:[[SDL_SemValue]]
:[[SDL_SemWait]]
:[[SDL_SemWaitTimeout]]

----
[[CategoryAPI]]

