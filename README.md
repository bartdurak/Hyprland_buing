# Hyprland_buing
I installed Hyprland on Kali linux. However, I cannot start the environment.  Below is the log file
--------------------------------------------
   Hyprland Crash Report
--------------------------------------------
Oops

Hyprland received signal 6(ABRT)
Version: 918d8340afd652b011b937d29d5eea0be08467f5
Tag: v0.41.2

System info:
	System name: Linux
	Node name: ka
	Release: 6.6.15-amd64
	Version: #1 SMP PREEMPT_DYNAMIC Kali 6.6.15-2kali1 (2024-05-17)

GPU:
	2d:00.0 VGA compatible controller [0300]: NVIDIA Corporation GA104 [GeForce RTX 3060] [10de:2487] (rev a1) (prog-if 00 [VGA controller])


os-release:
	PRETTY_NAME="Kali GNU/Linux Rolling"
	NAME="Kali GNU/Linux"
	VERSION_ID="2024.2"
	VERSION="2024.2"
	VERSION_CODENAME=kali-rolling
	ID=kali
	ID_LIKE=debian
	HOME_URL="https://www.kali.org/"
	SUPPORT_URL="https://forums.kali.org/"
	BUG_REPORT_URL="https://bugs.kali.org/"
	ANSI_COLOR="1;31"
Backtrace:
	# | hyprland(_Z12getBacktracev+0x5f) [0x55bb676f6fef]
		getBacktrace()
		??:?
	#1 | hyprland(_ZN13CrashReporter18createAndSaveCrashEi+0x965) [0x55bb67661115]
		CrashReporter::createAndSaveCrash(int)
		??:?
	#2 | hyprland(_Z25handleUnrecoverableSignali+0x60) [0x55bb675d7c80]
		handleUnrecoverableSignal(int)
		??:?
	#3 | /lib/x86_64-linux-gnu/libc.so.6(+0x3d580) [0x7fc3e0a2b580]
		??
		??:0
	#4 | /lib/x86_64-linux-gnu/libc.so.6(+0x8bb1c) [0x7fc3e0a79b1c]
		??
		??:0
	#5 | /lib/x86_64-linux-gnu/libc.so.6(raise+0x12) [0x7fc3e0a2b4e2]
		??
		??:0
	#6 | /lib/x86_64-linux-gnu/libc.so.6(abort+0xd3) [0x7fc3e0a144ed]
		??
		??:0
	#7 | /lib/x86_64-linux-gnu/libstdc++.so.6(+0xa0a3d) [0x7fc3e0ca0a3d]
		??
		??:0
	#8 | /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb1f4a) [0x7fc3e0cb1f4a]
		??
		??:0
	#9 | /lib/x86_64-linux-gnu/libstdc++.so.6(_ZSt10unexpectedv+0) [0x7fc3e0ca05e9]
		??
		??:0
	#1 | /lib/x86_64-linux-gnu/libstdc++.so.6(+0xb21c8) [0x7fc3e0cb21c8]
		??
		??:0
	#11 | hyprland(+0x16b669) [0x55bb6753c669]
		std::__throw_bad_optional_access()
		??:?
	#12 | hyprland(_ZN11CCompositor10initServerEv+0x4bb) [0x55bb675eb93b]
		CCompositor::initServer()
		??:?
	#13 | hyprland(main+0xa3d) [0x55bb6759aafd]
		main
		??:?
	#14 | /lib/x86_64-linux-gnu/libc.so.6(+0x27c8a) [0x7fc3e0a15c8a]
		??
		??:0
	#15 | /lib/x86_64-linux-gnu/libc.so.6(__libc_start_main+0x85) [0x7fc3e0a15d45]
		??
		??:0
	#16 | hyprland(_start+0x21) [0x55bb675d7af1]
		_start
		??:?


Log tail:
[LOG] Runtime directory: /run/user/1000/hypr/918d8340afd652b011b937d29d5eea0be08467f5_1724576829_1239957684
[LOG] Hyprland PID: 41935
[LOG] ===== SYSTEM INFO: =====
[LOG] System name: Linux
[LOG] Node name: ka
