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

---

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

## Limitation of IPv4

IPv4 supports about:

2^{32} \approx 4.3 \times 10^9

Around **4.3 billion addresses** only.

Because internet devices increased massively, IPv6 was introduced.

---

## Real Example Flow

When you open a website:

1. Your device has an IP
2. Website server has an IP
3. Routers use these IPs to send data packets
4. Response comes back to your device

Just like sending letters using postal addresses.
