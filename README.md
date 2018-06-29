Python 2.6 in Docker
=====================

## What is this?

For those poor souls stuck on python 2.6, this allows Dockerizing your projects.

**Do not use if you are able to use python 2.7 or 3. Instead, [use one of these](https://hub.docker.com/_/python/)**

## Missing modules

A few things are unsupported. Here is the output of `setup.py` (called via `make`):

```
Failed to find the necessary bits to build these modules:
_bsddb             _tkinter           bsddb185
dl                 imageop            linuxaudiodev
ossaudiodev        sunaudiodev
To find the necessary bits, look in setup.py in detect_modules() for the module's name.


Failed to build these modules:
_curses            _curses_panel
```
