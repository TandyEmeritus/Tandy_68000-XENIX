# Tandy 68000/XENIX 3.4
_Yes, that's right, it's an upgrade disk for a new version of XENIX for Big Tandy computers!_  Read the included Tandy_68000_XENIX_3.4.3_Release_Notes.txt file for full information about what's included in this release.

Here is a short summary from the Release Notes:

<ins>New Kernel Features</ins>
- Brand new kernel supporting automatic detection of MMU size, with automatic adjusting of user memory to fit what the MMU can support.
- New crashbeep feature, which is settable using /etc/cfg.  The kernel will beep when halting for any reason.
- Automatic move of allocateable items (such as disk buffers) outside of MMU-addressable space, which maximizes memory for user processes.  This is applicable for systems with no MMU exension board and more than 1MB of memory, and for systems with a Tandy MMU exension board (or clone) and more than 4MB of memory.
- New Real Time Clock driver for both trs80gp (use the '-ee' option) and Tandy Emeritus' new DS1511 RTC board.  Allows autobooting with F1 (use 'autoboot -a' as root to enable) and having XENIX come up with the correct time set with no prompting.  In trs80gp, it allows use of Turbo and Haste modes without the XENIX clock speeding up.  You can just leave Turbo on!

<ins>New Utilities</ins>
- New RTC utility /etc/hwclock, which allows querying and setting of the RTC. Setting is not supported in trs80gp.
- New version of /etc/cfg to support all the latest kernel features in XENIX 3.4.
- Updated /bin/as (68000 assembler) with a bug fix for long assembly macros.
- New version of /etc/getty which displays both the system name and the terminal in the banner.
- New version of /etc/shutdown which supports being linked to /etc/reboot, and also now allows "-n" in front of the kernel-name argument.
- New /etc/reboot link to /etc/haltsys which reboots the system instead of halting.</li><li>New and updated help pages for all of the above.
