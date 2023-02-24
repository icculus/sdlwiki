====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_DestroyAudioStream =

Free an audio stream 

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_DestroyAudioStream(SDL_AudioStream *stream);
</syntaxhighlight>

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_CreateAudioStream]]
:[[SDL_PutAudioStreamData]]
:[[SDL_GetAudioStreamData]]
:[[SDL_GetAudioStreamAvailable]]
:[[SDL_FlushAudioStream]]
:[[SDL_ClearAudioStream]]

----
[[CategoryAPI]]

