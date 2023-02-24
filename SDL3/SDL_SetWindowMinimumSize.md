====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_SetWindowMinimumSize =

Set the minimum size of a window's client area, in screen coordinates.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_SetWindowMinimumSize(SDL_Window *window, int min_w, int min_h);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window to change
|-
|'''min_w'''
|the minimum width of the window
|-
|'''min_h'''
|the minimum height of the window
|}

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetWindowMinimumSize]]
:[[SDL_SetWindowMaximumSize]]

----
[[CategoryAPI]], [[CategoryVideo]]
<!-- #See the Style Guide for instructions on editing the footer. -->

