====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_SetJoystickPlayerIndex =

Set the player index of an opened joystick.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_SetJoystickPlayerIndex(SDL_Joystick *joystick, int player_index);
</syntaxhighlight>

== Function Parameters ==

{|
|'''joystick'''
|the [[SDL_Joystick]] obtained from [[SDL_OpenJoystick]]()
|-
|'''player_index'''
|Player index to assign to this joystick, or -1 to clear the player index and turn off player LEDs.
|}

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

