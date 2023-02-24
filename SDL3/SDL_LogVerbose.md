====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_LogVerbose =

Log a message with [[SDL_LOG_PRIORITY_VERBOSE]].

== Syntax ==

<syntaxhighlight lang='c'>
void SDL_LogVerbose(int category, SDL_PRINTF_FORMAT_STRING const char *fmt, ...) SDL_PRINTF_VARARG_FUNC(2);
</syntaxhighlight>

== Function Parameters ==

{|
|'''category'''
|the category of the message
|-
|'''fmt'''
|a printf() style message format string
|-
|'''...'''
|additional parameters matching % tokens in the '''fmt''' string, if any
|}

== Version ==

This function is available since SDL 3.0.0.

== Related Functions ==

:[[SDL_Log]]
:[[SDL_LogCritical]]
:[[SDL_LogDebug]]
:[[SDL_LogError]]
:[[SDL_LogInfo]]
:[[SDL_LogMessage]]
:[[SDL_LogMessageV]]
:[[SDL_LogWarn]]

----
[[CategoryAPI]], [[CategoryLog]]

