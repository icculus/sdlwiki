====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_SetWindowIcon =

Set the icon for a window.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_SetWindowIcon(SDL_Window * window,
                       SDL_Surface * icon);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window to change
|-
|'''icon'''
|an [[SDL_Surface]] structure containing the icon for the window
|}

== Version ==

This function is available since SDL 2.0.0.

----
[[CategoryAPI]]

