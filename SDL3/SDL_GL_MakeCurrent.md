====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GL_MakeCurrent =

Set up an OpenGL context for rendering into an OpenGL window.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_GL_MakeCurrent(SDL_Window *window, SDL_GLContext context);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window to associate with the context
|-
|'''context'''
|the OpenGL context to associate with the window
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Remarks ==

The context must have been created with a compatible window.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GL_CreateContext]]

----
[[CategoryAPI]], [[CategoryVideo]]

