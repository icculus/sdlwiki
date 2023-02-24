====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GamepadHasButton =

Query whether a gamepad has a given button.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_GamepadHasButton(SDL_Gamepad *gamepad, SDL_GamepadButton button);
</syntaxhighlight>

== Function Parameters ==

{|
|'''gamepad'''
|a gamepad
|-
|'''button'''
|a button enum value (an [[SDL_GamepadButton]] value)
|}

== Return Value ==

Returns [[SDL_TRUE]] if the gamepad has this button, [[SDL_FALSE]]
otherwise.

== Remarks ==

This merely reports whether the gamepad's mapping defined this button, as
that is all the information SDL has about the physical device.

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

