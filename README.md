* dinstall

* 命令* dinstall

安装一个脚本文件，或者可执行文件，同时又支持将这个脚本文件的解释器(#!后的程序)
和可执行程序所依赖的库文件(ldd 后依赖的库文件) 一同copy 到目标 rootfs 下

制作 initrd.img 的时候因为需要在 img 的rootfs 上安装perl nc rsync 等相关命令和
依赖的库


  
