# 简单场景的显示与漫游实验报告

## 1. 场景构建
本次实验中，我构建了一个天空盒场景，在天空盒场景内有一个由1178个立方体构成的大型空心立方体，在空心立方体中有一个可以自由移动的小立方体。

## 2. 运行与交互
在 `./exe` 目录下双击 `EasyScene.exe` 可执行文件即可运行。

+ 移动鼠标或用键盘的 `W, S, A, D` 键可以自由移动摄像头，穿过立方体墙面可以观察到外部的天空盒。
+ 按空格键会赋予中心的小立方体一个随机速度，小立方体触碰到墙面后进行 `AABB碰撞检测` 并反弹。
+ 按 `I` 键可以切换为**反相**滤镜，按 `G` 键可以切换为**灰度**滤镜。
+ 按 `ESC` 键退出程序

## 3. 编译
在 `./src` 目录下可以看到代码源文件，其中：

+ `./src/include` 为 `OpenGL` 包含目录
+ `./src/lib` 为 `OpenGL` 库目录
+ `./src/resource` 为天空盒贴图和立方体纹理

各类文件的引用已经通过 `Visual Studio` 设置完成，通过 `Visual Studio` 打开 `EasyScene.sln`，设置编译环境为 `Debug x64` 进行编译即可。