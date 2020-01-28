# pcl-cmake-minimum
Minimum example of compiling against PCL using CMake

https://learn.microsoft.com/en-us/vcpkg/get_started/get-started?pivots=shell-cmd
```bat
set VCPKG_ROOT=c:\bin\vcpkg
set PATH=%VCPKG_ROOT%;%PATH%
rem create CMakePresets.json
cmake --preset=default
cmake --build build
```