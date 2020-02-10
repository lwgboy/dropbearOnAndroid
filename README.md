# dropbearOnAndroid
	binary可以直接运行在ARMV7-32的安卓机器上
	用户：root 密码:123456
##编译工具链：
	工具链： arm-linux-gcc交叉编译器适用 ARMV7-32 
	下载地址: https://download.csdn.net/download/hainan613/10250099#comment
##编译步骤：
	mkdir ~/install
	./configure --host=arm-linux-gnueabihf --disable-zlib --prefix=~/install
	export STATIC=1 CC=arm-linux-gnueabihf--gcc SCPPROGRESS=0 
	make clean && make -j4 strip
	make install

