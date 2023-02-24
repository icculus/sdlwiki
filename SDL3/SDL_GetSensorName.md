====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetSensorName =

Get the implementation dependent name of a sensor 

== Syntax ==

<syntaxhighlight lang='c'>
const char* SDL_GetSensorName(SDL_Sensor *sensor);
</syntaxhighlight>

== Function Parameters ==

{|
|'''sensor'''
|The [[SDL_Sensor]] object
|}

== Return Value ==

Returns the sensor name, or NULL if <code>sensor</code> is NULL.

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

