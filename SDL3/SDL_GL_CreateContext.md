====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GL_CreateContext =

Create an OpenGL context for an OpenGL window, and make it current.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_GLContext SDL_GL_CreateContext(SDL_Window *window);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window to associate with the context
|}

== Return Value ==

Returns the OpenGL context associated with <code>window</code> or NULL on
error; call [[SDL_GetError]]() for more details.

== Remarks ==

Windows users new to OpenGL should note that, for historical reasons, GL
functions added after OpenGL version 1.1 are not available by default.
Those functions must be loaded at run-time, either with an OpenGL
extension-handling library or with [[SDL_GL_GetProcAddress]]() and its
related functions.

[[SDL_GLContext]] is an alias for <code>void *</code>. It's opaque to the
application.

== Version ==

This function is available since SDL 3.0.0.

== Code Examples ==

<syntaxhighlight lang='c++'>

// Window mode MUST include SDL_WINDOW_OPENGL for use with OpenGL.
SDL_Window *window = SDL_CreateWindow(
    "SDL2/OpenGL Demo", 0, 0, 640, 480, 
    SDL_WINDOW_OPENGL|SDL_WINDOW_RESIZABLE);
  
// Create an OpenGL context associated with the window.
SDL_GLContext glcontext = SDL_GL_CreateContext(window);

// now you can make GL calls.
glClearColor(0,0,0,1);
glClear(GL_COLOR_BUFFER_BIT);
SDL_GL_SwapWindow(window);

// Once finished with OpenGL functions, the SDL_GLContext can be deleted.
SDL_GL_DeleteContext(glcontext);  
</syntaxhighlight>

== Related Functions ==

:[[SDL_GL_DeleteContext]]
:[[SDL_GL_MakeCurrent]]

----
[[CategoryAPI]], [[CategoryVideo]]

