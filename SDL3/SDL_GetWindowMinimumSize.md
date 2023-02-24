====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetWindowMinimumSize =

Get the minimum size of a window's client area, in screen coordinates.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_GetWindowMinimumSize(SDL_Window *window, int *w, int *h);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window to query
|-
|'''w'''
|a pointer filled in with the minimum width of the window, may be NULL
|-
|'''h'''
|a pointer filled in with the minimum height of the window, may be NULL
|}

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetWindowMaximumSize]]
:[[SDL_SetWindowMinimumSize]]

----
[[CategoryAPI]], [[CategoryVideo]]
<!-- #See the Style Guide for instructions on editing the footer. -->

