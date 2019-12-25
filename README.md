This project is a sample to show how to manage a library "virtual environment" for C++ and CMake using VcPkg.

To prepare environment using VcPkg:

```
vcpkg install range-v3 --vcpkg-root ./vcpkg --triplet x64-linux-hoge
```

To configure this project:

```
cmake -DCMAKE_TOOLCHAIN_FILE=./vcpkg/scripts/buildsystems/vcpkg.cmake -DVCPKG_TARGET_TRIPLET=x64-linux-hoge .
```

# LICENSE

All contents under directory `./vcpkg/` are from VcPkg's source code and are under Microsoft's copyright licensed under MIT. The rest of the content is under public domain.