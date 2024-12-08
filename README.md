<a id="installation"></a>  
<img src="Source/assets/Installation.gif" width="200"/>
---

Basic command to install, configure and run QEMU/KVM using virt-manager

> [!IMPORTANT]
> Commands are based on arch-linux, however packages should be same for other distros.
> Make sure you also have a GUI environment setup.

> [!CAUTION]
> Make sure you have a internet connection and a user with sudo perms.

To install, execute the following commands:

```shell
sudo pacman -S qemu virt-manager virt-viewer dnsmasq vde2 bridge-utils openbsd-netcat ebtables iptables libguestfs
sudo systemctl enable --now libvirtd
sudo usermod -aG libvirt {user_name}
sudo systemctl restart libvirtd
```

</div>
