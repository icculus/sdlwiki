====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_AudioStreamClear =

Clear any pending data in the stream without converting it 

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_AudioStreamClear(SDL_AudioStream *stream);
</syntaxhighlight>

== Version ==

This function is available since SDL 2.0.7.

== Related Functions ==

:[[SDL_NewAudioStream]]
:[[SDL_AudioStreamPut]]
:[[SDL_AudioStreamGet]]
:[[SDL_AudioStreamAvailable]]
:[[SDL_AudioStreamFlush]]
:[[SDL_FreeAudioStream]]

----
[[CategoryAPI]]

