cmake_minimum_required(VERSION 2.4)
project(scutclient C)
ADD_DEFINITIONS(-Os -Wall)
add_executable(scutclient src/auth.c src/drcom.c src/functions.c src/info.c src/main.c src/md5.c src/tracelog.c)
install(TARGETS scutclient RUNTIME DESTINATION bin)
set(CMAKE_C_COMPILER "/home/qiaoziming/downloads/openwrt/staging_dir/toolchain-aarch64_cortex-a53_gcc-8.4.0_musl/bin/aarch64-openwrt-linux-musl-gcc")
set(CMAKE_CXX_COMPILER "/home/qiaoziming/downloads/openwrt/staging_dir/toolchain-aarch64_cortex-a53_gcc-8.4.0_musl/bin/aarch64-openwrt-linux-musl-g++")
