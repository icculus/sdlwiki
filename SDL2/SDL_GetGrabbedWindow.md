====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GetGrabbedWindow =

Get the window that currently has an input grab enabled.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Window * SDL_GetGrabbedWindow(void);
</syntaxhighlight>

== Return Value ==

Returns the window if input is grabbed or NULL otherwise.

== Version ==

This function is available since SDL 2.0.4.

== Related Functions ==

:[[SDL_GetWindowGrab]]
:[[SDL_SetWindowGrab]]

----
[[CategoryAPI]]

