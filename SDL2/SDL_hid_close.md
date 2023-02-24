====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_hid_close =

Close a HID device.

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_hid_close(SDL_hid_device *dev);
</syntaxhighlight>

== Function Parameters ==

{|
|'''dev'''
|A device handle returned from [[SDL_hid_open]]().
|}

== Version ==

This function is available since SDL 2.0.18.

----
[[CategoryAPI]]

