IT VAULT
NETWORK CHAPTER
OSI MEDIA ACCESS CONTROL SUBLAYER
#-2_data_link_layer/media_access_control_sublayer

<mark style="background: #FFB8EBA6;">Media_Access_Control</mark> may refer to the sublayer that determines who is allowed to access the media at any one time (e.g. [CSMA_CD](https://en.wikipedia.org/wiki/Carrier-sense_multiple_access_with_collision_detection "Carrier-sense multiple access with collision detection")). (<mark style="background: #FFB8EBA6;">corr. CSMA/CD</mark> ) Other times it refers to a [frame_structure](https://en.wikipedia.org/wiki/Frame_(networking) "Frame (networking)") delivered based on [MAC addresses](https://en.wikipedia.org/wiki/MAC_address "MAC address") inside.

There are generally two forms of media access control: distributed and centralized.[[4]](https://en.wikipedia.org/wiki/Data_link_layer#cite_note-Miao-4) Both of these may be compared to communication between people. In a network made up of people speaking, i.e. a conversation, they will each pause a random amount of time and then attempt to speak again, effectively establishing a long and elaborate game of saying "no, you first".

The Media Access Control sublayer also performs [frame synchronization](https://en.wikipedia.org/wiki/Frame_synchronization "Frame synchronization"), which determines the start and end of each frame of data in the transmission [bitstream](https://en.wikipedia.org/wiki/Bitstream "Bitstream"). It entails one of several methods: timing-based detection, character counting, byte stuffing, and bit stuffing.

-   The time-based approach expects a specified amount of time between frames.
-   Character counting tracks the count of remaining characters in the frame header. This method, however, is easily disturbed if this field is corrupted.
-   [Byte stuffing](https://en.wikipedia.org/wiki/Byte_stuffing "Byte stuffing") precedes the frame with a special byte sequence such as [DLE](https://en.wikipedia.org/wiki/Data_Link_Escape "Data Link Escape") [STX](https://en.wikipedia.org/wiki/Start_Of_Text "Start Of Text") and succeeds it with DLE [ETX](https://en.wikipedia.org/wiki/End-of-Text_character "End-of-Text character"). Appearances of DLE (byte value 0x10) have to be [escaped](https://en.wikipedia.org/wiki/Escape_sequence "Escape sequence") with another DLE. The start and stop marks are detected at the receiver and removed as well as the inserted DLE characters.
-   Similarly, [bit stuffing](https://en.wikipedia.org/wiki/Bit_stuffing "Bit stuffing") replaces these start and end marks with flags consisting of a special bit pattern (e.g. a 0, six 1 bits and a 0). Occurrences of this bit pattern in the data to be transmitted are avoided by inserting a bit. To use the example where the flag is 01111110, a 0 is inserted after 5 consecutive 1's in the data stream. The flags and the inserted 0's are removed at the receiving end. This makes for arbitrary long frames and easy synchronization for the recipient. The stuffed bit is added even if the following data bit is 0, which could not be mistaken for a [sync sequence](https://en.wikipedia.org/wiki/Sync_sequence "Sync sequence"), so that the receiver can unambiguously distinguish stuffed bits from normal bits.


#-2_data_link_layer/Byte_stuffing
#-2_data_link_layer/CSMA_CD
#-2_data_link_layer/frame_structure
#-2_data_link_layer/frame_synchronisation 


