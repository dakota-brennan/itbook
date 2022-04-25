IT VAULT
NETWORK CHAPTER
EXTERNAL DATA REPRESENTATION PROTOCOL

#-6_presentation_layer/XDR

<mark style="background: #FF5582A6;">External Data Representation (XDR)</mark> is <mark style="background: #FFF3A3A6;">the standard</mark> for the <mark style="background: #FFB86CA6;">description</mark> and <mark style="background: #FFB86CA6;">encoding</mark> of <mark style="background: #BBFABBA6;">data</mark>. 
It is useful for transferring <mark style="background: #BBFABBA6;">data</mark> between computer architectures and has been used to communicate data between very diverse machines.
Converting from local representation to XDR is called encoding, whereas converting XDR into local representation is called decoding.

		-Data types
The XDR <mark style="background: #FF5582A6;">data format</mark> <mark style="background: #FFB86CA6;">is in use</mark> by many <mark style="background: #BBFABBA6;">systems</mark>, including:

-   [Network File System (protocol)](https://en.wikipedia.org/wiki/Network_File_System_(protocol) "Network File System (protocol)")
-   [ZFS](https://en.wikipedia.org/wiki/ZFS "ZFS") File System
-   [NDMP](https://en.wikipedia.org/wiki/NDMP "NDMP") Network Data Management Protocol
-   [Open Network Computing Remote Procedure Call](https://en.wikipedia.org/wiki/Open_Network_Computing_Remote_Procedure_Call "Open Network Computing Remote Procedure Call")
-   [Legato NetWorker](https://en.wikipedia.org/wiki/EMC_NetWorker "EMC NetWorker") backup software (later sold by EMC)
-   [NetCDF](https://en.wikipedia.org/wiki/NetCDF "NetCDF") (a scientific data format)
-   The [R language and environment for statistical computing](https://en.wikipedia.org/wiki/R_programming_language "R programming language")
-   The [HTTP-NG](http://www.w3.org/Protocols/HTTP-NG/http-ng-status.html) [Binary Wire Protocol](https://en.wikipedia.org/w/index.php?title=Binary_Wire_Protocol&action=edit&redlink=1 "Binary Wire Protocol (page does not exist)")
-   The [SpiderMonkey](https://en.wikipedia.org/wiki/SpiderMonkey_(Javascript_engine) "SpiderMonkey (Javascript engine)") JavaScript engine, to serialize/deserialize compiled JavaScript code
-   The [Ganglia](https://en.wikipedia.org/wiki/Ganglia_(software) "Ganglia (software)") distributed monitoring system
-   The [sFlow](https://en.wikipedia.org/wiki/SFlow "SFlow") network monitoring standard
-   The [libvirt](https://en.wikipedia.org/wiki/Libvirt "Libvirt") virtualization library, [API](https://en.wikipedia.org/wiki/Application_Programming_Interface "Application Programming Interface") and [UI](https://en.wikipedia.org/wiki/User_Interface "User Interface")
-   The [Firebird (database server)](https://en.wikipedia.org/wiki/Firebird_(database_server) "Firebird (database server)") for Remote Binary Wire Protocol
-   [Stellar Payment Network](https://en.wikipedia.org/wiki/Stellar_(payment_network) "Stellar (payment network

		-XDR Data types
-   [boolean](https://en.wikipedia.org/wiki/Boolean_datatype "Boolean datatype")
-   int – 32-bit [integer](https://en.wikipedia.org/wiki/Integer_(computer_science) "Integer (computer science)")
-   unsigned int – unsigned 32-bit [integer](https://en.wikipedia.org/wiki/Integer_(computer_science) "Integer (computer science)")
-   hyper – 64-bit [integer](https://en.wikipedia.org/wiki/Integer_(computer_science) "Integer (computer science)")
-   unsigned hyper – unsigned 64-bit [integer](https://en.wikipedia.org/wiki/Integer_(computer_science) "Integer (computer science)")
-   [IEEE](https://en.wikipedia.org/wiki/IEEE_754 "IEEE 754") [float](https://en.wikipedia.org/wiki/Floating_point "Floating point")
-   IEEE [double](https://en.wikipedia.org/wiki/Double_precision "Double precision")
-   [quadruple](https://en.wikipedia.org/wiki/Quadruple_precision "Quadruple precision") (new in RFC1832)
-   [enumeration](https://en.wikipedia.org/wiki/Enumerated_type "Enumerated type")
-   [structure](https://en.wikipedia.org/wiki/Record_(computer_science) "Record (computer science)")
-   [string](https://en.wikipedia.org/wiki/String_(computer_science) "String (computer science)")
-   fixed length [array](https://en.wikipedia.org/wiki/Array_data_structure "Array data structure")
-   variable length [array](https://en.wikipedia.org/wiki/Array_data_structure "Array data structure")
-   [union](https://en.wikipedia.org/wiki/Tagged_union "Tagged union") – discriminated union
-   fixed length [opaque](https://en.wikipedia.org/wiki/Opaque_data_type "Opaque data type") data
-   variable length [opaque](https://en.wikipedia.org/wiki/Opaque_data_type "Opaque data type") data
-   [void](https://en.wikipedia.org/wiki/Void_type "Void type") – zero byte quantity
-   optional – optional data is notated similarly to C pointers, but is represented as the data type "pointed to" with a boolean "present or not" flag. Semantically this is [option type](https://en.wikipedia.org/wiki/Option_type "Option type").

@ https://en.wikipedia.org/wiki/External_Data_Representation

#-6_presentation_layer/XDR/NFS
#-6_presentation_layer/binary_wire_protocol
#-6_presentation_layer/data_format
#-6_presentation_layer/data_types
#-6_presentation_layer/Firebird
#-6_presentation_layer/Ganglia
#-6_presentation_layer/HTTP-NG
#-6_presentation_layer/Legato_NetWorker
#-6_presentation_layer/libvirt
#-6_presentation_layer/libvirt/API
#-6_presentation_layer/libvirt/UI
#-6_presentation_layer/NetCDF
#-6_presentation_layer/Remote_binary_wire_protocol
#-6_presentation_layer/R_language_and_environment_for_statistical_computing
#-6_presentation_layer/sFlow
#-6_presentation_layer/SpiderMonkey
#-6_presentation_layer/Stellar_network_payment_system
#-6_presentation_layer/ZFS
