# ScummVM Steam Link Port

This is a mostly non-functional port of ScummVM to the Steam Link. Controller sort of works with the default analog-stick-as-mouse support
built into ScummVM, but the Steam Controller isn't working as it should with the haptic pad as the mouse instead which would be quite nice.

## Building

You need the Steam Link SDK in order to build this. Clone https://github.com/ValveSoftware/steamlink-sdk (it's over 3GB and takes a while!)
and run `source setenv.sh` while in the SDK root directory. Then enter the ScummVM source tree and run `./build_steamlink.sh`.

## Changes

I'm a noob so there are no actual code changes here, just a `steamlink` host assigned in `configure`. Fine tuning the correct options here
may or may not be necessary for better performance (but it already performs pretty well as it is).

## Credits and whatever else

GPLv2 as per original ScummVM, but there aren't likely to be any future changes to this repo so I don't consider it a real 'fork' anyway.

Big thanks to GranPC for pointing me in the right direction and answering my pathetic questions about SDKs even work.

