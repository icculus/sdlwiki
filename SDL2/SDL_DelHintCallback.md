====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_DelHintCallback =

Remove a function watching a particular hint.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_DelHintCallback(const char *name,
                         SDL_HintCallback callback,
                         void *userdata);
</syntaxhighlight>

== Function Parameters ==

{|
|'''name'''
|the hint being watched
|-
|'''callback'''
|An [[SDL_HintCallback]] function that will be called when the hint value changes
|-
|'''userdata'''
|a pointer being passed to the callback function
|}

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_AddHintCallback]]

----
[[CategoryAPI]]

