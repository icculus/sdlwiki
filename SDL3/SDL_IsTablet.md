====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_IsTablet =

Query if the current device is a tablet.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_IsTablet(void);
</syntaxhighlight>

== Return Value ==

Returns [[SDL_TRUE]] if the device is a tablet, [[SDL_FALSE]] otherwise.

== Remarks ==

If SDL can't determine this, it will return [[SDL_FALSE]].

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

