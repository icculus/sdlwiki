====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_JoystickSetVirtualButton =

Set values on an opened, virtual-joystick's button.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_JoystickSetVirtualButton(SDL_Joystick *joystick, int button, Uint8 value);
</syntaxhighlight>

== Function Parameters ==

{|
|'''joystick'''
|the virtual joystick on which to set state.
|-
|'''button'''
|the specific button on the virtual joystick to set.
|-
|'''value'''
|the new value for the specified button.
|}

== Return Value ==

Returns 0 on success, -1 on error.

== Remarks ==

Please note that values set here will not be applied until the next call to
[[SDL_JoystickUpdate]], which can either be called directly, or can be
called indirectly through various other SDL APIs, including, but not
limited to the following: [[SDL_PollEvent]], [[SDL_PumpEvents]],
[[SDL_WaitEventTimeout]], [[SDL_WaitEvent]].

== Version ==

This function is available since SDL 2.0.14.

----
[[CategoryAPI]]

