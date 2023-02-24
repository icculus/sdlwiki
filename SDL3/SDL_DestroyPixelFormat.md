====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_DestroyPixelFormat =

Free an [[SDL_PixelFormat]] structure allocated by [[SDL_CreatePixelFormat]]().

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_DestroyPixelFormat(SDL_PixelFormat *format);
</syntaxhighlight>

== Function Parameters ==

{|
|'''format'''
|the [[SDL_PixelFormat]] structure to free
|}

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_CreatePixelFormat]]

----
[[CategoryAPI]]

