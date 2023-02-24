====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_JoystickClose =

Close a joystick previously opened with [[SDL_JoystickOpen]]().

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_JoystickClose(SDL_Joystick *joystick);
</syntaxhighlight>

== Function Parameters ==

{|
|'''joystick'''
|The joystick device to close
|}

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_JoystickOpen]]

----
[[CategoryAPI]]

