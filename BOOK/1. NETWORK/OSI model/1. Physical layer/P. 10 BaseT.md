IT VAULT
NETWORK CHAPTER
10 BASE T PROTOCOL

#-1_physical_layer/10BaseT 

A type of standard for implementing Ethernet networks. 10BaseT is the most popular form of 10-Mbps Ethernet, using <mark style="background: #FFB8EBA6;">unshielded twisted-pair</mark> (UTP) cabling for connecting stations, and using hubs to form a network. 10BaseT supports a maximum bandwidth of 10 Mbps, but in actual networks, the presence of collisions reduces this to more like 4 to 6 Mbps. 10BaseT is based on the <mark style="background: #FFB8EBA6;">802.3 specifications</mark> of <mark style="background: #FFB8EBA6;">Project 802</mark> developed by the Institute of Electrical and Electronic Engineers (IEEE).

- 10BaseT networks are wired together in a <mark style="background: #FFB8EBA6;">star topology</mark> to a central hub. The UTP cabling used for wiring should be category 3 cabling, category 4 cabling, or category 5 cabling, terminated with RJ-45 connectors. Patch panels can be used to organize wiring and provide termination points for cables running to wall plates in work areas. Patch cables then connect each port on the patch panel to the hub. Usually, most of the wiring is hidden in a wiring cabinet and arranged on a rack for easy access.

- The maximum length of any particular segment of a 10BaseT network is 100 meters. If distances longer than this are required, two or more segments must be connected using repeaters. The minimum length of a segment should be 2.5 meters. By using stackable hubs or by cascading regular hubs into a cascaded star topology, you can network large numbers of computers using 10BaseT cable. Although they support up to 1024 nodes, collision domains supporting no more than 200 or 300 nodes will yield the best performance.


	-timeline
Early <mark style="background: #FF5582A6;">Ethernet</mark> <mark style="background: #FFB86CA6;">used</mark> <mark style="background: #FFF3A3A6;">various grades</mark> of [coaxial cable](https://en.wikipedia.org/wiki/Coaxial_cable "Coaxial cable"), but in 1984, [StarLAN](https://en.wikipedia.org/wiki/StarLAN "StarLAN") <mark style="background: #FFB86CA6;">showed</mark> the <mark style="background: #FFF3A3A6;">potential</mark> of simple [unshielded twisted pair](https://en.wikipedia.org/wiki/Unshielded_twisted_pair "Unshielded twisted pair"). This led to the development of <mark style="background: #FFB8EBA6;">10BASE-T</mark>  and its successors [100BASE-TX](https://en.wikipedia.org/wiki/100BASE-TX "100BASE-TX"), [1000BASE-T](https://en.wikipedia.org/wiki/1000BASE-T "1000BASE-T") and [10GBASE-T](https://en.wikipedia.org/wiki/10GBASE-T "10GBASE-T"), supporting speeds of 10 and 100 [megabit per second](https://en.wikipedia.org/wiki/Megabit_per_second "Megabit per second"), then 1 and 10 gigabit per second respectively.[[a]](https://en.wikipedia.org/wiki/Ethernet_over_twisted_pair#cite_note-2)

Two new variants of 10 megabit per second Ethernet over a _single_ twisted pair, known as <mark style="background: #FFB8EBA6;">10BASE-T1S</mark>  and <mark style="background: #FFB8EBA6;">10BASE-T1L</mark> , were standardized in <mark style="background: #FFB8EBA6;">IEEE Std 802.3cg-2019.[[2]]</mark> (https://en.wikipedia.org/wiki/Ethernet_over_twisted_pair#cite_note-ieee802.3CG-3) <mark style="background: #FFB8EBA6;">10BASE-T1S</mark> has its origins in the automotive industry and may be useful in other short-distance applications where substantial electrical noise is present. <mark style="background: #FFB8EBA6;">10BASE-T1L</mark> is a long-distance Ethernet, supporting connections up to 1 km in length. Both of these standards are finding applications implementing the [Internet of things](https://en.wikipedia.org/wiki/Internet_of_things "Internet of things").

The earlier standards use [8P8C modular connectors](https://en.wikipedia.org/wiki/8P8C_modular_connector "8P8C modular connector"),[[b]](https://en.wikipedia.org/wiki/Ethernet_over_twisted_pair#cite_note-4) and supported cable standards range from [Category 3](https://en.wikipedia.org/wiki/Category_3_cable "Category 3 cable") to [Category 8](https://en.wikipedia.org/wiki/Category_8_cable "Category 8 cable"). These cables typically have four pairs of wires for each connection, although early Ethernet used only two of the pairs. Unlike the earlier -T standards, the -T1 interfaces were designed to operate over a single pair of conductors and introduce the use of two new connectors referred to as IEC 63171-1[[3]](https://en.wikipedia.org/wiki/Ethernet_over_twisted_pair#cite_note-IEC_63171-1-5) and IEC 63171-6.[[4]](https://en.wikipedia.org/wiki/Ethernet_over_twisted_pair#cite_note-IEC_63171-6-6)

#-1_physical_layer/10BaseT/coaxial_cable
#-1_physical_layer/10BaseT/unshielded_twisted_pair
#-1_physical_layer/100BaseTX
#-1_physical_layer/1000Base-T
#-1_physical_layer/10GBase-T
#-1_physical_layer/10Base-T1S
#-1_physical_layer/10Base-T1L
#-1_physical_layer/IEEE_Std_802-3cg--2019-2
