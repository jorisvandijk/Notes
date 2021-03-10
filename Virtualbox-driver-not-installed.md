# Virtualbox driver not installed

```
Kernel driver not installed (rc=-1908)

The VirtualBox Linux kernel driver (vboxdrv) is either not loaded or there is a permission problem with /dev/vboxdrv. Please reinstall the kernel module by executing

'/sbin/vboxconfig'

as root.

where: suplibOsInit what: 3 VERR_VM_DRIVER_NOT_INSTALLED (-1908) - The support driver is not installed. On linux, open returned ENOENT. 
```

It's a super simple solution I always have to search for whenever I run into this error after installing Virtualbox.

```
sudo modprobe vboxdrv
```

That's it.