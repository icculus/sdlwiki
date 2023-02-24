====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GameControllerName =

Get the implementation-dependent name for an opened game controller.

== Syntax ==

<syntaxhighlight lang='c'>
const char* SDL_GameControllerName(SDL_GameController *gamecontroller);
</syntaxhighlight>

== Function Parameters ==

{|
|'''gamecontroller'''
|a game controller identifier previously returned by [[SDL_GameControllerOpen]]()
|}

== Return Value ==

Returns the implementation dependent name for the game controller, or NULL
if there is no name or the identifier passed is invalid.

== Remarks ==

This is the same name as returned by [[SDL_GameControllerNameForIndex]](),
but it takes a controller identifier instead of the (unstable) device
index.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GameControllerNameForIndex]]
:[[SDL_GameControllerOpen]]

----
[[CategoryAPI]]

