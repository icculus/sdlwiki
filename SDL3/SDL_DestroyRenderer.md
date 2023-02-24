====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_DestroyRenderer =

Destroy the rendering context for a window and free associated textures.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_DestroyRenderer(SDL_Renderer *renderer);
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

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_CreateRenderer]]

----
[[CategoryAPI]], [[CategoryRender]]

