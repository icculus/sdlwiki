====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_DestroyCond =

Destroy a condition variable.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_DestroyCond(SDL_cond * cond);
</syntaxhighlight>

== Function Parameters ==

{|
|'''cond'''
|the condition variable to destroy
|}

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_CondBroadcast]]
:[[SDL_CondSignal]]
:[[SDL_CondWait]]
:[[SDL_CondWaitTimeout]]
:[[SDL_CreateCond]]

----
[[CategoryAPI]]

