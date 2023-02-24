====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_DestroyCursor =

Free a previously-created cursor.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_DestroyCursor(SDL_Cursor * cursor);
</syntaxhighlight>

== Function Parameters ==

{|
|'''cursor'''
|the cursor to free
|}

== Remarks ==

Use this function to free cursor resources created with
[[SDL_CreateCursor]](), [[SDL_CreateColorCursor]]() or
[[SDL_CreateSystemCursor]]().

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_CreateColorCursor]]
:[[SDL_CreateCursor]]
:[[SDL_CreateSystemCursor]]

----
[[CategoryAPI]]

