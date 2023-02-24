====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetSensorInstanceType =

Get the type of a sensor.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_SensorType SDL_GetSensorInstanceType(SDL_SensorID instance_id);
</syntaxhighlight>

== Function Parameters ==

{|
|'''instance_id'''
|the sensor instance ID
|}

== Return Value ==

Returns the [[SDL_SensorType]], or <code>[[SDL_SENSOR_INVALID]]</code> if
<code>instance_id</code> is not valid

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

