====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_UpdateWindowSurface =

Copy the window surface to the screen.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_UpdateWindowSurface(SDL_Window *window);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window to update
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Remarks ==

This is the function you use to reflect any changes to the surface on the
screen.

This function is equivalent to the SDL 1.2 API [[SDL_Flip]]().

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetWindowSurface]]
:[[SDL_UpdateWindowSurfaceRects]]

----
[[CategoryAPI]], [[CategoryVideo]]

