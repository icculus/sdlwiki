====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_SetWindowSize =

Set the size of a window's client area, in screen coordinates.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_SetWindowSize(SDL_Window *window, int w, int h);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window to change
|-
|'''w'''
|the width of the window, must be > 0
|-
|'''h'''
|the height of the window, must be > 0
|}

== Remarks ==

The window size in screen coordinates may differ from the size in pixels if
the window is on a high density display (one with an OS scaling factor).

Fullscreen windows automatically match the size of the display mode, and
you should use [[SDL_SetWindowDisplayMode]]() to change their size.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetWindowSize]]
:[[SDL_SetWindowDisplayMode]]

----
[[CategoryAPI]], [[CategoryVideo]]

