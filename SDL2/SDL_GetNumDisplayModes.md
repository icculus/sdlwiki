====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GetNumDisplayModes =

Get the number of available display modes.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_GetNumDisplayModes(int displayIndex);
</syntaxhighlight>

== Function Parameters ==

{|
|'''displayIndex'''
|the index of the display to query
|}

== Return Value ==

Returns a number >= 1 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Remarks ==

The <code>displayIndex</code> needs to be in the range from 0 to
[[SDL_GetNumVideoDisplays]]() - 1.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GetDisplayMode]]
:[[SDL_GetNumVideoDisplays]]

----
[[CategoryAPI]]

