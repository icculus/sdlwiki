====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetRectIntersection =

Calculate the intersection of two rectangles.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_GetRectIntersection(const SDL_Rect * A,
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
|an [[SDL_Rect]] structure filled in with the intersection of rectangles <code>A</code> and <code>B</code>
|}

== Return Value ==

Returns [[SDL_TRUE]] if there is an intersection, [[SDL_FALSE]] otherwise.

== Remarks ==

If <code>result</code> is NULL then this function will return
[[SDL_FALSE]].

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_HasRectIntersection]]

----
[[CategoryAPI]]

