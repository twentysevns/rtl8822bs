
# rtl8822bs

## Known Issues

- High CPU load (idle 99%).
- Not fully support iw ioctl command (iw dev del).
- Unstable AP mode when Bluetooth is ON (client always reconnected).
- Trunk version armbian won't work, need to create custom build with stable version then change kernel name to prevent kernel upgrade or hold the pkgs, dont use "main" branch. 
- AP mode stuck at 12dbm.

__NOTE:__ Other issue are not fully tested, Not for daily use.

## How to use

Clone this repository.
```
git clone https://github.com/twentysevns/rtl8822bs
cd rtl8822bs
```
Compiling kernel module and install.
```
make -j$(nproc)
sudo make install
```
load kernel module.
```
sudo modprobe 88x2bs
```
