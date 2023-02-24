====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_DestroyWindow =

Destroy a window.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_DestroyWindow(SDL_Window *window);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window to destroy
|}

== Remarks ==

If <code>window</code> is NULL, this function will return immediately after
setting the SDL error message to "Invalid window". See [[SDL_GetError]]().

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_CreateWindow]]
:[[SDL_CreateWindowFrom]]

----
[[CategoryAPI]], [[CategoryVideo]]

