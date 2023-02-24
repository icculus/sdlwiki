====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_SetWindowPosition =

Set the position of a window.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_SetWindowPosition(SDL_Window * window,
                           int x, int y);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window to reposition
|-
|'''x'''
|the x coordinate of the window in screen coordinates, or <code>[[SDL_WINDOWPOS_CENTERED]]</code> or <code>[[SDL_WINDOWPOS_UNDEFINED]]</code>
|-
|'''y'''
|the y coordinate of the window in screen coordinates, or <code>[[SDL_WINDOWPOS_CENTERED]]</code> or <code>[[SDL_WINDOWPOS_UNDEFINED]]</code>
|}

== Remarks ==

The window coordinate origin is the upper left of the display.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GetWindowPosition]]

----
[[CategoryAPI]]

