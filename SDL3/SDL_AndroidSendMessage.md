====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
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

This function is available since SDL 3.0.0.

----
[[CategoryAPI]], [[CategoryAndroid]]

