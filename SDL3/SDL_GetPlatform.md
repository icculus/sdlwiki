====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetPlatform =

Get the name of the platform.

== Syntax ==

<syntaxhighlight lang='c'>
const char * SDL_GetPlatform (void);
</syntaxhighlight>

== Return Value ==

Returns the name of the platform. If the correct platform name is not
available, returns a string beginning with the text "Unknown".

== Remarks ==

Here are the names returned for some (but not all) supported platforms:

* "Windows"
* "macOS"
* "Linux"
* "iOS"
* "Android"

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]], [[CategoryPlatform]]

