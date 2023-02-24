====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_OpenSensor =

Open a sensor for use.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Sensor* SDL_OpenSensor(SDL_SensorID instance_id);
</syntaxhighlight>

== Function Parameters ==

{|
|'''instance_id'''
|the sensor instance ID
|}

== Return Value ==

Returns an [[SDL_Sensor]] sensor object, or NULL if an error occurred.

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

