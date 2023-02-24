====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GameControllerGetSerial =

Get the serial number of an opened controller, if available.

== Syntax ==

<syntaxhighlight lang='c'>
const char * SDL_GameControllerGetSerial(SDL_GameController *gamecontroller);
</syntaxhighlight>

== Function Parameters ==

{|
|'''gamecontroller'''
|the game controller object to query.
|}

== Return Value ==

Return the serial number, or NULL if unavailable.

== Remarks ==

Returns the serial number of the controller, or NULL if it is not
available.

== Version ==

This function is available since SDL 2.0.14.

----
[[CategoryAPI]]

