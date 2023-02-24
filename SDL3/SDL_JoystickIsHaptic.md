====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======

== Draft ==

'''THIS PAGE IS A WORK IN PROGRESS''' ... Please make edits to this page to improve it!
= SDL_JoystickIsHaptic =

Query if a joystick has haptic features.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_JoystickIsHaptic(SDL_Joystick * joystick);
</syntaxhighlight>

== Function Parameters ==

{|
|'''joystick'''
|the [[SDL_Joystick]] to test for haptic capabilities
|}

== Return Value ==

Returns [[SDL_TRUE]] if the joystick is haptic, [[SDL_FALSE]] if it isn't,
or a negative error code on failure; call [[SDL_GetError]]() for more
information.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_HapticOpenFromJoystick]]

----
[[CategoryAPI]], [[CategoryForceFeedback]], [[CategoryDraft]]

