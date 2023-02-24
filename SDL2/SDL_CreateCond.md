====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_CreateCond =

Create a condition variable.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_cond* SDL_CreateCond(void);
</syntaxhighlight>

== Return Value ==

Returns a new condition variable or NULL on failure; call
[[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_CondBroadcast]]
:[[SDL_CondSignal]]
:[[SDL_CondWait]]
:[[SDL_CondWaitTimeout]]
:[[SDL_DestroyCond]]

----
[[CategoryAPI]]

