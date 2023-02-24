====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_CreateRGBSurfaceWithFormat =

Allocate a new RGB surface with a specific pixel format.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Surface* SDL_CreateRGBSurfaceWithFormat
    (Uint32 flags, int width, int height, int depth, Uint32 format);
</syntaxhighlight>

== Function Parameters ==

{|
|'''flags'''
|the flags are unused and should be set to 0
|-
|'''width'''
|the width of the surface
|-
|'''height'''
|the height of the surface
|-
|'''depth'''
|the depth of the surface in bits
|-
|'''format'''
|the [[SDL_PixelFormatEnum]] for the new surface's pixel format.
|}

== Return Value ==

Returns the new [[SDL_Surface]] structure that is created or NULL if it
fails; call [[SDL_GetError]]() for more information.

== Remarks ==

This function operates mostly like [[SDL_CreateRGBSurface]](), except
instead of providing pixel color masks, you provide it with a predefined
format from [[SDL_PixelFormatEnum]].

== Version ==

This function is available since SDL 2.0.5.

== Related Functions ==

:[[SDL_CreateRGBSurface]]
:[[SDL_CreateRGBSurfaceFrom]]
:[[SDL_FreeSurface]]

----
[[CategoryAPI]]

