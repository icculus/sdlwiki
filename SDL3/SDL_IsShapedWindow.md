====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_IsShapedWindow =

Return whether the given window is a shaped window.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_IsShapedWindow(const SDL_Window *window);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|The window to query for being shaped.
|}

== Return Value ==

Return [[SDL_TRUE]] if the window is a window that can be shaped,
[[SDL_FALSE]] if the window is unshaped or NULL.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_CreateShapedWindow]]

----
[[CategoryAPI]]

