====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_DestroyPalette =

Free a palette created with [[SDL_CreatePalette]]().

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_DestroyPalette(SDL_Palette * palette);
</syntaxhighlight>

== Function Parameters ==

{|
|'''palette'''
|the [[SDL_Palette]] structure to be freed
|}

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_CreatePalette]]

----
[[CategoryAPI]]

