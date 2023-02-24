====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_JoystickGetDevicePlayerIndex =

Get the player index of a joystick, or -1 if it's not available This can be called before any joysticks are opened.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_JoystickGetDevicePlayerIndex(int device_index);
</syntaxhighlight>

== Version ==

This function is available since SDL 2.0.9.

----
[[CategoryAPI]]

