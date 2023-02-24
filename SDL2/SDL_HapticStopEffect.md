====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_HapticStopEffect =

Stop the haptic effect on its associated haptic device.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_HapticStopEffect(SDL_Haptic * haptic,
                         int effect);
</syntaxhighlight>

== Function Parameters ==

{|
|'''haptic'''
|the [[SDL_Haptic]] device to stop the effect on
|-
|'''effect'''
|the ID of the haptic effect to stop
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Remarks ==

*

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_HapticDestroyEffect]]
:[[SDL_HapticRunEffect]]

----
[[CategoryAPI]]

