====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetGamepadBindForButton =

Get the SDL joystick layer binding for a gamepad button mapping.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_GamepadBinding SDL_GetGamepadBindForButton(SDL_Gamepad *gamepad, SDL_GamepadButton button);
</syntaxhighlight>

== Function Parameters ==

{|
|'''gamepad'''
|a gamepad
|-
|'''button'''
|an button enum value (an [[SDL_GamepadButton]] value)
|}

== Return Value ==

Returns a [[SDL_GamepadBinding]] describing the bind. On failure (like the
given Controller button doesn't exist on the device), its
<code>.bindType</code> will be <code>[[SDL_GAMEPAD_BINDTYPE_NONE]]</code>.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetGamepadBindForAxis]]

----
[[CategoryAPI]]

