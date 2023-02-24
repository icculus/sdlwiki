====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_CloseJoystick =

Close a joystick previously opened with [[SDL_OpenJoystick]]().

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_CloseJoystick(SDL_Joystick *joystick);
</syntaxhighlight>

== Function Parameters ==

{|
|'''joystick'''
|The joystick device to close
|}

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_OpenJoystick]]

----
[[CategoryAPI]]

