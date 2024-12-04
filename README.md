
## rtl8822bs


### Known Issues

```
High CPU load (idle 99%)
Not fully support iw ioctl command (iw dev del)
Unstable AP mode when Bluetooth is ON
```

NOTE: Other issue are not fully tested, Not for daily use.

### How to use

Install linux-header first, that depend on your kernel!

```
git clone https://github.com/twentysevns/rtl8822bs
cd rtl8822bs
make -j$(nproc)
sudo make install
sudo modprobe 88x2bs
```

