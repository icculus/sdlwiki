====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_SetWindowMinimumSize =

Set the minimum size of a window's client area.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_SetWindowMinimumSize(SDL_Window * window,
                              int min_w, int min_h);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window to change
|-
|'''min_w'''
|the minimum width of the window in pixels
|-
|'''min_h'''
|the minimum height of the window in pixels
|}

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GetWindowMinimumSize]]
:[[SDL_SetWindowMaximumSize]]

----
[[CategoryAPI]]

