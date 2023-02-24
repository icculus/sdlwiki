====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_SendJoystickEffect =

Send a joystick specific effect packet 

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_SendJoystickEffect(SDL_Joystick *joystick, const void *data, int size);
</syntaxhighlight>

== Function Parameters ==

{|
|'''joystick'''
|The joystick to affect
|-
|'''data'''
|The data to send to the joystick
|-
|'''size'''
|The size of the data to send to the joystick
|}

== Return Value ==

Returns 0, or -1 if this joystick or driver doesn't support effect packets

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

