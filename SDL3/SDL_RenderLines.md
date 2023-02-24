====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_RenderLines =

Draw a series of connected lines on the current rendering target at subpixel precision.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_RenderLines(SDL_Renderer *renderer, const SDL_FPoint *points, int count);
</syntaxhighlight>

== Function Parameters ==

{|
|'''renderer'''
|The renderer which should draw multiple lines.
|-
|'''points'''
|The points along the lines
|-
|'''count'''
|The number of points, drawing count-1 lines
|}

== Return Value ==

Return 0 on success, or -1 on error

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

