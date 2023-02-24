====== (This function is part of SDL_mixer, a separate library from SDL.) ======
= Mix_AllocateChannels =

Dynamically change the number of channels managed by the mixer.

== Syntax ==

<syntaxhighlight lang='c'>
int Mix_AllocateChannels(int numchans);
</syntaxhighlight>

== Function Parameters ==

{|
|'''numchans'''
|the new number of channels, or < 0 to query current channel count.
|}

== Return Value ==

Returns the new number of allocated channels.

== Remarks ==

SDL_mixer deals with "channels," which is not the same thing as the
mono/stereo channels; they might be better described as "tracks," as each
one corresponds to a separate source of audio data. Three different WAV
files playing at the same time would be three separate SDL_mixer channels,
for example.

An app needs as many channels as it has audio data it wants to play
simultaneously, mixing them into a single stream to send to the audio
device.

SDL_mixer allocates <code>[[MIX_CHANNELS]]</code> (currently 8) channels
when you open an audio device, which may be more than an app needs, but if
the app needs more or wants less, this function can change it.

If decreasing the number of channels, any upper channels currently playing
are stopped. This will deregister all effects on those channels and call
any callback specified by [[Mix_ChannelFinished]]() for each removed
channel.

If <code>numchans</code> is less than zero, this will return the current
number of channels without changing anything.

== Version ==

This function is available since SDL_mixer 2.0.0.

----
[[CategoryAPI]]

