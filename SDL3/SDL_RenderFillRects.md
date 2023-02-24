====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_RenderFillRects =

Fill some number of rectangles on the current rendering target with the drawing color at subpixel precision.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_RenderFillRects(SDL_Renderer *renderer, const SDL_FRect *rects, int count);
</syntaxhighlight>

== Function Parameters ==

{|
|'''renderer'''
|The renderer which should fill multiple rectangles.
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
[[CategoryAPI]], [[CategoryRender]]

