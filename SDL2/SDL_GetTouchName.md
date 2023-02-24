====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GetTouchName =

Get the touch device name as reported from the driver or NULL if the index is invalid.

== Syntax ==

<syntaxhighlight lang='c'>
const char* SDL_GetTouchName(int index);
</syntaxhighlight>

== Version ==

This function is available since SDL 2.0.22.

----
[[CategoryAPI]]

