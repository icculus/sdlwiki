====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_SensorOpen =

Open a sensor for use.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Sensor* SDL_SensorOpen(int device_index);
</syntaxhighlight>

== Function Parameters ==

{|
|'''device_index'''
|The sensor to open
|}

== Return Value ==

Returns an [[SDL_Sensor]] sensor object, or NULL if an error occurred.

== Version ==

This function is available since SDL 2.0.9.

----
[[CategoryAPI]]

