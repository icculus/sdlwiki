====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_SensorGetType =

Get the type of a sensor.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_SensorType SDL_SensorGetType(SDL_Sensor *sensor);
</syntaxhighlight>

== Function Parameters ==

{|
|'''sensor'''
|The [[SDL_Sensor]] object to inspect
|}

== Return Value ==

Returns the [[SDL_SensorType]] type, or <code>[[SDL_SENSOR_INVALID]]</code>
if <code>sensor</code> is NULL.

== Version ==

This function is available since SDL 2.0.9.

----
[[CategoryAPI]]

