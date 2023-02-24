====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_CloseSensor =

Close a sensor previously opened with [[SDL_OpenSensor]]().

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_CloseSensor(SDL_Sensor *sensor);
</syntaxhighlight>

== Function Parameters ==

{|
|'''sensor'''
|The [[SDL_Sensor]] object to close
|}

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

