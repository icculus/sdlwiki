====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_hid_get_serial_number_string =

Get The Serial Number String from a HID device.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_hid_get_serial_number_string(SDL_hid_device *dev, wchar_t *string, size_t maxlen);
</syntaxhighlight>

== Function Parameters ==

{|
|'''dev'''
|A device handle returned from [[SDL_hid_open]]().
|-
|'''string'''
|A wide string buffer to put the data into.
|-
|'''maxlen'''
|The length of the buffer in multiples of wchar_t.
|}

== Return Value ==

Returns 0 on success and -1 on error.

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

