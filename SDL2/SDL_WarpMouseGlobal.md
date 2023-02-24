====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_WarpMouseGlobal =

Move the mouse to the given position in global screen space.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_WarpMouseGlobal(int x, int y);
</syntaxhighlight>

== Function Parameters ==

{|
|'''x'''
|the x coordinate
|-
|'''y'''
|the y coordinate
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Remarks ==

This function generates a mouse motion event.

A failure of this function usually means that it is unsupported by a
platform.

Note that this function will appear to succeed, but not actually move the
mouse when used over Microsoft Remote Desktop.

== Version ==

This function is available since SDL 2.0.4.

== Related Functions ==

:[[SDL_WarpMouseInWindow]]

----
[[CategoryAPI]]

