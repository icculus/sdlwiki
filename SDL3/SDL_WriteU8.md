====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======

== Draft ==

'''THIS PAGE IS A WORK IN PROGRESS''' ... Please make edits to this page to improve it!


<!-- #*^*^*^*^*See https://wiki.libsdl.org/SGFunctions for details on editing this page*^*^*^*^* -->
= SDL_WriteU8 =

Use this function to write a byte to an [[SDL_RWops]].

== Syntax ==

<syntaxhighlight lang='c'>
size_t SDL_WriteU8(SDL_RWops * dst, Uint8 value);
</syntaxhighlight>

== Function Parameters ==

{|
|'''dst'''
|the [[SDL_RWops]] to write to
|-
|'''value'''
|the byte value to write
|}

== Return Value ==

Returns 1 on success or 0 on failure; call [[SDL_GetError]]() for more
information.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_ReadU8]]

----
[[CategoryAPI]], [[CategoryIO]], [[CategoryDraft]]

