# NetPractice

- you can see in you lap your (IPv6 Address, Temporary IPv6 Address; Link-local IPv6 Address; IPv4 Address; Subnet Mask; Default Gateway): ``` ipconfig ```
- Default Gateway: forwards data from one network to another. (router: router only connects the devices with each other to make a LAN between them all, but with no access to the internet, a modem can connect to one device only, but provides access to the internet. To make a LAN that connects to the internet, you should combine both a modem and a router together, the router connects all the devices while a modem give them access to the internet.)
- Default: designated device is the first option thats looked upon when data needs to exit the network.
- IPv4 Address:works with a 32-bits address, and has over 4.3 billion addresses, IP addresses must be reused and masked, and it uses Numeric Dot-Decimal Notation and you have to configure it manually.
- IPv6 Address:works with a 128-bits address, and has over 340 undecillion addresses, every device can have it's unique IP address, and it uses Alphanumeric Hexadecimal Notation and it supports auto-configuration.

# IP ADDRESS
- IP address stands for Internet Protocol Address
- IP address: identifier for a computer or device on a network.
- consists of two parts: Network address, Host address.
-  set of rules for communication over the internet, such as sending emails, streaming videos, or connecting to a website, etc….
-  types of an IP address: 1. Static IP address: which stay permanent and it doesn’t change, and it’s used mostly for important equipement, such as (businesses, servers…)
2. Dynamic IP address: which changes occasionally, and it’s used for consumer equipement, such as (laptop, smartphone, tablet…)

# Subnet Mask
- [subnet mask](https://www.youtube.com/watch?v=s_Ntt6eTn94): reveals how many bits in the IP address are used for the network by masking the network portion of the IP address
- networks can be logically broken down into smaller networks, wihich knows as subnetting(stealing bits from the HOST part of IP address in order to divide the large network into smaller).
- 32 bits (4 bytes) address used to distinguish between a network address and a host address in the IP address. It defines the range of IP addresses that can be used within a network or a subnet.

# Switch
- switch is a device that connects devices within the same network, usually a LAN network (which is a Local Area Network)
- switch does not have any interfaces since it only distributes packets to its local network, and cannot talk directly to a network outside of its own.
  
![o](https://github.com/fasl8/NetPractice/blob/main/IP%20address.png)
- how to find binary number?
  8 bit octet chart(128 64 32 16 8 4 2 1) -> 128 + 64 = 192 that mean 1 1 0 0 0 0 0 0 becuase binary numbers are made up of 1 and 0 , 1 is count 0 does not count.

# TCP/IP
- TCP/IP stands for Transmission Control Protocol/Internet Protocol
- set of rules that guide and allow computers to communicate on a network such as the internet.
- IP is the part that obtains the address which the data is sent to, while TCP is the part that is responsible for data delivery once that IP address has been found.
- TCP/IP is to divide the different communication tasks into layers, each layer has a different function. Data goes through four individual layers before it is recieved on the other end.
- Datalink Layer(physical layer): handles the physical parts of sending and recieving data using the Ethernet, or WiFi.
- Internet Layer(network layer): controls the movement of the packets around the internet.
- Transport Layer: is what provides a reliable data connection between two devices, it divides the data into packets, knows the packets that are recieved from the other device, and it makes sure that the other device knows the packets it recieves.
- Application Layer: is the group of the applications that requires a network communication, which is what the user typically interacts with, such as emails, and messaging, because the lower layer handles the details of communication, and there’s no need for the applications to concern themselves with it.

![L1](https://github.com/fasl8/NetPractice/blob/main/level1.png)
# LEVEL 2
1.Understanding the Subnet Mask:
- subnet mask 255.255.255.252, when converted to binary, looks like this: 11111111.11111111.11111111.11111100.
In slash notation, /30 represents the number of bits in the subnet mask that are set to 1. In this case, there are 30 bits set to 1, leaving 2 bits for hosts.
- Interface D1 uses a subnet mask of /30, which means the first 30 bits of the IP address are dedicated to the network, leaving 2 bits for the host.
- Interface C1 uses a subnet mask of 255.255.255.252, which is equivalent to /30 in slash notation.
2. Determining the Network Address:
Both interfaces D1 and C1 belong to the same network because they share the same subnet mask (/30).
The network address for both interfaces is determined by the first 30 bits of their IP addresses.

https://github.com/lpaube/NetPractice?tab=readme-ov-file#subnet-mask
