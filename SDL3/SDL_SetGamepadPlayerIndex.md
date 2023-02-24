====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_SetGamepadPlayerIndex =

Set the player index of an opened gamepad.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_SetGamepadPlayerIndex(SDL_Gamepad *gamepad, int player_index);
</syntaxhighlight>

== Function Parameters ==

{|
|'''gamepad'''
|the gamepad object to adjust.
|-
|'''player_index'''
|Player index to assign to this gamepad, or -1 to clear the player index and turn off player LEDs.
|}

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

