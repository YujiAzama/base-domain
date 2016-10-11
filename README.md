# base-domain

## KVM Installation

```bash
$ sudo apt-get install qemu-kvm libvirt-bin virtinst openvswitch-switch
$ sudo modprobe vhost_net
# echo vhost_net >> /etc/modules
```

## Make qcow2 image

```bash
$ sudo qemu-img create -f qcow2 name.img 128G
```

## Define domain

```bash
$ sudo virsh define domain.xml
```
