
1. What is a Network?

A network allows devices to:

Send/receive data
Share files
Access internet
Communicate with servers
Use printers, databases, cloud services, etc.
Common Devices in a Network
6
Main components
Router → Connects different networks
Switch → Connects devices inside same network
Server → Provides services/data
Client → User devices
Firewall → Security protection
2. IP Address

Every device in a network gets an IP address.

Example IPv4:

192.168.1.10

Think of it like a house address for devices.

Two main versions:

IPv4 → 192.168.1.1
IPv6 → 2001:db8::1









An IP address (Internet Protocol address) is a unique number assigned to a device connected to a network or the internet.
## IPv4 Explained

**IPv4 (Internet Protocol Version 4)** is the most widely used version of the internet protocol.
It gives every device on a network a unique address so devices can communicate.

### Structure of IPv4

An IPv4 address is a **32-bit number** divided into **4 parts (octets)**.

Example:

```text
192.168.1.10
```

Each part:

* ranges from `0` to `255`
* separated by dots (`.`)

### Why only 0–255?

Because each octet contains **8 bits**.

2^8 = 256

Values start from `0`, so:

* minimum = `0`
* maximum = `255`

---

## Binary Form

Computers understand binary (0 and 1).

Example:

```text
192.168.1.10
```

in binary:

```text
11000000.10101000.00000001.00001010
```

---

## Parts of an IPv4 Address

IPv4 has:

1. **Network Portion** → identifies the network
2. **Host Portion** → identifies the device

Example:

```text
192.168.1.10/24
```

* `192.168.1` → network
* `10` → host/device

---

## Classes of IPv4

| Class | Range   | Purpose         |
| ----- | ------- | --------------- |
| A     | 1–126   | Large networks  |
| B     | 128–191 | Medium networks |
| C     | 192–223 | Small networks  |
| D     | 224–239 | Multicast       |
| E     | 240–255 | Research        |

---

## Private IP Ranges

These are used inside local networks.

| Range                           |
| ------------------------------- |
| `10.0.0.0 – 10.255.255.255`     |
| `172.16.0.0 – 172.31.255.255`   |
| `192.168.0.0 – 192.168.255.255` |

Example:

* Your Wi-Fi router may give your laptop:

```text
192.168.1.5
```

---

## Special IPv4 Addresses

| Address           | Meaning                      |
| ----------------- | ---------------------------- |
| `127.0.0.1`       | Localhost (your own machine) |
| `0.0.0.0`         | Default/unknown              |
| `255.255.255.255` | Broadcast                    |





What is a Subnet?

A subnet (subnetwork) is a smaller network created from a large network.

Instead of keeping all devices in one huge network, we divide them into smaller sections.

Example:

Main Network:
192.168.1.0/24

Subnets:
192.168.1.0/26
192.168.1.64/26
192.168.1.128/26
192.168.1.192/26
Why Subnets are Used
1. Better Performance

Smaller networks reduce unnecessary traffic.

2. Security

Different departments can be separated.

Example:

HR subnet
Finance subnet
Developers subnet
3. Easier Management

Admins can organize networks properly.

4. Efficient IP Usage

Avoid wasting IP addresses.

4. Understanding Network Parts

Example IP:

192.168.1.10/24

This has:

Network part
Host part
/24 means:

First 24 bits are network bits.

Subnet mask:

255.255.255.0
5. Subnet Mask

Subnet mask identifies:

Which part is network
Which part is host
Example

IP:

192.168.1.10

Subnet mask:

255.255.255.0

This means:

Network: 192.168.1.0
Host:    .10








## Subnet Mask

A subnet mask tells which part is network and which is host.

Example:

```text
IP Address : 192.168.1.10
Subnet Mask: 255.255.255.0
```

This means:

* first 3 octets → network
* last octet → host

---

## CIDR Notation

Instead of subnet masks, modern networks use CIDR.

Example:

```text
192.168.1.10/24
```

`/24` means:

* first 24 bits are network bits.

8 + 8 + 8 = 24

---



What is a Subnet?

A subnet (subnetwork) is a smaller network created from a large network.

Instead of keeping all devices in one huge network, we divide them into smaller sections.

Example:

Main Network:
192.168.1.0/24

Subnets:
192.168.1.0/26
192.168.1.64/26
192.168.1.128/26
192.168.1.192/26
Why Subnets are Used
1. Better Performance

Smaller networks reduce unnecessary traffic.

2. Security

Different departments can be separated.

Example:

HR subnet
Finance subnet
Developers subnet
3. Easier Management

Admins can organize networks properly.

4. Efficient IP Usage

Avoid wasting IP addresses.

4. Understanding Network Parts

Example IP:

192.168.1.10/24

This has:

Network part
Host part
/24 means:

First 24 bits are network bits.

Subnet mask:

255.255.255.0
5. Subnet Mask

Subnet mask identifies:

Which part is network
Which part is host
Example

IP:

192.168.1.10

Subnet mask:

255.255.255.0

This means:

Network: 192.168.1.0
Host:    .10


EXAMPLE OF SUBNET CALCULATION 

What is a Subnet?

A subnet (subnetwork) is a smaller network created from a large network.

Instead of keeping all devices in one huge network, we divide them into smaller sections.

Example:

Main Network:
192.168.1.0/24

Subnets:
192.168.1.0/26
192.168.1.64/26
192.168.1.128/26
192.168.1.192/26
Why Subnets are Used
1. Better Performance

Smaller networks reduce unnecessary traffic.

2. Security

Different departments can be separated.

Example:

HR subnet
Finance subnet
Developers subnet
3. Easier Management

Admins can organize networks properly.

4. Efficient IP Usage

Avoid wasting IP addresses.

4. Understanding Network Parts

Example IP:

192.168.1.10/24

This has:

Network part
Host part
/24 means:

First 24 bits are network bits.

Subnet mask:

255.255.255.0
5. Subnet Mask

Subnet mask identifies:

Which part is network
Which part is host
Example

IP:

192.168.1.10

Subnet mask:

255.255.255.0

This means:

Network: 192.168.1.0
Host:    .10




