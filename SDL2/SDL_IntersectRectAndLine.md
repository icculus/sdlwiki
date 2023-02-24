====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_IntersectRectAndLine =

Calculate the intersection of a rectangle and line segment.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_IntersectRectAndLine(const SDL_Rect *
                                  rect, int *X1,
                                  int *Y1, int *X2,
                                  int *Y2);
</syntaxhighlight>

== Function Parameters ==

{|
|'''rect'''
|an [[SDL_Rect]] structure representing the rectangle to intersect
|-
|'''X1'''
|a pointer to the starting X-coordinate of the line
|-
|'''Y1'''
|a pointer to the starting Y-coordinate of the line
|-
|'''X2'''
|a pointer to the ending X-coordinate of the line
|-
|'''Y2'''
|a pointer to the ending Y-coordinate of the line
|}

== Return Value ==

Returns [[SDL_TRUE]] if there is an intersection, [[SDL_FALSE]] otherwise.

== Remarks ==

This function is used to clip a line segment to a rectangle. A line segment
contained entirely within the rectangle or that does not intersect will
remain unchanged. A line segment that crosses the rectangle at either or
both ends will be clipped to the boundary of the rectangle and the new
coordinates saved in <code>X1</code>, <code>Y1</code>, <code>X2</code>,
and/or <code>Y2</code> as necessary.

== Version ==

This function is available since SDL 2.0.0.

----
[[CategoryAPI]]

