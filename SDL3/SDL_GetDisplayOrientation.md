====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetDisplayOrientation =

Get the orientation of a display.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_DisplayOrientation SDL_GetDisplayOrientation(SDL_DisplayID displayID);
</syntaxhighlight>

== Function Parameters ==

{|
|'''displayID'''
|the instance ID of the display to query
|}

== Return Value ==

Returns The [[SDL_DisplayOrientation]] enum value of the display, or
<code>[[SDL_ORIENTATION_UNKNOWN]]</code> if it isn't available.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetDisplays]]

----
[[CategoryAPI]]

