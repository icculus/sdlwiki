====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======

== Draft ==

'''THIS PAGE IS A WORK IN PROGRESS''' ... Please make edits to this page to improve it!
= SDL_HapticRumbleInit =

Initialize a haptic device for simple rumble playback.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_HapticRumbleInit(SDL_Haptic * haptic);
</syntaxhighlight>

== Function Parameters ==

{|
|'''haptic'''
|the haptic device to initialize for simple rumble playback
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_HapticOpen]]
:[[SDL_HapticRumblePlay]]
:[[SDL_HapticRumbleStop]]
:[[SDL_HapticRumbleSupported]]

----
[[CategoryAPI]], [[CategoryForceFeedback]], [[CategoryDraft]]

