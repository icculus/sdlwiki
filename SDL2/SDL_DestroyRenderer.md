====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_DestroyRenderer =

Destroy the rendering context for a window and free associated textures.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_DestroyRenderer(SDL_Renderer * renderer);
</syntaxhighlight>

== Function Parameters ==

{|
|'''renderer'''
|the rendering context
|}

== Remarks ==

If <code>renderer</code> is NULL, this function will return immediately
after setting the SDL error message to "Invalid renderer". See
[[SDL_GetError]]().

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_CreateRenderer]]

----
[[CategoryAPI]]

