====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetGamepadPath =

Get the implementation-dependent path for an opened gamepad.

== Syntax ==

<syntaxhighlight lang='c'>
const char* SDL_GetGamepadPath(SDL_Gamepad *gamepad);
</syntaxhighlight>

== Function Parameters ==

{|
|'''gamepad'''
|a gamepad identifier previously returned by [[SDL_OpenGamepad]]()
|}

== Return Value ==

Returns the implementation dependent path for the gamepad, or NULL if there
is no path or the identifier passed is invalid.

== Remarks ==

This is the same path as returned by [[SDL_GetGamepadNameForIndex]](), but
it takes a gamepad identifier instead of the (unstable) device index.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetGamepadInstancePath]]

----
[[CategoryAPI]]

