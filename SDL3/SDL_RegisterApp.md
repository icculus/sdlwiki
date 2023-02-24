====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_RegisterApp =

Register a win32 window class for SDL's use.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_RegisterApp(const char *name, Uint32 style, void *hInst);
</syntaxhighlight>

== Function Parameters ==

{|
|'''name'''
|the window class name, in UTF-8 encoding. If NULL, SDL currently uses "[[SDL_app]]" but this isn't guaranteed.
|-
|'''style'''
|the value to use in WNDCLASSEX::style. If <code>name</code> is NULL, SDL currently uses <code>(CS_BYTEALIGNCLIENT | CS_OWNDC)</code> regardless of what is specified here.
|-
|'''hInst'''
|the HINSTANCE to use in WNDCLASSEX::hInstance. If zero, SDL will use <code>GetModuleHandle(NULL)</code> instead.
|}

== Return Value ==

Returns 0 on success, -1 on error. [[SDL_GetError]]() may have details.

== Remarks ==

This can be called to set the application window class at startup. It is
safe to call this multiple times, as long as every call is eventually
paired with a call to [[SDL_UnregisterApp]], but a second registration
attempt while a previous registration is still active will be ignored,
other than to increment a counter.

Most applications do not need to, and should not, call this directly; SDL
will call it when initializing the video subsystem.

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

