

<img src="https://cannectivity.org/_static/CANnectivity.png" width="300" alt="CANnectivity Logo">

Project

https://cannectivity.org/building.html


Github

https://github.com/CANnectivity


INSTALL Ubuntu 24.04
------------------------------

west init -m https://github.com/CANnectivity/cannectivity --mr main my-workspace

 sudo apt update
 
 apt list --upgradable
 
 sudo apt install python3-pip python3-venv
 
 pip install --user -U west
 
 python3 -m venv .venv

cd my-workspace

source .venv/bin/activate

export ZEPHYR_TOOLCHAIN_VARIANT=gnuarmemb

export GNUARMEMB_TOOLCHAIN_PATH=/usr

west update

..

USB CAN FD SOLO     

west build -b usbcanfd_Oleksii_g431  cannectivity/app/ -- -DFILE_SUFFIX=release

USB CAN FD DUAL        

west build -b usbcanfd_Oleksii_g473  cannectivity/app/ -- -DFILE_SUFFIX=release

----------------------------
can-module.com
--------------------------

<img src="https://github.com/AlekseyMamontov/CANnectivity-_CANFD-_adapters/blob/main/img/Too_adapters2.jpeg" width="400" alt="USBCANFD 2ch adapter can-module.com">



