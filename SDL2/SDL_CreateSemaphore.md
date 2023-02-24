====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_CreateSemaphore =

Create a semaphore.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_sem* SDL_CreateSemaphore(Uint32 initial_value);
</syntaxhighlight>

== Function Parameters ==

{|
|'''initial_value'''
|the starting value of the semaphore
|}

== Return Value ==

Returns a new semaphore or NULL on failure; call [[SDL_GetError]]() for
more information.

== Remarks ==

This function creates a new semaphore and initializes it with the value
<code>initial_value</code>. Each wait operation on the semaphore will
atomically decrement the semaphore value and potentially block if the
semaphore value is 0. Each post operation will atomically increment the
semaphore value and wake waiting threads and allow them to retry the wait
operation.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_DestroySemaphore]]
:[[SDL_SemPost]]
:[[SDL_SemTryWait]]
:[[SDL_SemValue]]
:[[SDL_SemWait]]
:[[SDL_SemWaitTimeout]]

----
[[CategoryAPI]]

