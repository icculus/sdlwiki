====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GameControllerMapping =

Get the current mapping of a Game Controller.

== Syntax ==

<syntaxhighlight lang='c'>
char * SDL_GameControllerMapping(SDL_GameController *gamecontroller);
</syntaxhighlight>

== Function Parameters ==

{|
|'''gamecontroller'''
|the game controller you want to get the current mapping for
|}

== Return Value ==

Returns a string that has the controller's mapping or NULL if no mapping is
available; call [[SDL_GetError]]() for more information.

== Remarks ==

The returned string must be freed with [[SDL_free]]().

Details about mappings are discussed with
[[SDL_GameControllerAddMapping]]().

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GameControllerAddMapping]]
:[[SDL_GameControllerMappingForGUID]]

----
[[CategoryAPI]]

