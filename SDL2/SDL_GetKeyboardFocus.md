====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GetKeyboardFocus =

Query the window which currently has keyboard focus.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Window * SDL_GetKeyboardFocus(void);
</syntaxhighlight>

== Return Value ==

Returns the window with keyboard focus.

== Version ==

This function is available since SDL 2.0.0.

----
[[CategoryAPI]]

