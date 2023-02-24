====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_Metal_CreateView =

Create a CAMetalLayer-backed NSView/UIView and attach it to the specified window.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_MetalView SDL_Metal_CreateView(SDL_Window * window);
</syntaxhighlight>

== Remarks ==

On macOS, this does ''not'' associate a MTLDevice with the CAMetalLayer on
its own. It is up to user code to do that.

The returned handle can be casted directly to a NSView or UIView. To access
the backing CAMetalLayer, call [[SDL_Metal_GetLayer]]().

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_Metal_DestroyView]]
:[[SDL_Metal_GetLayer]]

----
[[CategoryAPI]]

