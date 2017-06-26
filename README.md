# pixiet_uboot_v2015_10
mx6q/dl/s/spl mx6pixiet u-boot v2015.10 
 
# Download repository
    git clone https://github.com/Edwardteo/yocto-imx6-uboot.git 
    cd yocto-imx6-uboot.git
 
# Install cross compiler
    apt-get install gcc-arm-linux-gnueabihf
 
# Setup cross compiler
    export CROSS_COMPILE=arm-linux-gnueabihf-
    export ARCH=arm
 
# Build (imx6q)
    make distclean
    make mx6qpixiet_config
    make
    cp u-boot.imx /tftp/uboot-mx6qpixiet.imx
 
# Build (imx6dl)
    TODO
 
# Build (imx6s)
    TODO
