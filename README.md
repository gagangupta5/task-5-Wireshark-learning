# task-5-Wireshark-learning

it is a powerful network protocal analyzer

#Step 1: Launching Wireshark
What you're doing:
You open Wireshark. What Wireshark is doing:
It's preparing to list all the available network interfaces (your Ethernet, Wi-Fi, virtual adapters, etc.).

What you should see:
A list of interfaces, with graphs showing live traffic (e.g., Wi-Fi: en0, Ethernet: eth0, etc.).

#Step 2: Selecting the Right Interface
What you're doing:
You click the interface that is currently active (like Wi-Fi) and hit Start.

What Wireshark is doing:
It starts capturing packets in real-time from that interface. Every single packet that goes through your network card is being logged.

#Step 3: Watching Packets Flow
What you're seeing:
A flood of packets in the top pane: each line is a separate packet. Columns show No., Time, Source, Destination, Protocol, Length, and Info.

What you're doing:
You observe the packets. You might see: ARP requests DNS queries HTTP traffic if you're browsing TCP handshakes

#Step 4: Filtering Traffic
What you're doing: You type a filter like http, ip.addr == 192.168.1.1, or tcp.port == 80 into the top filter bar.

What Wireshark is doing:
It narrows down the view to show only packets matching that filter. For example, http shows only web traffic, which is useful for web debugging or analysis.

#Step 5: Analyzing a Packet
What you're doing:
You click a packet, and the middle pane expands it into layers (e.g., Ethernet II, IP, TCP, HTTP). You click each layer to explore fields like IP addresses, port numbers, flags, sequence numbers, etc.

What’s happening:
You're seeing the OSI model in action: Layer 2: Ethernet Layer 3: IP Layer 4: TCP/UDP Layer 7: Application protocols (like HTTP, DNS, etc.)

#Step 6: Saving or Exporting Data
What you're doing:
You click File > Save As... to store the packet capture as a .pcap file for later analysis.

Why it’s useful:
You can load this file later to continue analysis or share with someone for troubleshooting or forensic investigation.

#Step 7: Stopping the Capture What you're doing: You click the red square Stop button at the top.

Result:
Capture freezes. You can now analyze data without new packets being added.
