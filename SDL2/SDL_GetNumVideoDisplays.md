====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GetNumVideoDisplays =

Get the number of available video displays.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_GetNumVideoDisplays(void);
</syntaxhighlight>

== Return Value ==

Returns a number >= 1 or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GetDisplayBounds]]

----
[[CategoryAPI]]

