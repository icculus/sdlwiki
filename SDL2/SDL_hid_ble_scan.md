====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_hid_ble_scan =

Start or stop a BLE scan on iOS and tvOS to pair Steam Controllers 

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_hid_ble_scan(SDL_bool active);
</syntaxhighlight>

== Function Parameters ==

{|
|'''active'''
|[[SDL_TRUE]] to start the scan, [[SDL_FALSE]] to stop the scan
|}

== Version ==

This function is available since SDL 2.0.18.

----
[[CategoryAPI]]

