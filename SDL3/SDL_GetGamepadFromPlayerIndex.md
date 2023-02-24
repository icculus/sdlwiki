====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetGamepadFromPlayerIndex =

Get the [[SDL_Gamepad]] associated with a player index.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Gamepad* SDL_GetGamepadFromPlayerIndex(int player_index);
</syntaxhighlight>

== Function Parameters ==

{|
|'''player_index'''
|the player index, which different from the instance ID
|}

== Return Value ==

Returns the [[SDL_Gamepad]] associated with a player index.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetGamepadPlayerIndex]]
:[[SDL_SetGamepadPlayerIndex]]

----
[[CategoryAPI]]

