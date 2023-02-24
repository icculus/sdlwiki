====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetJoystickProduct =

Get the USB product ID of an opened joystick, if available.

== Syntax ==

<syntaxhighlight lang='c'>
Uint16 SDL_GetJoystickProduct(SDL_Joystick *joystick);
</syntaxhighlight>

== Function Parameters ==

{|
|'''joystick'''
|the [[SDL_Joystick]] obtained from [[SDL_OpenJoystick]]()
|}

== Return Value ==

Returns the USB product ID of the selected joystick, or 0 if unavailable.

== Remarks ==

If the product ID isn't available this function returns 0.

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

