====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GameControllerClose =

Close a game controller previously opened with [[SDL_GameControllerOpen]]().

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_GameControllerClose(SDL_GameController *gamecontroller);
</syntaxhighlight>

== Function Parameters ==

{|
|'''gamecontroller'''
|a game controller identifier previously returned by [[SDL_GameControllerOpen]]()
|}

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GameControllerOpen]]

----
[[CategoryAPI]]

