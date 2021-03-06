# Computer graphics in Game development course

This repo contains a template for Computer graphics in Game development labs (summer 2022)

## Pre-requirements

- Version control: [Git](https://git-scm.com/)
- C++ compiler: **MSVS**, Clang, GCC
- Build automation: [CMake](https://cmake.org/download/)
- C++ IDE: [Visual Studio Community](https://visualstudio.microsoft.com/downloads/), [CLion](https://www.jetbrains.com/clion/)
- DirectX related: [Windows SDK](https://developer.microsoft.com/en-us/windows/downloads/windows-sdk/)

## How to build the solution

Use `git clone --recursive` to clone the repo with submodules or run `git submodule update --init --recursive` after the first clone.

Go to the project folder and run the next command:

```sh
mkdir build
cmake --build build --config Debug --target Rasterization
```

## Running

Raytracing:
```sh
.\build\Release\Raytracing.exe --model_path models/CornellBox-Original.obj --camera_position 0.0,1.0,2.0 --accumulation_num 16 --raytracing_depth 3
```

DirectX12:
```sh
.\build\Release\DirectX12.exe
```

## Third-party tools and data

- [STB](https://github.com/nothings/stb) by Sean Barrett (Public Domain)
- [Linalg.h](https://github.com/sgorsten/linalg) by Sterling Orsten (The Unlicense)
- [Tinyobjloader](https://github.com/syoyo/tinyobjloader) by Syoyo Fujita (MIT License)
- [Cxxopts](https://github.com/jarro2783/cxxopts) by jarro2783 (MIT License)
- [Cornell Box models](https://casual-effects.com/g3d/data10/index.html#) by Morgan McGuire (CC BY 3.0 License)
- [Cube model](https://casual-effects.com/g3d/data10/index.html#) by Morgan McGuire (CC BY 3.0 License)
- [Dabrovic Sponza](https://casual-effects.com/g3d/data10/index.html#) by Marko Dabrovic (CC BY-NC)
