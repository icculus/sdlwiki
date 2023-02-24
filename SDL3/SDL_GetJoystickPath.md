====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetJoystickPath =

Get the implementation dependent path of a joystick.

== Syntax ==

<syntaxhighlight lang='c'>
const char* SDL_GetJoystickPath(SDL_Joystick *joystick);
</syntaxhighlight>

== Function Parameters ==

{|
|'''joystick'''
|the [[SDL_Joystick]] obtained from [[SDL_OpenJoystick]]()
|}

== Return Value ==

Returns the path of the selected joystick. If no path can be found, this
function returns NULL; call [[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetJoystickInstancePath]]

----
[[CategoryAPI]]

