
	-DEF
The ethernet protocol organizes bits from the physical layer into ethernet frames so that the higher layers have 1 unique source to work with regardless of the hardware technology. This source is called an Ethernet Frame.
@@

In [computer networking](https://en.wikipedia.org/wiki/Computer_network "Computer network"), an **Ethernet frame** is a [data link layer](https://en.wikipedia.org/wiki/Data_link_layer "Data link layer") [protocol data unit](https://en.wikipedia.org/wiki/Protocol_data_unit "Protocol data unit") and uses the underlying [Ethernet physical layer](https://en.wikipedia.org/wiki/Ethernet_physical_layer "Ethernet physical layer") transport mechanisms. In other words, a [data unit](https://en.wikipedia.org/wiki/Network_packet "Network packet") on an [Ethernet](https://en.wikipedia.org/wiki/Ethernet "Ethernet") link transports an Ethernet frame as its payload.[[1]](https://en.wikipedia.org/wiki/Ethernet_frame#cite_note-IEEE_802.3_Clause_3.1.1-1)

An Ethernet [frame](https://en.wikipedia.org/wiki/Frame_(networking) "Frame (networking)") is preceded by a [preamble](https://en.wikipedia.org/wiki/Preamble_(communication) "Preamble (communication)") and start frame delimiter (SFD), which are both part of the Ethernet packet at the [physical layer](https://en.wikipedia.org/wiki/Physical_layer "Physical layer"). Each Ethernet frame starts with an Ethernet header, which contains destination and source [MAC addresses](https://en.wikipedia.org/wiki/MAC_address "MAC address") as its first two fields. The middle section of the frame is payload data including any headers for other protocols (for example, [Internet Protocol](https://en.wikipedia.org/wiki/Internet_Protocol "Internet Protocol")) carried in the frame. The frame ends with a [frame check sequence](https://en.wikipedia.org/wiki/Frame_check_sequence "Frame check sequence") (FCS), which is a 32-bit [cyclic redundancy check](https://en.wikipedia.org/wiki/Cyclic_redundancy_check "Cyclic redundancy check") used to detect any in-transit corruption of data.
@ https://en.wikipedia.org/wiki/Ethernet_frame

	-ETHERNET FRAME VARIATIONS

- Ethernet II
(also known as **DIX Ethernet**, named after [DEC](https://en.wikipedia.org/wiki/Digital_Equipment_Corporation "Digital Equipment Corporation"), [Intel](https://en.wikipedia.org/wiki/Intel "Intel") and [Xerox](https://en.wikipedia.org/wiki/Xerox "Xerox"), the major participants in its design[[8]](https://en.wikipedia.org/wiki/Ethernet_frame#cite_note-14)), defines the two-octet [EtherType](https://en.wikipedia.org/wiki/EtherType "EtherType") field in an Ethernet [frame](https://en.wikipedia.org/wiki/Frame_(telecommunications) "Frame (telecommunications)"), preceded by destination and source MAC addresses, that identifies an [upper layer protocol](https://en.wikipedia.org/wiki/Upper_layer_protocol "Upper layer protocol") [encapsulated](https://en.wikipedia.org/wiki/Encapsulation_(networking) "Encapsulation (networking)") by the frame data. For example, an EtherType value of 0x0800 signals that the frame contains an [IPv4](https://en.wikipedia.org/wiki/IPv4 "IPv4") datagram. Likewise, an EtherType of 0x0806 indicates an [ARP](https://en.wikipedia.org/wiki/Address_Resolution_Protocol "Address Resolution Protocol") frame, 0x86DD indicates an [IPv6](https://en.wikipedia.org/wiki/IPv6 "IPv6") frame and 0x8100 indicates the presence of an IEEE 802.1Q tag (as described above).

![](Ethernet_Type_II_Frame_format.svg)


- IEEE 802.3

![](Ethernet%20packet%20and%20frame%20structure%20802.3.docx)

