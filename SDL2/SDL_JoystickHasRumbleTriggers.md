====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_JoystickHasRumbleTriggers =

Query whether a joystick has rumble support on triggers.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_JoystickHasRumbleTriggers(SDL_Joystick *joystick);
</syntaxhighlight>

== Function Parameters ==

{|
|'''joystick'''
|The joystick to query
|}

== Return Value ==

Return [[SDL_TRUE]] if the joystick has trigger rumble, [[SDL_FALSE]]
otherwise.

== Version ==

This function is available since SDL 2.0.18.

== Related Functions ==

:[[SDL_JoystickRumbleTriggers]]

----
[[CategoryAPI]]

