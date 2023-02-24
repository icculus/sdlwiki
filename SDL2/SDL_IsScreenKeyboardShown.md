====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_IsScreenKeyboardShown =

Check whether the screen keyboard is shown for given window.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_IsScreenKeyboardShown(SDL_Window *window);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window for which screen keyboard should be queried
|}

== Return Value ==

Returns [[SDL_TRUE]] if screen keyboard is shown or [[SDL_FALSE]] if not.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_HasScreenKeyboardSupport]]

----
[[CategoryAPI]]

