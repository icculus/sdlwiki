====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_UpdateSensors =

Update the current state of the open sensors.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_UpdateSensors(void);
</syntaxhighlight>

== Remarks ==

This is called automatically by the event loop if sensor events are
enabled.

This needs to be called from the thread that initialized the sensor
subsystem.

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

