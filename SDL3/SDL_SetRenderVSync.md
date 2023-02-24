====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_SetRenderVSync =

Toggle VSync of the given renderer.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_SetRenderVSync(SDL_Renderer *renderer, int vsync);
</syntaxhighlight>

== Function Parameters ==

{|
|'''renderer'''
|The renderer to toggle
|-
|'''vsync'''
|1 for on, 0 for off. All other values are reserved
|}

== Return Value ==

Returns a 0 int on success, or non-zero on failure

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

