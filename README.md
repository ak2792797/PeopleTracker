# PeopleTracker

People Detection and Tracking for Respberry Pi 3，based on DPM &amp; KCF. 
# Build
### Dependencies
* C++11
* OpenCV 3.1.0 with contrib
* CMake

Compilation has been tested on OS X 10.11.4 with Apple LLVM version 7.3.0 (clang-703.0.29).

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

TO-DO
=============
- [x] ~~DPM & KCF 融合 ( 2016/04/11 )~~
- [ ] 输出 1080p 或 720p 视频（ 现在是 320*240 ）
- [ ] 程序 & 算法 优化
  - [ ] 优化跟丢检测逻辑
  - [ ] 目标出入时的检测
  - [ ] 优化程序运行速度
- [ ] 自动云台控制
  - [ ] 蓝牙通信
  - [ ] 命令收发
- [ ] 程序 & 算法 并行化
- [ ] 多目标跟踪（目前是多目标识别，单目标跟踪）
- [ ] 视频服务器搭建，向其他设备输出视频。

# Special thanks to:
[Gump-II](https://github.com/Gump-II) His [UAV-Detect](https://github.com/Gump-II/UAV-Detect) respository inspire me.