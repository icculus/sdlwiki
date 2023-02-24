====== (This function is part of SDL_mixer, a separate library from SDL.) ======
= Mix_GetChunkDecoder =

Get a chunk decoder's name.

== Syntax ==

<syntaxhighlight lang='c'>
const char * Mix_GetChunkDecoder(int index);
</syntaxhighlight>

== Function Parameters ==

{|
|'''index'''
|index of the chunk decoder.
|}

== Return Value ==

Returns the chunk decoder's name.

== Remarks ==

The requested decoder's index must be between zero and
[[Mix_GetNumChunkDecoders]]()-1. It's safe to call this with an invalid
index; this function will return NULL in that case.

This list can change between builds AND runs of the program, if external
libraries that add functionality become available. You must successfully
call [[Mix_OpenAudio]]() or [[Mix_OpenAudioDevice]]() before calling this
function, as decoders are activated at device open time.

== Version ==

This function is available since SDL_mixer 2.0.0.

== Related Functions ==

:[[Mix_GetNumChunkDecoders]]

----
[[CategoryAPI]]

