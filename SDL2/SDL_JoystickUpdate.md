====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_JoystickUpdate =

Update the current state of the open joysticks.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_JoystickUpdate(void);
</syntaxhighlight>

== Remarks ==

This is called automatically by the event loop if any joystick events are
enabled.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_JoystickEventState]]

----
[[CategoryAPI]]

