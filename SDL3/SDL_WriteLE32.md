====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_WriteLE32 =

Use this function to write 32 bits in native format to a [[SDL_RWops]] as little-endian data.

== Syntax ==

<syntaxhighlight lang='c'>
size_t SDL_WriteLE32(SDL_RWops * dst, Uint32 value);
</syntaxhighlight>

== Function Parameters ==

{|
|'''dst'''
|the stream to which data will be written
|-
|'''value'''
|the data to be written, in native format
|}

== Return Value ==

Returns 1 on successful write, 0 on error.

== Remarks ==

SDL byteswaps the data only if necessary, so the application always
specifies native format, and the data written will be in little-endian
format.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_WriteBE32]]

----
[[CategoryAPI]], [[CategoryIO]]

