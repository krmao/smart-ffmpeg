# smart-ffmpeg
for learn ffmpeg

# build ios arm64/x86_64
> https://github.com/wang-bin/avbuild/wiki
```
cd build-script/avbuild
export FFSRC=../../build-source/ffmpeg-4.1.3
./avbuild.sh and "armv7 x86_64"
./avbuild.sh ios "x86_64"
./avbuild.sh ios "arm64 x86_64"
```

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