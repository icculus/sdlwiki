====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_HapticRumbleInit =

Initialize a haptic device for simple rumble playback.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_HapticRumbleInit(SDL_Haptic * haptic);
</syntaxhighlight>

== Function Parameters ==

{|
|'''haptic'''
|the haptic device to initialize for simple rumble playback
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_HapticOpen]]
:[[SDL_HapticRumblePlay]]
:[[SDL_HapticRumbleStop]]
:[[SDL_HapticRumbleSupported]]

----
[[CategoryAPI]]

