# Task 5: Capture and Analyze Network Traffic Using Wireshark

## Objective

The objective of this task is to capture live network packets using Wireshark and analyze the captured traffic to identify different network protocols and understand basic network communication.

## Tools Used

- Wireshark
- Windows Command Prompt
- Internet connection

## Task Performed

For this task, Wireshark was used to capture live network traffic from the active network interface.

The following activities were performed to generate network traffic:

1. Started a packet capture in Wireshark.
2. Used Command Prompt to generate ICMP traffic with:
   ```text
   ping google.com
   ```
3. Used DNS lookup to generate DNS-related traffic:
   ```text
   nslookup google.com
   ```
4. Accessed a website through a web browser to generate additional network traffic.
5. Stopped the Wireshark capture after collecting sufficient packets.
6. Applied Wireshark display filters to analyze the captured packets.

## Protocol Analysis

The captured traffic was analyzed using Wireshark display filters.

### DNS

Filter used:

```text
dns
```

DNS packets were examined to understand domain-name resolution between the system and DNS servers.

### ICMP

Filter used:

```text
icmp
```

ICMP traffic was generated using the `ping google.com` command. The captured packets can be used to observe Echo Request and Echo Reply communication.

### TCP

Filter used:

```text
tcp
```

TCP packets were examined to identify TCP-based network communication present in the capture.

## Wireshark Filters Used

```text
dns
```

```text
icmp
```

```text
tcp
```

These filters were used to isolate specific types of traffic and make packet analysis easier.

## Key Observations

- Wireshark successfully captured live network traffic.
- DNS traffic could be filtered and analyzed using the `dns` display filter.
- ICMP traffic was generated using the `ping` command and analyzed using the `icmp` filter.
- TCP traffic was examined using the `tcp` display filter.
- Wireshark provides packet-level information such as source, destination, protocol, packet length, and packet details.

## Files Included

```text
README.md
task5_network_capture.pcapng
report/
screenshots/
```

The packet capture file contains the network traffic collected during the practical exercise.

## Conclusion

This task provided hands-on experience with capturing and analyzing network traffic using Wireshark. The activity helped in understanding packet capture, protocol identification, display filtering, and basic network troubleshooting concepts.

Wireshark can be useful for examining network communication and identifying issues by analyzing individual packets and protocols.
