====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_HapticOpenFromMouse =

Try to open a haptic device from the current mouse.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Haptic* SDL_HapticOpenFromMouse(void);
</syntaxhighlight>

== Return Value ==

Returns the haptic device identifier or NULL on failure; call
[[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_HapticOpen]]
:[[SDL_MouseIsHaptic]]

----
[[CategoryAPI]]

