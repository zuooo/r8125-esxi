!!! LACK OF TESTING, Please test and feedback.

!!! WARNING: Do not use in production environment.


# Realtek RTL8125 NIC driver for ESXi 6.7

This source code is based on realtek official source, VMware-ESXI-67U3-ODP and VMware-TOOLS-10.2.0-ODP.

Just do these steps:
- Prepare the building environment, I did it on CentOS 7
- Log in with root, make a folder name 'build' on /, make folder toolchain and vsphere in /build.
- Copy and extract gcc-4.8.0, binutils-2.22, glibc-2.3.4-2.41 to /build/toolchain/src 
- Compile the toolchain, dest path is /build/toolchain/lin64
- Extract and copy vmkdrivers-gpl from 67U3-ODP to /build/vsphere
- Copy build-r8125.sh to /build/vsphere/vmkdrivers-gpl/
- Copy r8125 folder to /build/vsphere/vmkdrivers-gpl/vmkdrivers/src_9/drivers/net
- Run build-r8125.sh

# Realtek PCIe FE / GBE / 2.5G / Gaming Ethernet Family Controller Software

- https://www.realtek.com/en/component/zoo/category/network-interface-controllers-10-100-1000m-gigabit-ethernet-pci-express-software

# VMware vSphere Hypervisor (ESXi) 6.7 Open Source Information

- https://my.vmware.com/web/vmware/downloads/details?downloadGroup=ESXI670-OSS&productId=742

## Open Source Disclosure packages for VMWare vSphere Hypervisor (ESXi) 6.7.0

- MD5SUM:	205b26afde7f87d5a68cc98203da9a6c
- SHA1SUM: 	1f5c274fe4f737631cfad2d9a0bdaa00c4a55d65
- SHA256SUM: 	00c387fb3361eb85d73729462f0e268e8752924d209557b3f9efbd617cd32c7c
- https://download3.vmware.com/software/vsphere67/open-source/VMware-ESXI-670-ODP.iso

## Open Source Disclosure Package for VMware vSphere Hypervisor (ESXi) 6.7 Toolchain

TOOLCHAIN packages, contains all the used toolchains during the build process, together with source, build instructions and build scripts.

- MD5SUM:	0a01bb88c6058aa9c5a966af48d13b87
- SHA1SUM: 	09e18fa77bb2cbc7a9fffc874715602f2ab0aad6
- SHA256SUM: 	4545117140af9fe4ba6969274834a95ecf173ce7836b2a6fbccb54aacb1da214
- https://download3.vmware.com/software/vsphere67/open-source/VMware-TOOLS-10.2.0-ODP.iso
