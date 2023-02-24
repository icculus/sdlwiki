====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_JoystickNumAxes =

Get the number of general axis controls on a joystick.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_JoystickNumAxes(SDL_Joystick *joystick);
</syntaxhighlight>

== Function Parameters ==

{|
|'''joystick'''
|an [[SDL_Joystick]] structure containing joystick information
|}

== Return Value ==

Returns the number of axis controls/number of axes on success or a negative
error code on failure; call [[SDL_GetError]]() for more information.

== Remarks ==

Often, the directional pad on a game controller will either look like 4
separate buttons or a POV hat, and not axes, but all of this is up to the
device and platform.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_JoystickGetAxis]]
:[[SDL_JoystickOpen]]

----
[[CategoryAPI]]

