_**VBoxEx**_ **is an extension of VirtualBox. It will implement many useful functions that VirtualBox does not have.**


---

  * 0.0.1 version (released)
    1. The maximum count of network adapters in a VM is increased to 512 (using ICH9 chipset).

> Notes: If you encounter some errors while starting a VM with many NIC, you should increase the VM's HyperHeapSize to reslove it by modifying the VM's configuration file. The following is an example (HyperHeapSize is defined in size of KB, i.e., 20480 means 20MB):
```
<VirtualBox xmlns="http://www.innotek.de/VirtualBox-settings" version="1.13-windows">
  <Machine ...>
    <MediaRegistry>
       ...
    </MediaRegistry>
    <ExtraData>
      <ExtraDataItem name="HyperHeapSize" value="20480"/>
    </ExtraData>
```


---


**TODO:**
  * Increase the maximum size of a virtual disk
  * Export virtual disk to host OS.
  * Direct copy/paste files between host and guest via Ctrl+C/V
  * Debug application/driver in VirtualBox with Visual Studio.
  * Nested virtualization (run VirtualBox/Xen/KVM/VMware/Hyper-V in VirtualBox)
  * USB 2.0/3.0 support
  * Disk encryption
  * VM record/reply.