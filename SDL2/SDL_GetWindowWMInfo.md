====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_GetWindowWMInfo =

Get driver-specific information about a window.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_bool SDL_GetWindowWMInfo(SDL_Window * window,
                             SDL_SysWMinfo * info);
</syntaxhighlight>

== Function Parameters ==

{|
|'''window'''
|the window about which information is being requested
|-
|'''info'''
|an [[SDL_SysWMinfo]] structure filled in with window information
|}

== Return Value ==

Returns [[SDL_TRUE]] if the function is implemented and the
<code>version</code> member of the <code>info</code> struct is valid, or
[[SDL_FALSE]] if the information could not be retrieved; call
[[SDL_GetError]]() for more information.

== Remarks ==

You must include [[SDL_syswm]].h for the declaration of [[SDL_SysWMinfo]].

The caller must initialize the <code>info</code> structure's version by
using <code>[[SDL_VERSION]](&info.version)</code>, and then this function
will fill in the rest of the structure with information about the given
window.

== Version ==

This function is available since SDL 2.0.0.

----
[[CategoryAPI]]

