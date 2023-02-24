====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_FreeSurface =

Free an RGB surface.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_FreeSurface(SDL_Surface * surface);
</syntaxhighlight>

== Function Parameters ==

{|
|'''surface'''
|the [[SDL_Surface]] to free.
|}

== Remarks ==

It is safe to pass NULL to this function.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_CreateRGBSurface]]
:[[SDL_CreateRGBSurfaceFrom]]
:[[SDL_LoadBMP]]
:[[SDL_LoadBMP_RW]]

----
[[CategoryAPI]]

