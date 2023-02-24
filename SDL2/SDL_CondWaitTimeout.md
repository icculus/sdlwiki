====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_CondWaitTimeout =

Wait until a condition variable is signaled or a certain time has passed.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_CondWaitTimeout(SDL_cond * cond,
                        SDL_mutex * mutex, Uint32 ms);
</syntaxhighlight>

== Function Parameters ==

{|
|'''cond'''
|the condition variable to wait on
|-
|'''mutex'''
|the mutex used to coordinate thread access
|-
|'''ms'''
|the maximum time to wait, in milliseconds, or <code>[[SDL_MUTEX_MAXWAIT]]</code> to wait indefinitely
|}

== Return Value ==

Returns 0 if the condition variable is signaled,
<code>[[SDL_MUTEX_TIMEDOUT]]</code> if the condition is not signaled in the
allotted time, or a negative error code on failure; call [[SDL_GetError]]()
for more information.

== Remarks ==

This function unlocks the specified <code>mutex</code> and waits for
another thread to call [[SDL_CondSignal]]() or [[SDL_CondBroadcast]]() on
the condition variable <code>cond</code>, or for the specified time to
elapse. Once the condition variable is signaled or the time elapsed, the
mutex is re-locked and the function returns.

The mutex must be locked before calling this function.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_CondBroadcast]]
:[[SDL_CondSignal]]
:[[SDL_CondWait]]
:[[SDL_CreateCond]]
:[[SDL_DestroyCond]]

----
[[CategoryAPI]]

