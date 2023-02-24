====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_ShowCursor =

Toggle whether or not the cursor is shown.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_ShowCursor(int toggle);
</syntaxhighlight>

== Function Parameters ==

{|
|'''toggle'''
|<code>[[SDL_ENABLE]]</code> to show the cursor, <code>[[SDL_DISABLE]]</code> to hide it, <code>[[SDL_QUERY]]</code> to query the current state without changing it.
|}

== Return Value ==

Returns <code>[[SDL_ENABLE]]</code> if the cursor is shown, or
<code>[[SDL_DISABLE]]</code> if the cursor is hidden, or a negative error
code on failure; call [[SDL_GetError]]() for more information.

== Remarks ==

The cursor starts off displayed but can be turned off. Passing
<code>[[SDL_ENABLE]]</code> displays the cursor and passing
<code>[[SDL_DISABLE]]</code> hides it.

The current state of the mouse cursor can be queried by passing
<code>[[SDL_QUERY]]</code>; either <code>[[SDL_DISABLE]]</code> or
<code>[[SDL_ENABLE]]</code> will be returned.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_CreateCursor]]
:[[SDL_SetCursor]]

----
[[CategoryAPI]]

