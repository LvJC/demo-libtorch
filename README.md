# cpp-libtorch
Pytorch (libTorch) C++ Domo

## 1. Download libTorch
First, you need to download libTorch package to support C++ development. For example, libtorch for CUDA9.0 can download use this:
https://download.pytorch.org/libtorch/nightly/cu90/libtorch-shared-with-deps-latest.zip

After download this zip file, you need to unzip it here in your reposity 'cpp-libtorch/'.

Now the resposity should be like this:
```
cpp-libtorch
    |libtorch
        |build-version
        |include
        |lib
        |share
    |CMakeLists.txt
    |example-app.cpp
    |model.pt
    |MyModule.py
    |LICENSE
    |README.md
```

## 2. Cmake
Second, cmake & build & make.
```
mkdir build
cd build
cmake .. -DCMAKE_PREFIX_PATH=../libtorch
make
```

## 3. Run example-app
Third, you can run the example-app after make.
```
./example-app ../model.pt
```
