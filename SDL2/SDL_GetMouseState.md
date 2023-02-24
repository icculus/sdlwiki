====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GetMouseState =

Retrieve the current state of the mouse.

== Syntax ==

<syntaxhighlight lang='c'>
Uint32 SDL_GetMouseState(int *x, int *y);
</syntaxhighlight>

== Function Parameters ==

{|
|'''x'''
|the x coordinate of the mouse cursor position relative to the focus window
|-
|'''y'''
|the y coordinate of the mouse cursor position relative to the focus window
|}

== Return Value ==

Returns a 32-bit button bitmask of the current button state.

== Remarks ==

The current button state is returned as a button bitmask, which can be
tested using the <code>[[SDL_BUTTON]](X)</code> macros (where
<code>X</code> is generally 1 for the left, 2 for middle, 3 for the right
button), and <code>x</code> and <code>y</code> are set to the mouse cursor
position relative to the focus window. You can pass NULL for either
<code>x</code> or <code>y</code>.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_GetGlobalMouseState]]
:[[SDL_GetRelativeMouseState]]
:[[SDL_PumpEvents]]

----
[[CategoryAPI]]

