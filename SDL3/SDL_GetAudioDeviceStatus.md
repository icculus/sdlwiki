====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetAudioDeviceStatus =

Use this function to get the current audio state of an audio device.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_AudioStatus SDL_GetAudioDeviceStatus(SDL_AudioDeviceID dev);
</syntaxhighlight>

== Function Parameters ==

{|
|'''dev'''
|the ID of an audio device previously opened with [[SDL_OpenAudioDevice]]()
|}

== Return Value ==

Returns the [[SDL_AudioStatus]] of the specified audio device.

== Version ==

This function is available since SDL 3.0.0.

== Code Examples ==

<<Include(SDL_AudioStatus, , , from="== Code Examples ==", to="== Remarks ==")>>

== Related Functions ==

:[[SDL_PlayAudioDevice]]
:[[SDL_PauseAudioDevice]]

----
[[CategoryAPI]], [[CategoryAudio]]

