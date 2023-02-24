====== (This is the legacy documentation for stable SDL2, the current stable version; [https://wiki.libsdl.org/SDL3/ SDL3] is the current development version.) ======
= SDL_AndroidSendMessage =

Send a user command to SDLActivity.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_AndroidSendMessage(Uint32 command, int param);
</syntaxhighlight>

== Function Parameters ==

{|
|'''command'''
|user command that must be greater or equal to 0x8000
|-
|'''param'''
|user parameter
|}

== Remarks ==

Override "boolean onUnhandledMessage(Message msg)" to handle the message.

== Version ==

This function is available since SDL 2.0.22.

----
[[CategoryAPI]]

