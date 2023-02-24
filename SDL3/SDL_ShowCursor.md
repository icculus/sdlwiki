====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======

== Draft ==

'''THIS PAGE IS A WORK IN PROGRESS''' ... Please make edits to this page to improve it!
= SDL_ShowCursor =

Show the cursor.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_ShowCursor(void);
</syntaxhighlight>

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 3.0.0.

== Code Examples ==

<syntaxhighlight lang='c++'>
int main(int argc, char *argv[]) {
    /* creates a blank cursor */
    SDL_ShowCursor(SDL_DISABLE);
    /* ... */
    return 0;
}
</syntaxhighlight>

== Related Functions ==

:[[SDL_CursorVisible]]
:[[SDL_HideCursor]]

----
[[CategoryAPI]], [[CategoryMouse]], [[CategoryDraft]]

