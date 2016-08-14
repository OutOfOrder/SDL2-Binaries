# SDL2 Binaries from OutOfOrder.cc

These are the pre-built SDL2 binaries that I, and several other game porters, use in all of our game ports.
These are kept up with the official release versions and sometimes include certain backported patches when needed for games.

## OS Targets

### Windows
Build via Visual Studio 2013
They run in Windows XP and newer, 32bit and 64bit.

### Mac OS X
Built via the Xcode project, dylib ONLY
Mac OS X 10.6 32bit and 64bit.

### Linux
Built via the configure script

Glib 2.4 or higher. (Basically any linux distribution in the past 6 years at least). 32bit and 64bit.

## CMake Support

Included is a CMake config script for use with find_package(SDL2 CONFIG).  Simply append the SDL2 path to the CMAKE_PREFIX_PATH
list(APPEND CMAKE_PREFIX_PATH  ../prebuilt/SDL2)
find_package(SDL2 CONFIG)

This will set the following variables
SDL2_INCLUDE_DIRS
SDL2_LIBRARIES

as well as a interface target of  SDL2 if you are using cmake 3.0+

## Other
The source code is included for what the binaries are build against. Any patches will be put in a patches folder
AND incorporated into the source tree
