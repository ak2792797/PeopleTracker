# PeopleTracker
==============================

People Detection and Tracking based on DPM &amp; KCF.
# Build
## Dependencies
* C++11
* OpenCV 3.1.0 with contrib
* CMake

Compilation has been tested on OS X 10.11.4 with Apple LLVM version 7.3.0 (clang-703.0.29).

### Windows
I don't know.

### OS X & Linux
* Install OpenCV 3.1 with contrib and CMake.
* Configure and complie:

`mkdir build`<br />
`cd build`<br />
`cmake ..`<br />
`make -j4`<br />

# Usage
Make sure your Camera working on /dev/video0 
then run `./PeopleDetect`

# Thanks
[Gump-II](https://github.com/Gump-II) 's [UAV-Detect](https://github.com/Gump-II/UAV-Detect) respository inspire me.