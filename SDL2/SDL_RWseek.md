====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_RWseek =

Seek within an [[SDL_RWops]] data stream.

== Syntax ==

<syntaxhighlight lang='c'>
Sint64 SDL_RWseek(SDL_RWops *context,
                  Sint64 offset, int whence);
</syntaxhighlight>

== Function Parameters ==

{|
|'''context'''
|a pointer to an [[SDL_RWops]] structure
|-
|'''offset'''
|an offset in bytes, relative to '''whence''' location; can be negative
|-
|'''whence'''
|any of <code>RW_SEEK_SET</code>, <code>RW_SEEK_CUR</code>, <code>RW_SEEK_END</code>
|}

== Return Value ==

Returns the final offset in the data stream after the seek or -1 on error.

== Remarks ==

This function seeks to byte <code>offset</code>, relative to
<code>whence</code>.

<code>whence</code> may be any of the following values:

* <code>RW_SEEK_SET</code>: seek from the beginning of data
* <code>RW_SEEK_CUR</code>: seek relative to current read point
* <code>RW_SEEK_END</code>: seek relative to the end of data

If this stream can not seek, it will return -1.

[[SDL_RWseek]]() is actually a wrapper function that calls the
[[SDL_RWops]]'s <code>seek</code> method appropriately, to simplify
application development.

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
:[[SDL_RWtell]]
:[[SDL_RWwrite]]

----
[[CategoryAPI]]

