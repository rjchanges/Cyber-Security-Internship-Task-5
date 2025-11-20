# Task 5: Network Traffic Analysis with Wireshark

## Overview
This project involves capturing live network traffic to analyze and identify different communication protocols using Wireshark. The goal is to understand how data packets are structured and transmitted over a network.

## Objectives
- Capture live network packets from an active interface.
- Filter and analyze specific protocols (TCP, TLS, DNS).
- Generate a `.pcap` file for review.

## Tools Used
- **Wireshark:** For packet capturing and analysis.
- **Web Browser:** To generate live HTTP/HTTPS and DNS traffic.

## Findings & Analysis

### 1. TCP (Transmission Control Protocol)
**Observation:** I captured the TCP 3-way handshake, which establishes a reliable connection between my client and the server.
- **Key Details:** Observed flags like `SYN` (synchronize) and `ACK` (acknowledge), ensuring reliable delivery.
- **Screenshot:** ![TCP Capture](tcp_screenshot.png)

### 2. TLS (Transport Layer Security)
**Observation:** Most modern web traffic is encrypted. I filtered for `tls` to view this secure traffic.
- **Key Details:** The capture shows the "Client Hello" and "Server Hello" handshake packets used to negotiate encryption keys.
- **Screenshot:** ![TLS Capture](tls_screenshot.png)

### 3. DNS (Domain Name System)
**Observation:** DNS packets were captured when my browser resolved domain names into IP addresses.
- **Key Details:** I observed queries for `gemini.google.com` and `canva.com`. This traffic helps map human-readable names to machine-readable IP addresses.
- **Screenshot:** ![DNS Capture](dns_screenshot.png)

## Conclusion
This task demonstrated the variety of traffic on a standard network, distinguishing between reliable transport (TCP), encrypted data (TLS), and name resolution (DNS).
