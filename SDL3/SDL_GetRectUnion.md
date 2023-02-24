====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetRectUnion =

Calculate the union of two rectangles.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_GetRectUnion(const SDL_Rect * A,
                   const SDL_Rect * B,
                   SDL_Rect * result);
</syntaxhighlight>

== Function Parameters ==

{|
|'''A'''
|an [[SDL_Rect]] structure representing the first rectangle
|-
|'''B'''
|an [[SDL_Rect]] structure representing the second rectangle
|-
|'''result'''
|an [[SDL_Rect]] structure filled in with the union of rectangles <code>A</code> and <code>B</code>
|}

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

