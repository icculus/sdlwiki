====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_RestoreWindow =

Restore the size and position of a minimized or maximized window.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_RestoreWindow(SDL_Window *window);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window to restore
|}

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_MaximizeWindow]]
:[[SDL_MinimizeWindow]]

----
[[CategoryAPI]], [[CategoryVideo]]

