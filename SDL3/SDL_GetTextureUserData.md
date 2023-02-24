====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_GetTextureUserData =

Get the user-specified pointer associated with a texture 

== Syntax ==

<syntaxhighlight lang='c'>
void* SDL_GetTextureUserData(SDL_Texture *texture);
</syntaxhighlight>

== Function Parameters ==

{|
|'''texture'''
|the texture to query.
|}

== Return Value ==

Return the pointer associated with the texture, or NULL if the texture is
not valid.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_SetTextureUserData]]

----
[[CategoryAPI]]

