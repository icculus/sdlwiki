====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_RenderPresent =

Update the screen with any rendering performed since the previous call.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_RenderPresent(SDL_Renderer *renderer);
</syntaxhighlight>

== Function Parameters ==

{|
|'''renderer'''
|the rendering context
|}

== Remarks ==

SDL's rendering functions operate on a backbuffer; that is, calling a
rendering function such as [[SDL_RenderLine]]() does not directly put a
line on the screen, but rather updates the backbuffer. As such, you compose
your entire scene and ''present'' the composed backbuffer to the screen as
a complete picture.

Therefore, when using SDL's rendering API, one does all drawing intended
for the frame, and then calls this function once per frame to present the
final drawing to the user.

The backbuffer should be considered invalidated after each present; do not
assume that previous contents will exist between frames. You are strongly
encouraged to call [[SDL_RenderClear]]() to initialize the backbuffer
before starting each new frame's drawing, even if you plan to overwrite
every pixel.

== Thread Safety ==

You may only call this function on the main thread.

== Version ==

This function is available since SDL 3.0.0.

== Code Examples ==

Please refer to the code example in [[SDL_RenderClear]].

== Related Functions ==

:[[SDL_RenderClear]]
:[[SDL_RenderLine]]
:[[SDL_RenderLines]]
:[[SDL_RenderPoint]]
:[[SDL_RenderPoints]]
:[[SDL_RenderRect]]
:[[SDL_RenderRects]]
:[[SDL_RenderFillRect]]
:[[SDL_RenderFillRects]]
:[[SDL_SetRenderDrawBlendMode]]
:[[SDL_SetRenderDrawColor]]

----
[[CategoryAPI]], [[CategoryRender]]

