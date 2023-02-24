====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_WasInit =

Get a mask of the specified subsystems which are currently initialized.

== Syntax ==

<syntaxhighlight lang='c'>
Uint32 SDL_WasInit(Uint32 flags);
</syntaxhighlight>

== Function Parameters ==

{|
|'''flags'''
|any of the flags used by [[SDL_Init]](); see [[SDL_Init]] for details.
|}

== Return Value ==

Returns a mask of all initialized subsystems if <code>flags</code> is 0,
otherwise it returns the initialization status of the specified subsystems.

The return value does not include [[SDL_INIT_NOPARACHUTE]].

== Version ==

This function is available since SDL 2.0.0.

== Related Functions ==

:[[SDL_Init]]
:[[SDL_InitSubSystem]]

----
[[CategoryAPI]]

