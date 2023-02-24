====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_AllocFormat =

Create an [[SDL_PixelFormat]] structure corresponding to a pixel format.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_PixelFormat * SDL_AllocFormat(Uint32 pixel_format);
</syntaxhighlight>

== Function Parameters ==

{|
|'''pixel_format'''
|one of the [[SDL_PixelFormatEnum]] values
|}

== Return Value ==

Returns the new [[SDL_PixelFormat]] structure or NULL on failure; call
[[SDL_GetError]]() for more information.

== Remarks ==

Returned structure may come from a shared global cache (i.e. not newly
allocated), and hence should not be modified, especially the palette. Weird
errors such as <code>Blit combination not supported</code> may occur.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_FreeFormat]]

----
[[CategoryAPI]]

