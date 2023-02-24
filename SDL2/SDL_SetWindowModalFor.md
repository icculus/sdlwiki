====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_SetWindowModalFor =

Set the window as a modal for another window.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_SetWindowModalFor(SDL_Window * modal_window, SDL_Window * parent_window);
</syntaxhighlight>

== Function Parameters ==

{|
|'''modal_window'''
|the window that should be set modal
|-
|'''parent_window'''
|the parent window for the modal window
|}

== Return Value ==

Returns 0 on success or a negative error code on failure; call
[[SDL_GetError]]() for more information.

== Version ==

This function is available since SDL 2.0.5.

----
[[CategoryAPI]]

