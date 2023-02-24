====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_SensorGetDeviceInstanceID =

Get the instance ID of a sensor.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_SensorID SDL_SensorGetDeviceInstanceID(int device_index);
</syntaxhighlight>

== Function Parameters ==

{|
|'''device_index'''
|The sensor to get instance id from
|}

== Return Value ==

Returns the sensor instance ID, or -1 if <code>device_index</code> is out
of range.

== Version ==

This function is available since SDL 2.0.9.

----
[[CategoryAPI]]

