====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_SendGamepadEffect =

Send a gamepad specific effect packet 

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_SendGamepadEffect(SDL_Gamepad *gamepad, const void *data, int size);
</syntaxhighlight>

== Function Parameters ==

{|
|'''gamepad'''
|The gamepad to affect
|-
|'''data'''
|The data to send to the gamepad
|-
|'''size'''
|The size of the data to send to the gamepad
|}

== Return Value ==

Returns 0, or -1 if this gamepad or driver doesn't support effect packets

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

