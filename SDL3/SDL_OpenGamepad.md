====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_OpenGamepad =

Open a gamepad for use.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Gamepad* SDL_OpenGamepad(SDL_JoystickID instance_id);
</syntaxhighlight>

== Function Parameters ==

{|
|'''instance_id'''
|the joystick instance ID
|}

== Return Value ==

Returns a gamepad identifier or NULL if an error occurred; call
[[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_CloseGamepad]]
:[[SDL_GetGamepadNameForIndex]]
:[[SDL_IsGamepad]]

----
[[CategoryAPI]]

