====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_IsGameController =

Check if the given joystick is supported by the game controller interface.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_IsGameController(int joystick_index);
</syntaxhighlight>

== Function Parameters ==

{|
|'''joystick_index'''
|the device_index of a device, up to [[SDL_NumJoysticks]]()
|}

== Return Value ==

Returns [[SDL_TRUE]] if the given joystick is supported by the game
controller interface, [[SDL_FALSE]] if it isn't or it's an invalid index.

== Remarks ==

<code>joystick_index</code> is the same as the <code>device_index</code>
passed to [[SDL_JoystickOpen]]().

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GameControllerNameForIndex]]
:[[SDL_GameControllerOpen]]

----
[[CategoryAPI]]

