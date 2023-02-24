====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetYUVConversionModeForResolution =

Get the YUV conversion mode, returning the correct mode for the resolution when the current conversion mode is [[SDL_YUV_CONVERSION_AUTOMATIC]] 

== Syntax ==

<syntaxhighlight lang='c'>
SDL_YUV_CONVERSION_MODE SDL_GetYUVConversionModeForResolution(int width, int height);
</syntaxhighlight>

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

