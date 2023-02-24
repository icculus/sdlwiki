====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======

== Draft ==

'''THIS PAGE IS A WORK IN PROGRESS''' ... Please make edits to this page to improve it!
= SDL_SetCursor =

Set the active cursor.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_SetCursor(SDL_Cursor * cursor);
</syntaxhighlight>

== Function Parameters ==

{|
|'''cursor'''
|a cursor to make active
|}

== Remarks ==

This function sets the currently active cursor to the specified one. If the
cursor is currently visible, the change will be immediately represented on
the display. [[SDL_SetCursor]](NULL) can be used to force cursor redraw, if
this is desired for any reason.

== Version ==

This function is available since SDL 3.0.0.

== Code Examples ==

<syntaxhighlight lang='c++'>
You can add your code example here
</syntaxhighlight>

== Related Functions ==

:[[SDL_CreateCursor]]
:[[SDL_GetCursor]]

----
[[CategoryAPI]], [[CategoryMouse]], [[CategoryDraft]]

