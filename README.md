# PeopleTracker

People Detection and Tracking for Respberry Pi 3，based on DPM &amp; KCF. ( OMG, only 2.0 fps when DPM, 9.0 fps when KCF on Respberry Pi 3 Single Thread mode. )
# Build
### Dependencies
* C++11
* OpenCV 3.1.0 with contrib
* CMake

Compilation has been tested on 

* OS X 10.11.4 with Apple LLVM version 7.3.0 (clang-703.0.29).
* Raspbian 4.9.2-10 with GCC 4.9.2

### Windows
* Install OpenCV 3.1 with contrib and CMake.
* Set environment variables according to [OpenCV Setup - Environment Variables](http://docs.opencv.org/doc/tutorials/introduction/windows_install/windows_install.html#windowssetpathandenviromentvariable)
* Launch cmake-gui, create a build folder and configure.
* Open PeopleTracker.sln in Visual Studio and compile the projects PeopleTracker.

### OS X & Linux
* Install OpenCV 3.1 with contrib and CMake.
* Configure and complie:
	
 1) ``` mkdir build ```
	
 2) ``` cd build ```
	
 3) ``` cmake .. ```
	
 4) ``` make -j4 ```

# Usage
Make sure your Camera working on /dev/video0 
then run `./PeopleTracker`

# Special thanks to:
[Gump-II](https://github.com/Gump-II) His [UAV-Detect](https://github.com/Gump-II/UAV-Detect) respository inspire me.