====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetGamepadMappingForGUID =

Get the gamepad mapping string for a given GUID.

== Syntax ==

<syntaxhighlight lang='c'>
char * SDL_GetGamepadMappingForGUID(SDL_JoystickGUID guid);
</syntaxhighlight>

== Function Parameters ==

{|
|'''guid'''
|a structure containing the GUID for which a mapping is desired
|}

== Return Value ==

Returns a mapping string or NULL on error; call [[SDL_GetError]]() for more
information.

== Remarks ==

The returned string must be freed with [[SDL_free]]().

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetJoystickInstanceGUID]]
:[[SDL_GetJoystickGUID]]

----
[[CategoryAPI]]

