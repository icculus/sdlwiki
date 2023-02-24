====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetJoystickGUIDFromString =

Convert a GUID string into a [[SDL_JoystickGUID]] structure.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_JoystickGUID SDL_GetJoystickGUIDFromString(const char *pchGUID);
</syntaxhighlight>

== Function Parameters ==

{|
|'''pchGUID'''
|string containing an ASCII representation of a GUID
|}

== Return Value ==

Returns a [[SDL_JoystickGUID]] structure.

== Remarks ==

Performs no error checking. If this function is given a string containing
an invalid GUID, the function will silently succeed, but the GUID generated
will not be useful.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetJoystickGUIDString]]

----
[[CategoryAPI]]

