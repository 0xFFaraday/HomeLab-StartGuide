# HomeLab Guide
There are multiple aspects to creating a HomeLab. 

These aspects break down into a few categories.
- Server Hardware
- Software
- Networking Hardware
- Mounting Hardware (Optional)

## Server Hardware
There are a million different choices we can pick with our hardware. Depending on your budget you can use a older computer from a garage sale or buy a used server from online. Used servers are very common because of data centers and companies upgrade their hardware every few years which creates a surplus of used hardware.

The general criteria for hardware to have seamless virtualization follows: 
- 64-bit processor that supports virtualization with at least 8 threads or more
- 8-16GB+ of RAM 
- 500GB+ of storage (preferably an SSD for the boot drive of the operating system)

Many people use an older gaming computer or newer office computer to start small. If you are wanting to jump into the deep end, it is best to buy a server that has the ability to increase RAM and general storage overtime.

## Software
Since we picked out our server hardware, what should we run on it?
Depending on where you want to start, you can go for a bare-metal OS like [Ubuntu Server](https://ubuntu.com/download/server) or the evaluation period of [Windows Server](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2019). However, if you have the computing power to spare. I highly recommend [Proxmox VE](https://www.proxmox.com/en/proxmox-ve). This is a Debian-based distribution that is a [Type 1 Hypervisor](https://phoenixnap.com/kb/what-is-hypervisor-type-1-2) that focuses on virtualization and containers. The base edition of it is FREE and is highly universal for any environment. This will allow you to compartmentalize your services for your HomeLab like a virtual router, game servers, or container clusters.

## Networking Hardware
Our networking category can be pretty basic. 
The basics are:
- Router (Your Home's ISP Router or standalone)
- Managed Switch (Ability to configure for VLANs, Port Security, etc.)
- Cables!

Using your ISP's router for your HomeLab connection is perfectly fine. However, if you are wanting to learn router technologies like NAT, port forwarding, and firewall rules. It is best to use [pfSense](https://www.pfsense.org/) as a virtual router for free or buy one of [MikroTik's](https://www.amazon.com/MikroTik-Gigabit-Ethernet-Router-RB760iGS/dp/B07F7HDRKX/) routers which are highly valued and versatile.

Getting a managed switch is highly important because you want to secure your HomeLab's network depending on your use case. For example, using [VLANs](https://www.youtube.com/watch?v=MmwF1oHOvmg) to segment each network with its corresponding devices.

## Mounting Hardware (Optional)
If you're planning to go for the used server route, it is preferred to get some mounting hardware. [Racks](https://en.wikipedia.org/wiki/19-inch_rack) are used for storing all your HomeLab equipment. They come in many different sizes to support whatever you would like. These sizes are [Rack Units](https://en.wikipedia.org/wiki/Rack_unit) which change the overall height of your rack. Your server, switch, and router can all be mounted by its ears or buying a shelf that can support the weight. There are fancier ways to mount servers. For example, rails allow you to pull out the server and maintenance it while it is still within the rack.

### Example Projects
- [Pi-hole - DNS server that can block ads, monitor network statistics, and improve network performance](https://pi-hole.net/) 
- [Self-Hosted VPN](https://www.digitalocean.com/community/tutorials/how-to-set-up-an-openvpn-server-on-ubuntu-18-04)
- [Docker Server - Learn about containers](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04)
- [Network Attached Storage (NAS) - General network storage needs for your HomeLab](https://www.truenas.com/download-truenas-core/)

### Useful Resources
- [NetworkChuck - Network Guides and Hacking](https://www.youtube.com/c/NetworkChuck)
- [TechnoTim - HomeLab Hardware/Software infrastructure guides](https://www.youtube.com/c/TechnoTimLive)




