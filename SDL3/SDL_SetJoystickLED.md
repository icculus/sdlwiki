====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_SetJoystickLED =

Update a joystick's LED color.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_SetJoystickLED(SDL_Joystick *joystick, Uint8 red, Uint8 green, Uint8 blue);
</syntaxhighlight>

== Function Parameters ==

{|
|'''joystick'''
|The joystick to update
|-
|'''red'''
|The intensity of the red LED
|-
|'''green'''
|The intensity of the green LED
|-
|'''blue'''
|The intensity of the blue LED
|}

== Return Value ==

Returns 0 on success, -1 if this joystick does not have a modifiable LED

== Remarks ==

An example of a joystick LED is the light on the back of a PlayStation 4's
DualShock 4 controller.

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

