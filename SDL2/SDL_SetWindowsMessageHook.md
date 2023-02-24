====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_SetWindowsMessageHook =

Set a callback for every Windows message, run before TranslateMessage().

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_SetWindowsMessageHook(SDL_WindowsMessageHook callback, void *userdata);
</syntaxhighlight>

== Function Parameters ==

{|
|'''callback'''
|The [[SDL_WindowsMessageHook]] function to call.
|-
|'''userdata'''
|a pointer to pass to every iteration of <code>callback</code>
|}

== Version ==

This function is available since SDL 2.0.4.

----
[[CategoryAPI]]

