# vnpm
计划对 node_modules 进行虚拟化，以解决项目移动时，大量细碎文件导致 IO 操作缓慢的问题。

## 需要实现的功能

+ 模拟 npm install 过程，在不进行实际下载的情况下计算 node_modules 的大小。
+ 实现跨平台的内存盘。（最好仿 WinMount，node_modules 存储在压缩包中，压缩包挂载到内存）
+ 支持内存盘挂载到指定目录。
