====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetGamepadStringForAxis =

Convert from an [[SDL_GamepadAxis]] enum to a string.

== Syntax ==

<syntaxhighlight lang='c'>
const char* SDL_GetGamepadStringForAxis(SDL_GamepadAxis axis);
</syntaxhighlight>

== Function Parameters ==

{|
|'''axis'''
|an enum value for a given [[SDL_GamepadAxis]]
|}

== Return Value ==

Returns a string for the given axis, or NULL if an invalid axis is
specified. The string returned is of the format used by [[SDL_Gamepad]]
mapping strings.

== Remarks ==

The caller should not [[SDL_free]]() the returned string.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetGamepadAxisFromString]]

----
[[CategoryAPI]]

