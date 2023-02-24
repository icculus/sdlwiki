====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_SensorGetName =

Get the implementation dependent name of a sensor 

== Syntax ==

<syntaxhighlight lang='c'>
const char* SDL_SensorGetName(SDL_Sensor *sensor);
</syntaxhighlight>

== Function Parameters ==

{|
|'''sensor'''
|The [[SDL_Sensor]] object
|}

== Return Value ==

Returns the sensor name, or NULL if <code>sensor</code> is NULL.

== Version ==

This function is available since SDL 2.0.9.

----
[[CategoryAPI]]

