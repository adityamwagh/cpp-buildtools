# Introduction to C++ Buildsystem for Beginners

These set of notes explains the basics of using Makefile, CMake etc to beginners.
This tutorial is based upon [this](https://www.youtube.com/playlist?list=PLalVdRk2RC6o5GHu618ARWh0VO0bFlif4) playlist. Thanks to the creator for making these!

## Basics

### Makefile

- Must use tabs to indent the files.

### CMake

- Must create a file called CMakeLists.txt
- Need to tell CMake where `src` folder and `build` folder is. Try not to make the `build` folder where `src` is. There is no standard for this.
- Need to provide a path to the build folder. Most people make a `build` folder and pass it to `cmake`.
CMake usage

```txt
Usage

  cmake [options] <path-to-source>
  cmake [options] <path-to-existing-build>
  cmake [options] -S <path-to-source> -B <path-to-build>

Specify a source directory to (re-)generate a build system for it in the
current working directory.  Specify an existing build directory to
re-generate its build system.

Run 'cmake --help' for more information.
```
-   `cmake [options] -S <path-to-source> -B <path-to-build>` makes some files in build folder. **DO NOT TOUCH THOSE FILES**