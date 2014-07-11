* dinstall

安装一个脚本文件，或者可执行文件，同时又支持将这个脚本文件的解释器(#!后的程序)
和可执行程序所依赖的库文件(ldd 后依赖的库文件) 一同copy 到目标 rootfs 下

制作 initrd.img 的时候因为需要在 img 的rootfs 上安装perl nc rsync 等相关命令和
依赖的库。


* sample usage.

<pre>
# dinstall -l -D /home/yuting/i/t -a /usr/local/bin/fornode.pl
# find t
t
t/usr
t/usr/local
t/usr/local/bin
t/usr/local/bin/fornode.pl
t/usr/local/bin/perl
t/usr/local/lib
t/usr/local/lib/perl5
t/usr/local/lib/perl5/5.8.9
t/usr/local/lib/perl5/5.8.9/x86_64-linux
t/usr/local/lib/perl5/5.8.9/x86_64-linux/CORE
t/usr/local/lib/perl5/5.8.9/x86_64-linux/CORE/libperl.so
t/lib
t/lib/x86_64-linux-gnu
t/lib/x86_64-linux-gnu/libc-2.15.so
t/lib/x86_64-linux-gnu/libc.so.6
t/lib/x86_64-linux-gnu/libm-2.15.so
t/lib/x86_64-linux-gnu/libm.so.6
t/lib/x86_64-linux-gnu/libdl.so.2
t/lib/x86_64-linux-gnu/ld-2.15.so
t/lib/x86_64-linux-gnu/libdl-2.15.so
t/lib64
t/lib64/ld-linux-x86-64.so.2

</pre>
  
