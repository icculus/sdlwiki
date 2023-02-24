====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GameControllerHasRumbleTriggers =

Query whether a game controller has rumble support on triggers.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_GameControllerHasRumbleTriggers(SDL_GameController *gamecontroller);
</syntaxhighlight>

== Function Parameters ==

{|
|'''gamecontroller'''
|The controller to query
|}

== Return Value ==

Returns [[SDL_TRUE]], or [[SDL_FALSE]] if this controller does not have
trigger rumble support

== Version ==

This function is available since SDL 2.0.18.

== Related Functions ==

:[[SDL_GameControllerRumbleTriggers]]

----
[[CategoryAPI]]

