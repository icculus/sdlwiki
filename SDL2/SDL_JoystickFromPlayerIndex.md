====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_JoystickFromPlayerIndex =

Get the [[SDL_Joystick]] associated with a player index.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Joystick* SDL_JoystickFromPlayerIndex(int player_index);
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

This function is available since SDL 2.0.12.

----
[[CategoryAPI]]

