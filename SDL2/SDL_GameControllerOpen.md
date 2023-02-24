====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GameControllerOpen =

Open a game controller for use.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_GameController* SDL_GameControllerOpen(int joystick_index);
</syntaxhighlight>

== Function Parameters ==

{|
|'''joystick_index'''
|the device_index of a device, up to [[SDL_NumJoysticks]]()
|}

== Return Value ==

Returns a gamecontroller identifier or NULL if an error occurred; call
[[SDL_GetError]]() for more information.

== Remarks ==

<code>joystick_index</code> is the same as the <code>device_index</code>
passed to [[SDL_JoystickOpen]]().

The index passed as an argument refers to the N'th game controller on the
system. This index is not the value which will identify this controller in
future controller events. The joystick's instance id ([[SDL_JoystickID]])
will be used there instead.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GameControllerClose]]
:[[SDL_GameControllerNameForIndex]]
:[[SDL_IsGameController]]

----
[[CategoryAPI]]

