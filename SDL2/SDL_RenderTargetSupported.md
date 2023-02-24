====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_RenderTargetSupported =

Determine whether a renderer supports the use of render targets.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_RenderTargetSupported(SDL_Renderer *renderer);
</syntaxhighlight>

== Function Parameters ==

{|
|'''renderer'''
|the renderer that will be checked
|}

== Return Value ==

Returns [[SDL_TRUE]] if supported or [[SDL_FALSE]] if not.

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_SetRenderTarget]]

----
[[CategoryAPI]]

