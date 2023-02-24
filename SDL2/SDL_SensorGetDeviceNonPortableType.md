====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_SensorGetDeviceNonPortableType =

Get the platform dependent type of a sensor.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_SensorGetDeviceNonPortableType(int device_index);
</syntaxhighlight>

== Function Parameters ==

{|
|'''device_index'''
|The sensor to check
|}

== Return Value ==

Returns the sensor platform dependent type, or -1 if
<code>device_index</code> is out of range.

== Version ==

This function is available since SDL 2.0.9.

----
[[CategoryAPI]]

