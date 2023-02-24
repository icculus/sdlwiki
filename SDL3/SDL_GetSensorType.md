====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetSensorType =

Get the type of a sensor.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_SensorType SDL_GetSensorType(SDL_Sensor *sensor);
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

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

