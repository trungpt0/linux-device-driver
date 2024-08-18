# Usage

Insert and remove kernel module

## Insert

```bash
make
sudo insmod dfile.ko
ls -l /dev | grep "rootv_device"
sudo dmesg | tail -10
sudo chmod 777 /dev/rootv_device
```
## App

```bash
make -f Makefile1
./app
```

## Remove

```bash
sudo rmmod dfile
sudo dmesg | tail -10
make clean
make clean -f Makefile1
```

# Authors

Trung Tran (RootV)

# License

GPL