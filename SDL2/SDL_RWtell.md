====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_RWtell =

Determine the current read/write offset in an [[SDL_RWops]] data stream.

== Syntax ==

<syntaxhighlight lang='c'>
Sint64 SDL_RWtell(SDL_RWops *context);
</syntaxhighlight>

== Function Parameters ==

{|
|'''context'''
|a [[SDL_RWops]] data stream object from which to get the current offset
|}

== Return Value ==

Returns the current offset in the stream, or -1 if the information can not
be determined.

== Remarks ==

[[SDL_RWtell]] is actually a wrapper function that calls the
[[SDL_RWops]]'s <code>seek</code> method, with an offset of 0 bytes from
<code>RW_SEEK_CUR</code>, to simplify application development.

Prior to SDL 2.0.10, this function was a macro.

== Version ==

This function is available since SDL 2.0.10.

== Related Functions ==

:[[SDL_RWclose]]
:[[SDL_RWFromConstMem]]
:[[SDL_RWFromFile]]
:[[SDL_RWFromFP]]
:[[SDL_RWFromMem]]
:[[SDL_RWread]]
:[[SDL_RWseek]]
:[[SDL_RWwrite]]

----
[[CategoryAPI]]

