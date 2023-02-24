====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetJoystickFromPlayerIndex =

Get the [[SDL_Joystick]] associated with a player index.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Joystick* SDL_GetJoystickFromPlayerIndex(int player_index);
</syntaxhighlight>

== Function Parameters ==

{|
|'''player_index'''
|the player index to get the [[SDL_Joystick]] for
|}

== Return Value ==

Returns an [[SDL_Joystick]] on success or NULL on failure; call
[[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

