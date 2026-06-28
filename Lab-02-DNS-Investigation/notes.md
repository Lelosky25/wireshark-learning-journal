# Lab 02 - DNS Investigation

## Objective

Learn how DNS traffic appears in Wireshark and understand how domain names are translated into IP addresses.

---

## Tools Used

- Kali Linux
- Wireshark

---

## Lab Setup

- Operating System: Kali Linux (VirtualBox VM)
- Network Interface: Wi-fi

---

## Capture Information

- Total Packets Captured: 36,670
- DNS Packets: 582

---

## Websites Visited

- google.com
- wikipedia.org
- youtube.com

---

## Investigation Results

### Example DNS Query

Requested Domain:

www.google.com

### DNS Response

The DNS server returned the information required for the computer to connect to Google's services.

### DNS Record Type

- Type: A
- Class: IN

---

## Findings

- DNS packets were generated each time a website was visited.
- Every DNS query observed appeared to receive a matching response.
- DNS traffic occurred before establishing connections to websites.
- Type A records were used to obtain IPv4 addresses.

---

## What I Learned

- DNS translates domain names into IP addresses.
- A DNS query is a request asking a DNS server to resolve a domain name.
- A DNS response contains the information needed to connect to the requested website.
- Type A records return IPv4 addresses.
- Class IN represents the Internet.

---

## Reflection

This lab helped me understand how computers locate websites before establishing a connection. Before this lab, I knew websites had IP addresses but did not understand how they were found. After analyzing DNS traffic in Wireshark, I now understand that DNS acts like the Internet's directory service, allowing computers to translate domain names into IP addresses automatically.
