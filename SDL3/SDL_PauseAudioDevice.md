====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_PauseAudioDevice =

Use this function to pause audio playback on a specified device.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_PauseAudioDevice(SDL_AudioDeviceID dev);
</syntaxhighlight>

== Function Parameters ==

{|
|'''dev'''
|a device opened by [[SDL_OpenAudioDevice]]()
|}

== Remarks ==

This function pauses the audio callback processing for a given device.
Silence will be written to the audio device while paused, and the audio
callback is guaranteed to not be called. Pausing one device does not
prevent other unpaused devices from running their callbacks.

If you just need to protect a few variables from race conditions vs your
callback, you shouldn't pause the audio device, as it will lead to dropouts
in the audio playback. Instead, you should use [[SDL_LockAudioDevice]]().

== Version ==

This function is available since SDL 3.0.0.

== Code Examples ==

<syntaxhighlight lang='c++'>
extern SDL_AudioDeviceID devid;
SDL_PauseAudioDevice(devid, 1);  // audio callback is stopped when this returns.
SDL_Delay(5000);  // audio device plays silence for 5 seconds
SDL_PauseAudioDevice(devid, 0);  // audio callback starts running again.
</syntaxhighlight>

== Related Functions ==

:[[SDL_LockAudioDevice]]
:[[SDL_PlayAudioDevice]]

----
[[CategoryAPI]], [[CategoryAudio]]

