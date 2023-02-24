====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======

== Draft ==

'''THIS PAGE IS A WORK IN PROGRESS''' ... Please make edits to this page to improve it!
= SDL_HapticNumAxes =

Get the number of haptic axes the device has.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_HapticNumAxes(SDL_Haptic * haptic);
</syntaxhighlight>

== Function Parameters ==

{|
|'''haptic'''
|the [[SDL_Haptic]] device to query
|}

== Return Value ==

Returns the number of axes on success or a negative error code on failure;
call [[SDL_GetError]]() for more information.

== Remarks ==

The number of haptic axes might be useful if working with the
[[SDL_HapticDirection]] effect.

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]], [[CategoryForceFeedback]], [[CategoryDraft]]

