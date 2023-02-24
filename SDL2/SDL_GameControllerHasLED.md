====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GameControllerHasLED =

Query whether a game controller has an LED.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_GameControllerHasLED(SDL_GameController *gamecontroller);
</syntaxhighlight>

== Function Parameters ==

{|
|'''gamecontroller'''
|The controller to query
|}

== Return Value ==

Returns [[SDL_TRUE]], or [[SDL_FALSE]] if this controller does not have a
modifiable LED

== Version ==

This function is available since SDL 2.0.14.

----
[[CategoryAPI]]

