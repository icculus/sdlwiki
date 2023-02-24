====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_RWclose =

Close and free an allocated [[SDL_RWops]] structure.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_RWclose(SDL_RWops *context);
</syntaxhighlight>

== Function Parameters ==

{|
|'''context'''
|[[SDL_RWops]] structure to close
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Remarks ==

[[SDL_RWclose]]() closes and cleans up the [[SDL_RWops]] stream. It
releases any resources used by the stream and frees the [[SDL_RWops]]
itself with [[SDL_FreeRW]](). This returns 0 on success, or -1 if the
stream failed to flush to its output (e.g. to disk).

Note that if this fails to flush the stream to disk, this function reports
an error, but the [[SDL_RWops]] is still invalid once this function
returns.

Prior to SDL 2.0.10, this function was a macro.

== Version ==

This function is available since SDL 2.0.10.

== Related Functions ==

:[[SDL_RWFromConstMem]]
:[[SDL_RWFromFile]]
:[[SDL_RWFromFP]]
:[[SDL_RWFromMem]]
:[[SDL_RWread]]
:[[SDL_RWseek]]
:[[SDL_RWwrite]]

----
[[CategoryAPI]]

