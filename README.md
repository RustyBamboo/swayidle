# swayidle

This is sway's idle management daemon, swayidle. It is compatible with any
Wayland compositor which implements the KDE
[idle](https://github.com/swaywm/sway/blob/master/protocols/idle.xml) protocol.
See the man page, `swayidle(1)`, for instructions on configuring swayidle.

## Release Signatures

Releases are signed with [B22DA89A](http://pgp.mit.edu/pks/lookup?op=vindex&search=0x52CB6609B22DA89A)
and published [on GitHub](https://github.com/swaywm/sway/releases). swayidle
releases are managed independently of sway releases.

## Installation

### From Packages

Sway is available in many distributions. Try installing the "swayidle" package
for yours. If it's not available, check out [this wiki
page](https://github.com/swaywm/sway/wiki/Unsupported-packages) for information
on installation for your distributions.

If you're interested in packaging sway for your distribution, stop by the IRC
channel or shoot an email to sir@cmpwn.com for advice.

### Compiling from Source

Install dependencies:

* meson \*
* [wlroots](https://github.com/swaywm/wlroots)
* wayland
* wayland-protocols \*
* [scdoc](https://git.sr.ht/~sircmpwn/scdoc) (optional: man pages) \*
* git \*

_\*Compile-time dep_

Run these commands:

    meson build
    ninja -C build
    sudo ninja -C build install
