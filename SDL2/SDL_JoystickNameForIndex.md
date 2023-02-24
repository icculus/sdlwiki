====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_JoystickNameForIndex =

Get the implementation dependent name of a joystick.

== Syntax ==

<syntaxhighlight lang='c'>
const char* SDL_JoystickNameForIndex(int device_index);
</syntaxhighlight>

== Function Parameters ==

{|
|'''device_index'''
|the index of the joystick to query (the N'th joystick on the system)
|}

== Return Value ==

Returns the name of the selected joystick. If no name can be found, this
function returns NULL; call [[SDL_GetError]]() for more information.

== Remarks ==

This can be called before any joysticks are opened.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_JoystickName]]
:[[SDL_JoystickOpen]]

----
[[CategoryAPI]]

