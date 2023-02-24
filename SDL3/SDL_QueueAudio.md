====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_QueueAudio =

Queue more audio on non-callback devices.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_QueueAudio(SDL_AudioDeviceID dev, const void *data, Uint32 len);
</syntaxhighlight>

== Function Parameters ==

{|
|'''dev'''
|the device ID to which we will queue audio
|-
|'''data'''
|the data to queue to the device for later playback
|-
|'''len'''
|the number of bytes (not samples!) to which <code>data</code> points
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Remarks ==

If you are looking to retrieve queued audio from a non-callback capture
device, you want [[SDL_DequeueAudio]]() instead. [[SDL_QueueAudio]]() will
return -1 to signify an error if you use it with capture devices.

SDL offers two ways to feed audio to the device: you can either supply a
callback that SDL triggers with some frequency to obtain more audio (pull
method), or you can supply no callback, and then SDL will expect you to
supply data at regular intervals (push method) with this function.

There are no limits on the amount of data you can queue, short of
exhaustion of address space. Queued data will drain to the device as
necessary without further intervention from you. If the device needs audio
but there is not enough queued, it will play silence to make up the
difference. This means you will have skips in your audio playback if you
aren't routinely queueing sufficient data.

This function copies the supplied data, so you are safe to free it when the
function returns. This function is thread-safe, but queueing to the same
device from two threads at once does not promise which buffer will be
queued first.

You may not queue audio on a device that is using an application-supplied
callback; doing so returns an error. You have to use the audio callback or
queue audio with this function, but not both.

You should not call [[SDL_LockAudio]]() on the device before queueing; SDL
handles locking internally for this function.

Note that SDL does not support planar audio. You will need to resample from
planar audio formats into a non-planar one (see [[SDL_AudioFormat]]) before
queuing audio.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_ClearQueuedAudio]]
:[[SDL_GetQueuedAudioSize]]

----
[[CategoryAPI]], [[CategoryAudio]]

