====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
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

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_HapticOpenFromJoystick]]

----
[[CategoryAPI]]

