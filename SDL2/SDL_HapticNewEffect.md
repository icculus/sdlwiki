====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_HapticNewEffect =

Create a new haptic effect on a specified device.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_HapticNewEffect(SDL_Haptic * haptic,
                        SDL_HapticEffect * effect);
</syntaxhighlight>

== Function Parameters ==

{|
|'''haptic'''
|an [[SDL_Haptic]] device to create the effect on
|-
|'''effect'''
|an [[SDL_HapticEffect]] structure containing the properties of the effect to create
|}

== Return Value ==

Returns the ID of the effect on success or a negative error code on
failure; call [[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_HapticDestroyEffect]]
:[[SDL_HapticRunEffect]]
:[[SDL_HapticUpdateEffect]]

----
[[CategoryAPI]]

