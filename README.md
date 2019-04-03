# CMakeCheckTypeSizeIOSTest
Testing CheckTypeSize CMake module while cross-compiling for iOS with CMake 3.14+

# HowTo

```
mkdir build;
cd build;
# Do this to use a toolchain file
cmake -DCMAKE_TOOLCHAIN_FILE=../cmake/toolchains/<toolchainFile> ..;
# Or this to cross-compile by setting command options
cmake -DCMAKE_SYSTEM_NAME=iOS \
    "-DCMAKE_OSX_ARCHITECTURES=arm64" \
    -DCMAKE_OSX_DEPLOYMENT_TARGET=9.3 \
    -DCMAKE_XCODE_ATTRIBUTE_ONLY_ACTIVE_ARCH=NO \
    -DCMAKE_IOS_INSTALL_COMBINED=YES ..;
```
