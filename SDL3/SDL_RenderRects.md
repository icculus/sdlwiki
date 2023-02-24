====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_RenderRects =

Draw some number of rectangles on the current rendering target at subpixel precision.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_RenderRects(SDL_Renderer *renderer, const SDL_FRect *rects, int count);
</syntaxhighlight>

== Function Parameters ==

{|
|'''renderer'''
|The renderer which should draw multiple rectangles.
|-
|'''rects'''
|A pointer to an array of destination rectangles.
|-
|'''count'''
|The number of rectangles.
|}

== Return Value ==

Return 0 on success, or -1 on error

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

