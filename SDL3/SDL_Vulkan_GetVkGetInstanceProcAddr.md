====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_Vulkan_GetVkGetInstanceProcAddr =

Get the address of the <code>vkGetInstanceProcAddr</code> function.

== Syntax ==

<syntaxhighlight lang='c'>
SDL_FunctionPointer SDL_Vulkan_GetVkGetInstanceProcAddr(void);
</syntaxhighlight>

== Return Value ==

Returns the function pointer for <code>vkGetInstanceProcAddr</code> or NULL
on error.

== Remarks ==

This should be called after either calling [[SDL_Vulkan_LoadLibrary]]() or
creating an [[SDL_Window]] with the <code>[[SDL_WINDOW_VULKAN]]</code>
flag.

The actual type of the returned function pointer is
PFN_vkGetInstanceProcAddr, but that isn't available because the Vulkan
headers are not included here. You should cast the return value of this
function to that type, e.g.

<code>vkGetInstanceProcAddr =
(PFN_vkGetInstanceProcAddr)[[SDL_Vulkan_GetVkGetInstanceProcAddr]]();</code>

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

