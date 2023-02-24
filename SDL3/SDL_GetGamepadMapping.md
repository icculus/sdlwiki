====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetGamepadMapping =

Get the current mapping of a gamepad.

== Syntax ==

<syntaxhighlight lang='c'>
char * SDL_GetGamepadMapping(SDL_Gamepad *gamepad);
</syntaxhighlight>

== Function Parameters ==

{|
|'''gamepad'''
|the gamepad you want to get the current mapping for
|}

== Return Value ==

Returns a string that has the gamepad's mapping or NULL if no mapping is
available; call [[SDL_GetError]]() for more information.

== Remarks ==

The returned string must be freed with [[SDL_free]]().

Details about mappings are discussed with [[SDL_AddGamepadMapping]]().

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_AddGamepadMapping]]
:[[SDL_GetGamepadMappingForGUID]]

----
[[CategoryAPI]]

