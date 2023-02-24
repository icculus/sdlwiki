====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======

== Draft ==

'''THIS PAGE IS A WORK IN PROGRESS''' ... Please make edits to this page to improve it!
= SDL_HapticOpen =

Open a haptic device for use.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_Haptic* SDL_HapticOpen(int device_index);
</syntaxhighlight>

== Function Parameters ==

{|
|'''device_index'''
|index of the device to open
|}

== Return Value ==

Returns the device identifier or NULL on failure; call [[SDL_GetError]]()
for more information.

== Remarks ==

The index passed as an argument refers to the N'th haptic device on this
system.

When opening a haptic device, its gain will be set to maximum and
autocenter will be disabled. To modify these values use
[[SDL_HapticSetGain]]() and [[SDL_HapticSetAutocenter]]().

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_HapticClose]]
:[[SDL_HapticIndex]]
:[[SDL_HapticOpenFromJoystick]]
:[[SDL_HapticOpenFromMouse]]
:[[SDL_HapticPause]]
:[[SDL_HapticSetAutocenter]]
:[[SDL_HapticSetGain]]
:[[SDL_HapticStopAll]]

----
[[CategoryAPI]], [[CategoryForceFeedback]], [[CategoryDraft]]

