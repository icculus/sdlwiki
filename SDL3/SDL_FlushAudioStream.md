====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_FlushAudioStream =

Tell the stream that you're done sending data, and anything being buffered should be converted/resampled and made available immediately.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_FlushAudioStream(SDL_AudioStream *stream);
</syntaxhighlight>

== Remarks ==

It is legal to add more data to a stream after flushing, but there will be
audio gaps in the output. Generally this is intended to signal the end of
input, so the complete output becomes available.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_CreateAudioStream]]
:[[SDL_PutAudioStreamData]]
:[[SDL_GetAudioStreamData]]
:[[SDL_GetAudioStreamAvailable]]
:[[SDL_ClearAudioStream]]
:[[SDL_DestroyAudioStream]]

----
[[CategoryAPI]]

