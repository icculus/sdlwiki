====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======

== Draft ==

'''THIS PAGE IS A WORK IN PROGRESS''' ... Please make edits to this page to improve it!


<!-- #*^*^*^*^*See https://wiki.libsdl.org/SGFunctions for details on editing this page*^*^*^*^* -->
= SDL_GetGrabbedWindow =

Get the window that currently has an input grab enabled.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Window* SDL_GetGrabbedWindow(void);
</syntaxhighlight>

== Return Value ==

Returns the window if input is grabbed or NULL otherwise.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetWindowGrab]]
:[[SDL_SetWindowGrab]]

----
[[CategoryAPI]], [[CategoryVideo]], [[CategoryDraft]]
<!-- #See the Style Guide for instructions on editing the footer. -->

