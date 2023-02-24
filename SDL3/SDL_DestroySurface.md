====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_DestroySurface =

Free an RGB surface.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_DestroySurface(SDL_Surface *surface);
</syntaxhighlight>

== Function Parameters ==

{|
|'''surface'''
|the [[SDL_Surface]] to free.
|}

== Remarks ==

It is safe to pass NULL to this function.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_CreateSurface]]
:[[SDL_CreateSurfaceFrom]]
:[[SDL_LoadBMP]]
:[[SDL_LoadBMP_RW]]

----
[[CategoryAPI]]

