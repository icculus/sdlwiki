====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetNumJoystickHats =

Get the number of POV hats on a joystick.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_GetNumJoystickHats(SDL_Joystick *joystick);
</syntaxhighlight>

== Function Parameters ==

{|
|'''joystick'''
|an [[SDL_Joystick]] structure containing joystick information
|}

== Return Value ==

Returns the number of POV hats on success or a negative error code on
failure; call [[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetJoystickHat]]
:[[SDL_OpenJoystick]]

----
[[CategoryAPI]]

