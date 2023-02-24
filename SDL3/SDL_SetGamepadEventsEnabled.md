====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_SetGamepadEventsEnabled =

Set the state of gamepad event processing.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_SetGamepadEventsEnabled(SDL_bool enabled);
</syntaxhighlight>

== Function Parameters ==

{|
|'''enabled'''
|whether to process gamepad events or not
|}

== Remarks ==

If gamepad events are disabled, you must call [[SDL_UpdateGamepads]]()
yourself and check the state of the gamepad when you want gamepad
information.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GamepadEventsEnabled]]

----
[[CategoryAPI]]

