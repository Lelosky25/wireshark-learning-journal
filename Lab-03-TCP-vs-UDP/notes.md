# Lab 03 - TCP vs UDP

## Objective

Learn the differences between TCP and UDP by capturing and analyzing network traffic in Wireshark.

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

- Total Packets Captured: 10,045
- TCP Packets: 5,959
- UDP/QUIC Packets: 2,992

---

## Investigation Results

### TCP Analysis

- TCP was the most common protocol observed during the packet capture.
- TCP is a connection-oriented protocol that provides reliable communication by ensuring packets are delivered correctly and in order.

### UDP Analysis

- When filtering for UDP traffic, most packets were identified as QUIC traffic.
- QUIC is a modern transport protocol that runs over UDP and is commonly used by services such as Google and YouTube to improve performance and reduce latency.

### Packet Details

- Source Port: 54491
- Destination Port: 51
- Sequence Number: 1
- Acknowledgment Number: 1

---

## Findings

- TCP generated more traffic than UDP during this capture.
- Modern web traffic commonly uses encrypted protocols, making it difficult to identify specific website content.
- QUIC traffic was observed when filtering for UDP packets.
- Encrypted web traffic helps protect user privacy and communications.

---

## TCP vs UDP Comparison

### TCP

- Connection-oriented
- Reliable delivery
- Performs error checking
- Guarantees packet delivery
- Commonly used for:
  - HTTPS
  - File transfers
  - Email
  - Web browsing

### UDP

- Connectionless
- Faster communication
- No guarantee of packet delivery
- Lower overhead
- Commonly used for:
  - DNS
  - Voice over IP (VoIP)
  - Video streaming
  - Online gaming
  - QUIC

---

## What I Learned

- TCP and UDP serve different purposes depending on the application.
- TCP prioritizes reliability, while UDP prioritizes speed.
- QUIC is built on top of UDP and is widely used by modern web applications.
- Encrypted traffic can limit the visibility of website content within packet captures.
- Source ports, destination ports, sequence numbers, and acknowledgment numbers are important components of TCP communication.

---

## Reflection

This lab helped me understand why different applications use different transport protocols. I learned that TCP is used when reliable communication is required, while UDP is preferred for applications where speed is more important than guaranteed delivery. I also observed how modern websites use encrypted protocols such as QUIC, making it more difficult to identify website content directly from packet captures. This lab strengthened my understanding of network communications and transport layer protocols.
