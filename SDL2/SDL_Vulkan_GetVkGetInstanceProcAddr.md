====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_Vulkan_GetVkGetInstanceProcAddr =

Get the address of the <code>vkGetInstanceProcAddr</code> function.

== Syntax ==

<syntaxhighlight lang='c'>
void* SDL_Vulkan_GetVkGetInstanceProcAddr(void);
</syntaxhighlight>

== Return Value ==

Returns the function pointer for <code>vkGetInstanceProcAddr</code> or NULL
on error.

== Remarks ==

This should be called after either calling [[SDL_Vulkan_LoadLibrary]]() or
creating an [[SDL_Window]] with the <code>[[SDL_WINDOW_VULKAN]]</code>
flag.

== Version ==

This function is available since SDL 2.0.6.

----
[[CategoryAPI]]

