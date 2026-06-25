# Lab 01 - Basic Packet Capture

## Objective

Learn how to capture and analyze network traffic using Wireshark.

---

## Tools Used

- Kali Linux
- Wireshark

---

## Lab Setup

- Operating System: Kali Linux (VirtualBox VM)
- Network Interface: eth0

---

## Capture Information

- Interface Used: eth0
- Total Packets Captured: 24,500

---

## Protocols Observed

| Protocol | Packets |
|----------|---------:|
| TCP | 18,032 |
| QUIC | 6,160 |
| TLSv1.3 | 5,048 |
| DNS | 308 |

---

## Findings

- TCP was the most common protocol observed.
- DNS requests were generated while visiting websites.
- TLSv1.3 traffic showed that web communications were encrypted.
- QUIC traffic was heavily used while browsing Google and YouTube.

---

## Observation

I expected to see HTTP traffic because I visited Google, YouTube, and Wikipedia. However, no HTTP traffic appeared.

After researching, I learned that modern websites use HTTPS instead of HTTP. HTTPS encrypts traffic using TLS, which explains the large amount of TLSv1.3 packets observed during the capture.

I also discovered QUIC, a modern transport protocol that operates over UDP and is used heavily by Google services to improve speed and performance.

---

## What I Learned

- How to start and stop a packet capture in Wireshark.
- How to identify common network protocols.
- TCP was the most common protocol during my capture.
- DNS translates domain names into IP addresses.
- Modern websites primarily use HTTPS instead of HTTP.
- TLS encrypts web traffic.
- QUIC is commonly used by Google and YouTube for faster communication.

---

## Reflection

This was my first Wireshark lab. I learned how to capture live network traffic and identify several common protocols. I was surprised that I did not observe any HTTP traffic, which led me to learn about HTTPS, TLS, and QUIC. This lab gave me a better understanding of how modern web traffic works and provided a strong foundation for future packet analysis.
