====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetWindowSizeInPixels =

Get the size of a window's client area, in pixels.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_GetWindowSizeInPixels(SDL_Window *window, int *w, int *h);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window from which the drawable size should be queried
|-
|'''w'''
|a pointer to variable for storing the width in pixels, may be NULL
|-
|'''h'''
|a pointer to variable for storing the height in pixels, may be NULL
|}

== Remarks ==

The window size in pixels may differ from the size in screen coordinates if
the window is on a high density display (one with an OS scaling factor).

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_CreateWindow]]
:[[SDL_GetWindowSize]]

----
[[CategoryAPI]]

