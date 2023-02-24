====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetWindowPosition =

Get the position of a window, in screen coordinates.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_GetWindowPosition(SDL_Window *window, int *x, int *y);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window to query
|-
|'''x'''
|a pointer filled in with the x position of the window, may be NULL
|-
|'''y'''
|a pointer filled in with the y position of the window, may be NULL
|}

== Remarks ==

If you do not need the value for one of the positions a NULL may be passed
in the <code>x</code> or <code>y</code> parameter.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_SetWindowPosition]]

----
[[CategoryAPI]], [[CategoryVideo]]

