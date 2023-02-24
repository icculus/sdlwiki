====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_RenderPoint =

Draw a point on the current rendering target at subpixel precision.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_RenderPoint(SDL_Renderer *renderer, float x, float y);
</syntaxhighlight>

== Function Parameters ==

{|
|'''renderer'''
|The renderer which should draw a point.
|-
|'''x'''
|The x coordinate of the point.
|-
|'''y'''
|The y coordinate of the point.
|}

== Return Value ==

Return 0 on success, or -1 on error

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

