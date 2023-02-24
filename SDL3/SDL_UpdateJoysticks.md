====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_UpdateJoysticks =

Update the current state of the open joysticks.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_UpdateJoysticks(void);
</syntaxhighlight>

== Remarks ==

This is called automatically by the event loop if any joystick events are
enabled.

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

