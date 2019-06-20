Raspberry Kernel 4.14.98 Hash 5d63a4595d32a8505590d5fea5c4ec1ca79fd49d

wget https://github.com/raspberrypi/linux/archive/5d63a4595d32a8505590d5fea5c4ec1ca79fd49d.tar.gz -O kernel-4.14.98.gz

Crosstools: git clone https://github.com/raspberrypi/tools ~/tools

export PATH=$PATH:~/tools/arm-bcm2708/gcc-linaro-arm-linux-gnueabihf-raspbian-x64/bin

make ARCH=arm CROSS_COMPILE=arm-linux-gnueabihf- menuconfig

make ARCH=arm CROSS_COMPILE=arm-linux-gnueabihf- bzImage dtbs

References: https://github.com/yutakakn/qemu-raspi
