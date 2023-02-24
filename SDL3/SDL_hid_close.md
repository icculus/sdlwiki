====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
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

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

