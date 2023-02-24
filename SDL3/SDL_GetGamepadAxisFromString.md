====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetGamepadAxisFromString =

Convert a string into [[SDL_GamepadAxis]] enum.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_GamepadAxis SDL_GetGamepadAxisFromString(const char *str);
</syntaxhighlight>

== Function Parameters ==

{|
|'''str'''
|string representing a [[SDL_Gamepad]] axis
|}

== Return Value ==

Returns the [[SDL_GamepadAxis]] enum corresponding to the input string, or
<code>[[SDL_GAMEPAD_AXIS_INVALID]]</code> if no match was found.

== Remarks ==

This function is called internally to translate [[SDL_Gamepad]] mapping
strings for the underlying joystick device into the consistent
[[SDL_Gamepad]] mapping. You do not normally need to call this function
unless you are parsing [[SDL_Gamepad]] mappings in your own code.

Note specially that "righttrigger" and "lefttrigger" map to
<code>[[SDL_GAMEPAD_AXIS_RIGHT_TRIGGER]]</code> and
<code>[[SDL_GAMEPAD_AXIS_LEFT_TRIGGER]]</code>, respectively.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetGamepadStringForAxis]]

----
[[CategoryAPI]]

