====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GL_UnbindTexture =

Unbind an OpenGL/ES/ES2 texture from the current context.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_GL_UnbindTexture(SDL_Texture *texture);
</syntaxhighlight>

== Function Parameters ==

{|
|'''texture'''
|the texture to unbind from the current OpenGL/ES/ES2 context
|}

== Return Value ==

Returns 0 on success, or -1 if the operation is not supported

== Remarks ==

See [[SDL_GL_BindTexture]]() for examples on how to use these functions

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GL_BindTexture]]
:[[SDL_GL_MakeCurrent]]

----
[[CategoryAPI]], [[CategoryRender]]

