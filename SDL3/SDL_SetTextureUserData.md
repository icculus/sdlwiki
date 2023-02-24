====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_SetTextureUserData =

Associate a user-specified pointer with a texture.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_SetTextureUserData(SDL_Texture *texture, void *userdata);
</syntaxhighlight>

== Function Parameters ==

{|
|'''texture'''
|the texture to update.
|-
|'''userdata'''
|the pointer to associate with the texture.
|}

== Return Value ==

Returns 0 on success, or -1 if the texture is not valid.

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_GetTextureUserData]]

----
[[CategoryAPI]]

