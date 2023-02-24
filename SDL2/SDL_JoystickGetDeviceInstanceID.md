====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_JoystickGetDeviceInstanceID =

Get the instance ID of a joystick.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_JoystickID SDL_JoystickGetDeviceInstanceID(int device_index);
</syntaxhighlight>

== Function Parameters ==

{|
|'''device_index'''
|the index of the joystick to query (the N'th joystick on the system
|}

== Return Value ==

Returns the instance id of the selected joystick. If called on an invalid
index, this function returns -1.

== Remarks ==

This can be called before any joysticks are opened.

== Version ==

This function is available since SDL 2.0.6.

----
[[CategoryAPI]]

