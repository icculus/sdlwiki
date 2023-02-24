====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_hid_get_feature_report =

Get a feature report from a HID device.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_hid_get_feature_report(SDL_hid_device *dev, unsigned char *data, size_t length);
</syntaxhighlight>

== Function Parameters ==

{|
|'''dev'''
|A device handle returned from [[SDL_hid_open]]().
|-
|'''data'''
|A buffer to put the read data into, including the Report ID. Set the first byte of <code>data</code> to the Report ID of the report to be read, or set it to zero if your device does not use numbered reports.
|-
|'''length'''
|The number of bytes to read, including an extra byte for the report ID. The buffer can be longer than the actual report.
|}

== Return Value ==

Returns the number of bytes read plus one for the report ID (which is still
in the first byte), or -1 on error.

== Remarks ==

Set the first byte of <code>data</code> to the Report ID of the report to
be read. Make sure to allow space for this extra byte in <code>data</code>.
Upon return, the first byte will still contain the Report ID, and the
report data will start in data[1].

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]]

