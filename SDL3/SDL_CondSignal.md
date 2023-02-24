====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_CondSignal =

Restart one of the threads that are waiting on the condition variable.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_CondSignal(SDL_cond *cond);
</syntaxhighlight>

== Function Parameters ==

{|
|'''cond'''
|the condition variable to signal
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_CondBroadcast]]
:[[SDL_CondWait]]
:[[SDL_CondWaitTimeout]]
:[[SDL_CreateCond]]
:[[SDL_DestroyCond]]

----
[[CategoryAPI]], [[CategoryMutex]]

