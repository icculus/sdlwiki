====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetMasksForPixelFormatEnum =

Convert one of the enumerated pixel formats to a bpp value and RGBA masks.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_GetMasksForPixelFormatEnum(Uint32 format,
                                    int *bpp,
                                    Uint32 * Rmask,
                                    Uint32 * Gmask,
                                    Uint32 * Bmask,
                                    Uint32 * Amask);
</syntaxhighlight>

== Function Parameters ==

{|
|'''format'''
|one of the [[SDL_PixelFormatEnum]] values
|-
|'''bpp'''
|a bits per pixel value; usually 15, 16, or 32
|-
|'''Rmask'''
|a pointer filled in with the red mask for the format
|-
|'''Gmask'''
|a pointer filled in with the green mask for the format
|-
|'''Bmask'''
|a pointer filled in with the blue mask for the format
|-
|'''Amask'''
|a pointer filled in with the alpha mask for the format
|}

== Return Value ==

Returns [[SDL_TRUE]] on success or [[SDL_FALSE]] if the conversion wasn't
possible; call [[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetPixelFormatEnumForMasks]]

----
[[CategoryAPI]]

