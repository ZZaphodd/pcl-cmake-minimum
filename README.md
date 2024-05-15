# pcl-cmake-minimum
Minimum example of compiling against PCL using CMake

https://learn.microsoft.com/en-us/vcpkg/get_started/get-started?pivots=shell-cmd
```ps1
$env:VCPKG_ROOT = "C:\bin\vcpkg"
$env:PATH = "$env:VCPKG_ROOT;$env:PATH"
rem create CMakePresets.json
cd cloud_viewer
cmake --preset=default
cmake --build build

.\build\Debug\cloud_viewer.exe
```

```.\vcpkg.exe list```
```
boost-algorithm:x64-windows                       1.84.0#1            Boost algorithm module
boost-align:x64-windows                           1.84.0#1            Boost align module
boost-any:x64-windows                             1.84.0#1            Boost any module
boost-array:x64-windows                           1.84.0#1            Boost array module
boost-asio:x64-windows                            1.84.0#1            Boost asio module
boost-assert:x64-windows                          1.84.0#1            Boost assert module
boost-atomic:x64-windows                          1.84.0#1            Boost atomic module
boost-bimap:x64-windows                           1.84.0#1            Boost bimap module
boost-bind:x64-windows                            1.84.0#1            Boost bind module
boost-chrono:x64-windows                          1.84.0#1            Boost chrono module
boost-circular-buffer:x64-windows                 1.84.0#1            Boost circular_buffer module
boost-cmake:x64-windows                           1.84.0              Boost cmake files
boost-concept-check:x64-windows                   1.84.0#1            Boost concept_check module
boost-config:x64-windows                          1.84.0#1            Boost config module
boost-container-hash:x64-windows                  1.84.0#1            Boost container_hash module
boost-container:x64-windows                       1.84.0#1            Boost container module
boost-context:x64-windows                         1.84.0#1            Boost context module
boost-conversion:x64-windows                      1.84.0#1            Boost conversion module
boost-core:x64-windows                            1.84.0#1            Boost core module
boost-coroutine:x64-windows                       1.84.0#1            Boost coroutine module
boost-date-time:x64-windows                       1.84.0#1            Boost date_time module
boost-describe:x64-windows                        1.84.0#1            Boost describe module
boost-detail:x64-windows                          1.84.0#1            Boost detail module
boost-dynamic-bitset:x64-windows                  1.84.0#1            Boost dynamic_bitset module
boost-endian:x64-windows                          1.84.0#1            Boost endian module
boost-exception:x64-windows                       1.84.0#1            Boost exception module
boost-filesystem:x64-windows                      1.84.0#1            Boost filesystem module
boost-foreach:x64-windows                         1.84.0#1            Boost foreach module
boost-function-types:x64-windows                  1.84.0#1            Boost function_types module
boost-function:x64-windows                        1.84.0#1            Boost function module
boost-functional:x64-windows                      1.84.0#1            Boost functional module
boost-fusion:x64-windows                          1.84.0#1            Boost fusion module
boost-graph:x64-windows                           1.84.0#1            Boost graph module
boost-headers:x64-windows                         1.84.0              Boost headers module
boost-integer:x64-windows                         1.84.0#1            Boost integer module
boost-interprocess:x64-windows                    1.84.0#1            Boost interprocess module
boost-intrusive:x64-windows                       1.84.0#1            Boost intrusive module
boost-io:x64-windows                              1.84.0#1            Boost io module
boost-iostreams:x64-windows                       1.84.0#1            Boost iostreams module
boost-iostreams[bzip2]:x64-windows                                    Support bzip2 filters
boost-iostreams[lzma]:x64-windows                                     Support LZMA/xz filters
boost-iostreams[zlib]:x64-windows                                     Support zlib filters
boost-iostreams[zstd]:x64-windows                                     Support zstd filters
boost-iterator:x64-windows                        1.84.0#1            Boost iterator module
boost-lambda:x64-windows                          1.84.0#1            Boost lambda module
boost-lexical-cast:x64-windows                    1.84.0#1            Boost lexical_cast module
boost-math:x64-windows                            1.84.0#1            Boost math module
boost-move:x64-windows                            1.84.0#1            Boost move module
boost-mp11:x64-windows                            1.84.0#1            Boost mp11 module
boost-mpl:x64-windows                             1.84.0#1            Boost mpl module
boost-multi-array:x64-windows                     1.84.0#1            Boost multi_array module
boost-multi-index:x64-windows                     1.84.0#1            Boost multi_index module
boost-numeric-conversion:x64-windows              1.84.0#1            Boost numeric_conversion module
boost-optional:x64-windows                        1.84.0#1            Boost optional module
boost-parameter:x64-windows                       1.84.0#1            Boost parameter module
boost-phoenix:x64-windows                         1.84.0#1            Boost phoenix module
boost-pool:x64-windows                            1.84.0#1            Boost pool module
boost-predef:x64-windows                          1.84.0#1            Boost predef module
boost-preprocessor:x64-windows                    1.84.0#1            Boost preprocessor module
boost-property-map:x64-windows                    1.84.0#1            Boost property_map module
boost-property-tree:x64-windows                   1.84.0#1            Boost property_tree module
boost-proto:x64-windows                           1.84.0#1            Boost proto module
boost-ptr-container:x64-windows                   1.84.0#1            Boost ptr_container module
boost-random:x64-windows                          1.84.0#1            Boost random module
boost-range:x64-windows                           1.84.0#1            Boost range module
boost-ratio:x64-windows                           1.84.0#1            Boost ratio module
boost-regex:x64-windows                           1.84.0#1            Boost regex module
boost-serialization:x64-windows                   1.84.0#1            Boost serialization module
boost-signals2:x64-windows                        1.84.0#1            Boost signals2 module
boost-smart-ptr:x64-windows                       1.84.0#1            Boost smart_ptr module
boost-sort:x64-windows                            1.84.0#1            Boost sort module
boost-spirit:x64-windows                          1.84.0#1            Boost spirit module
boost-static-assert:x64-windows                   1.84.0#1            Boost static_assert module
boost-system:x64-windows                          1.84.0#1            Boost system module
boost-thread:x64-windows                          1.84.0#1            Boost thread module
boost-throw-exception:x64-windows                 1.84.0#1            Boost throw_exception module
boost-tokenizer:x64-windows                       1.84.0#1            Boost tokenizer module
boost-tti:x64-windows                             1.84.0#1            Boost tti module
boost-tuple:x64-windows                           1.84.0#1            Boost tuple module
boost-type-index:x64-windows                      1.84.0#1            Boost type_index module
boost-type-traits:x64-windows                     1.84.0#1            Boost type_traits module
boost-typeof:x64-windows                          1.84.0#1            Boost typeof module
boost-uninstall:x64-windows                       1.84.0#1            Internal vcpkg port used to uninstall Boost
boost-unordered:x64-windows                       1.84.0#1            Boost unordered module
boost-utility:x64-windows                         1.84.0#1            Boost utility module
boost-uuid:x64-windows                            1.84.0#1            Boost uuid module
boost-variant2:x64-windows                        1.84.0#1            Boost variant2 module
boost-variant:x64-windows                         1.84.0#1            Boost variant module
boost-winapi:x64-windows                          1.84.0#1            Boost winapi module
boost-xpressive:x64-windows                       1.84.0#1            Boost xpressive module
brotli:x64-windows                                1.1.0#1             a generic-purpose lossless compression algorithm...
bzip2:x64-windows                                 1.0.8#5             bzip2 is a freely available, patent free, high-q...
bzip2[tool]:x64-windows                                               Builds bzip2 executable
cereal:x64-windows                                1.3.2#1             a header-only C++11 serialization library (built...
cgns:x64-windows                                  4.4.0               The CFD General Notation System (CGNS) provides ...
cgns[hdf5]:x64-windows                                                Enable hdf5 support
cgns[lfs]:x64-windows                                                 Enable LFS support
cgns[lfsselector]:x64-windows                                         Selector for LFS
curl:x64-windows                                  8.7.1#3             A library for transferring data with URLs
curl[non-http]:x64-windows                                            Enables protocols beyond HTTP/HTTPS/HTTP2
curl[schannel]:x64-windows                                            SSL support (Secure Channel)
curl[ssl]:x64-windows                                                 Default SSL backend
curl[sspi]:x64-windows                                                SSPI support
double-conversion:x64-windows                     3.3.0               Efficient binary-decimal and decimal-binary conv...
egl-registry:x64-windows                          2024-01-25          EGL API and Extension Registry
eigen3:x64-windows                                3.4.0#4             C++ template library for linear algebra: matrice...
expat:x64-windows                                 2.6.2               XML parser library written in C
exprtk:x64-windows                                2022-01-01#2        Simple to use, easy to integrate and extremely e...
fast-float:x64-windows                            6.1.1               Fast and exact implementation of the C++ from_ch...
flann:x64-windows                                 2019-04-07#7        Fast Library for Approximate Nearest Neighbors
fmt:x64-windows                                   10.2.1#2            {fmt} is an open-source formatting library provi...
freetype:x64-windows                              2.13.2#1            A library to render fonts.
freetype[brotli]:x64-windows                                          Support decompression of WOFF2 streams
freetype[bzip2]:x64-windows                                           Support bzip2 compressed fonts.
freetype[png]:x64-windows                                             Support PNG compressed OpenType embedded bitmaps.
freetype[zlib]:x64-windows                                            Use zlib instead of internal library for DEFLATE
gklib:x64-windows                                 2023-03-27          General helper libraries for KarypisLab.
glew:x64-windows                                  2.2.0#3             The OpenGL Extension Wrangler Library (GLEW) is ...
hdf5:x64-windows                                  1.14.2              HDF5 is a data model, library, and file format f...
hdf5[szip]:x64-windows                                                Build with szip
hdf5[tools]:x64-windows                                               Build hdf tools
hdf5[zlib]:x64-windows                                                Build with zlib
jsoncpp:x64-windows                               1.9.5#4             JsonCpp is a C++ library that allows manipulatin...
libharu:x64-windows                               2.4.4#1             libharu - free PDF library
libiconv:x64-windows                              1.17#3              GNU Unicode text conversion
libjpeg-turbo:x64-windows                         3.0.2               libjpeg-turbo is a JPEG image codec that uses SI...
liblzma:x64-windows                               5.4.4               Compression library with an API similar to that ...
libogg:x64-windows                                1.3.5#1             Ogg is a multimedia container format, and the na...
libpng:x64-windows                                1.6.43#1            libpng is a library implementing an interface fo...
libtheora:x64-windows                             1.2.0alpha1-2...    Theora is a free and open video compression form...
libxml2:x64-windows                               2.11.7              Libxml2 is the XML C parser and toolkit develope...
libxml2[iconv]:x64-windows                                            Add ICONV support
libxml2[lzma]:x64-windows                                             Use LZMA
libxml2[zlib]:x64-windows                                             Use ZLib
lz4:x64-windows                                   1.9.4#1             Lossless compression algorithm, providing compre...
matio:x64-windows                                 1.5.26              MATLAB MAT File I/O Library
matio[hdf5]:x64-windows                                               Check for HDF5 library
matio[zlib]:x64-windows                                               Check for zlib library
metis:x64-windows                                 2022-07-27          Serial Graph Partitioning and Fill-reducing Matr...
netcdf-c:x64-windows                              4.8.1#5             A set of self-describing, machine-independent da...
netcdf-c[dap]:x64-windows                                             Build with DAP remote access client support
netcdf-c[hdf5]:x64-windows                                            Build with HDF5 support
netcdf-c[nczarr]:x64-windows                                          Build with NCZarr cloud storage access support
netcdf-c[netcdf-4]:x64-windows                                        Build with netCDF-4 support
nlohmann-json:x64-windows                         3.11.3              JSON for Modern C++
opengl-registry:x64-windows                       2024-02-10#1        OpenGL, OpenGL ES, and OpenGL ES-SC API and Exte...
opengl:x64-windows                                2022-12-04#3        Open Graphics Library (OpenGL)[3][4][5] is a cro...
pcl:x64-windows                                   1.14.1              Point Cloud Library (PCL) is open source library...
pcl[visualization]:x64-windows                                        Build visualization
pcl[vtk]:x64-windows                                                  An alias for visualization
pegtl:x64-windows                                 3.2.7               The Parsing Expression Grammar Template Library ...
pkgconf:x64-windows                               2.2.0               pkgconf is a program which helps to configure co...
proj:x64-windows                                  9.4.0               PROJ library for cartographic projections
proj[net]:x64-windows                                                 Enable network support
proj[tiff]:x64-windows                                                Enable TIFF support to read some grids
pugixml:x64-windows                               1.14                Light-weight, simple and fast XML parser for C++...
qhull:x64-windows                                 8.0.2#5             computes the convex hull, Delaunay triangulation...
seacas:x64-windows                                2022-11-22#5        The Sandia Engineering Analysis Code Access Syst...
sqlite3:x64-windows                               3.45.3              SQLite is a software library that implements a s...
sqlite3[json1]:x64-windows                                            Enable JSON functionality for sqlite3
sqlite3[tool]:x64-windows                                             Build sqlite3 executable
szip:x64-windows                                  2.1.1#12            Szip compression software, providing lossless co...
tiff:x64-windows                                  4.6.0#4             A library that supports the manipulation of TIFF...
tiff[jpeg]:x64-windows                                                Support JPEG compression in TIFF image files
tiff[lzma]:x64-windows                                                Support LZMA compression in TIFF image files
tiff[zip]:x64-windows                                                 Support ZIP/deflate compression in TIFF image files
utfcpp:x64-windows                                4.0.5               UTF-8 with C++ in a Portable Way
vcpkg-boost:x64-windows                           2024-04-25
vcpkg-cmake-config:x64-windows                    2022-02-06#1
vcpkg-cmake:x64-windows                           2024-04-18
vcpkg-pkgconfig-get-modules:x64-windows           2024-04-03
vcpkg-tool-meson:x64-windows                      1.3.2#2             Meson build system
verdict:x64-windows                               1.4.0               Compute quality functions of 2 and 3-dimensional...
vtk:x64-windows                                   9.3.0-pv5.12.0#2    Software system for 3D computer graphics, image ...
vtk[opengl]:x64-windows                                               All opengl related modules
zlib:x64-windows                                  1.3.1               A compression library
zstd:x64-windows                                  1.5.6               Zstandard - Fast real-time compression algorithm
```