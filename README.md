#openal-soft

OpenAL Soft official fork(keep sync with https://github.com/kcat/openal-soft.git).

## Standalone Toolchain

Make standalone android ndk toolchain($NDK/docs/STANDALONE-TOOLCHAIN.html):
$cd $NDK_ROOT
$./build/tools/make-standalone-toolchain.sh --platform=android-14 --install-dir=/home/Administrator/toolchains/arm-linux-androideabi-r9d-14
$export PATH=$PATH:/home/Administrator/toolchains/arm-linux-androideabi-r9d-14/bin

## Build
Ensure you have installed cmake(2.6 or higher), and make standalone android ndk toolchain($NDK/docs/STANDALONE-TOOLCHAIN.html), build steps:
- $cd build
- $cmake -D CMAKE_TOOLCHAIN_FILE=../cmake/android.toolchain.cmake -G "Unix Makefiles" ..
- $make -j4

Enjoy it!!!
