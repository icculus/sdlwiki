====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetSensorFromInstanceID =

Return the [[SDL_Sensor]] associated with an instance ID.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Sensor* SDL_GetSensorFromInstanceID(SDL_SensorID instance_id);
</syntaxhighlight>

== Function Parameters ==

{|
|'''instance_id'''
|the sensor instance ID
|}

== Return Value ==

Returns an [[SDL_Sensor]] object.

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

