# UE4ConsoleCommand
This is a Collection of UnrealEngine4 Console Command. Must of them are using in my projects.

这个合集为UE4控制台命令合集，大部分是我在项目工作中收集的，我会尽最大努力将这些写得详尽一点，并且由于本人英文比较菜，所以优先更新中文资料。如有错误，欢迎大家指正。
## GoogleVR Plugin Command(Google VR插件)
该部分命令仅在启用GoogleVR 的情况下可用
### STEREO ON/OFF
开启或关闭立体渲染模式，关闭后，只渲染单一画面。可用作进入和退出VR模式。*注意：开启或关闭该模式画面依然会跟随陀螺仪状态进行移动*


### HMD ON/OFF
开启或者关闭HMD模式，在GoogleVR 中，最终效果和命令"STEREO ON/OFF" 一样（代码就是调用的同一个方法）


### DISTORT
控制反畸变功能，参数和对应功能如下：
#### ON/OFF
开启或关闭反畸变功能。关闭反畸变功能后渲染开销降低，FPS会有一定的提升。
#### PPHMD
关闭反畸变功能。
#### GVRAPI
开启反畸变功能。


### GVRRENDERSIZE
调整渲染尺寸相关参数
#### W=? H=?
根据W和H的值设置渲染的宽度和高度大小
#### S=?
根据S的值设置渲染目标尺寸
#### RESET
设置渲染尺寸为默认值


### DISTORTMESH
只在GoogleVRHMD支持的设备上有效，在使用虚幻后期处理反畸变时，调整反畸变模型的偏移量（mesh vert count）。参数设置偏移量由小到大分别为：
1. VERSMALL
1. SMALL
1. MEDIUM
1. LARGE
1. VERYLARGE
### GVRSPLASH
*暂时还不知道此命令的作用*
