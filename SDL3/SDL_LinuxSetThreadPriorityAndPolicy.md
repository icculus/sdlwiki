====== (This is the documentation for SDL3, which is under heavy development and the API is changing! [https://wiki.libsdl.org/SDL2/ SDL2] is the current stable version!) ======
= SDL_LinuxSetThreadPriorityAndPolicy =

Sets the priority (not nice level) and scheduling policy for a thread.

== Syntax ==

<syntaxhighlight lang='c'>
int SDL_LinuxSetThreadPriorityAndPolicy(Sint64 threadID, int sdlPriority, int schedPolicy);
</syntaxhighlight>

== Function Parameters ==

{|
|'''threadID'''
|The Unix thread ID to change priority of.
|-
|'''sdlPriority'''
|The new [[SDL_ThreadPriority]] value.
|-
|'''schedPolicy'''
|The new scheduling policy (SCHED_FIFO, SCHED_RR, SCHED_OTHER, etc...)
|}

== Return Value ==

Returns 0 on success, or -1 on error.

== Remarks ==

This uses setpriority() if possible, and RealtimeKit if available.

== Version ==

This function is available since SDL 3.0.0.

----
[[CategoryAPI]], [[CategoryLinux]]

