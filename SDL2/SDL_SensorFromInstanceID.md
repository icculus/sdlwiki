====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_SensorFromInstanceID =

Return the [[SDL_Sensor]] associated with an instance id.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Sensor* SDL_SensorFromInstanceID(SDL_SensorID instance_id);
</syntaxhighlight>

== Function Parameters ==

{|
|'''instance_id'''
|The sensor from instance id
|}

== Return Value ==

Returns an [[SDL_Sensor]] object.

== Version ==

This function is available since SDL 2.0.9.

----
[[CategoryAPI]]

