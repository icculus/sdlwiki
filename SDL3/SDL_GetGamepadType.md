====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetGamepadType =

Get the type of this currently opened gamepad 

== Syntax ==

<syntaxhighlight lang='c'>
SDL_GamepadType SDL_GetGamepadType(SDL_Gamepad *gamepad);
</syntaxhighlight>

== Function Parameters ==

{|
|'''gamepad'''
|the gamepad object to query.
|}

== Return Value ==

Returns the gamepad type.

== Remarks ==

This is the same name as returned by [[SDL_GetGamepadInstanceType]](), but
it takes a gamepad identifier instead of the (unstable) device index.

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

