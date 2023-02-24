====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_HapticUnpause =

Unpause a haptic device.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_HapticUnpause(SDL_Haptic * haptic);
</syntaxhighlight>

== Function Parameters ==

{|
|'''haptic'''
|the [[SDL_Haptic]] device to unpause
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Remarks ==

Call to unpause after [[SDL_HapticPause]]().

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_HapticPause]]

----
[[CategoryAPI]]

