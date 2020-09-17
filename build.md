## 迁移说明

将PMS算法编译成动态库，测试程序编译成可执行程序，运行时动态链接。

## 编译 
```
mkdir build
cd build
cmake ..
make
```

## 运行
```
build/demo/demo Data/Cone/im2.png Data/Cone/im6.png 0 64
```
