====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_SensorGetDeviceName =

Get the implementation dependent name of a sensor.

== Syntax ==

<syntaxhighlight lang='c'>
const char* SDL_SensorGetDeviceName(int device_index);
</syntaxhighlight>

== Function Parameters ==

{|
|'''device_index'''
|The sensor to obtain name from
|}

== Return Value ==

Returns the sensor name, or NULL if <code>device_index</code> is out of
range.

== Version ==

This function is available since SDL 2.0.9.

----
[[CategoryAPI]]

