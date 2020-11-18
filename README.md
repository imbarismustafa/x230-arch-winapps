# x230-arch-winapps

``` sudo pacman -S libvirt virt-manager freerdp ebtables dnsmasq qemu polkit```

```sudo systemctl enable libvirtd ```

```sudo sed -i "s/#user = "root"/user = "$(id -un)"/g" /etc/libvirt/qemu.conf```

```sudo sed -i "s/#group = "root"/group = "$(id -gn)"/g" /etc/libvirt/qemu.conf```

```sudo usermod -a -G kvm $(id -un)```

```sudo usermod -a -G libvirt $(id -un)```

