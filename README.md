# smart-ffmpeg
for learn ffmpeg

# build ios arm64/x86_64
> https://github.com/wang-bin/avbuild/wiki
```
cd build-script/avbuild
export FFSRC=../../build-source/ffmpeg-4.1.3
```
* build for android
    >./avbuild.sh and "armv7 x86_64"
* build for ios
    >./avbuild.sh ios "arm64 x86_64"
* build for macos 
    >./avbuild.sh macos10.14.4 "x86_64"   #macbookpro platform query by command in terminal $uname -a

# problems

### 1 nasm/yasm not found or too old. Use --disable-x86asm for a crippled build.
> yasm是x86架构下的一个汇编器, 默认开启

```
brew install yasm
```

### 2 WARNING: pkg-config not found, library detection may fail.

```
brew install pkg-config
```

### 3 WARNING: Building with deprecated library libavresample.