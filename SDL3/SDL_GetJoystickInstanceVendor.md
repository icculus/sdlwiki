====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetJoystickInstanceVendor =

Get the USB vendor ID of a joystick, if available.

== Syntax ==

<syntaxhighlight lang='c'>
Uint16 SDL_GetJoystickInstanceVendor(SDL_JoystickID instance_id);
</syntaxhighlight>

== Function Parameters ==

{|
|'''instance_id'''
|the joystick instance ID
|}

== Return Value ==

Returns the USB vendor ID of the selected joystick. If called on an invalid
index, this function returns zero

== Remarks ==

This can be called before any joysticks are opened. If the vendor ID isn't
available this function returns 0.

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

