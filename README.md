start-stop-daemon
=================

Installation:
=============

Extract the source file to some location and execute the following:

```
  gcc start-stop-daemon.c -o start-stop-daemon
  sudo mv start-stop-daemon /usr/sbin/start-stop-daemon
```

Example Usage:
========
Please see `example_service`

Notes:
======
The source code was extracted from:
  http://www.hpcf.upr.edu/web/sites/default/files/start-stop-daemon.c


```
A rewrite of the original Debian's start-stop-daemon Perl script
in C (faster - it is executed many times during system startup).

Written by Marek Michalkiewicz <marekm@i17linuxb.ists.pwr.wroc.pl>,
public domain.  Based conceptually on start-stop-daemon.pl, by Ian
Jackson <ijackson@gnu.ai.mit.edu>.  May be used and distributed
freely for any purpose.  Changes by Christian Schwarz
<schwarz@monet.m.isar.de>, to make output conform to the Debian
Console Message Standard, also placed in public domain.  Minor
changes by Klee Dienes <klee@debian.org>, also placed in the Public
Domain.

Changes by Ben Collins <bcollins@debian.org>, added --chuid, --background
and --make-pidfile options, placed in public domain aswell.

Port to OpenBSD by Sontri Tomo Huynh <huynh.29@osu.edu>
               and Andreas Schuldei <andreas@schuldei.org>
Changes by Ian Jackson: added --retry (and associated rearrangements).

Modified for Gentoo rc-scripts by Donny Davies <woodchip@gentoo.org>:
 I removed the BSD/Hurd/OtherOS stuff, added #include <stddef.h>
 and stuck in a #define VERSION "1.9.18".  Now it compiles without
 the whole automake/config.h dance.
```
