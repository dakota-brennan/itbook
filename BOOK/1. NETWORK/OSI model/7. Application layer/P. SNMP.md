IT VAULT
NETWORK CHAPTER
SIMPLE NETWORK MANAGEMENT PROTOCOL

#-7_application_layer/SNMP

It stands for <mark style="background: #FFB86CA6;">Simple Network Management Protocol</mark>. It gathers data by polling the devices on the network from a <mark style="background: #FF5582A6;">management station</mark> at fixed or random intervals, requiring them to disclose certain information.
It is a way that servers can share information about their current state, and also a channel through which an administrate can modify <mark style="background: #FF5582A6;">pre-defined values</mark>. 
<mark style="background: #ADCCFFA6;">Port 161 - TCP</mark> 
<mark style="background: #ADCCFFA6;">Port 162 - UDP</mark> 

#-7_application_layer/SNMP/port_161
#-7_application_layer/SNMP/port_162

 
	COMMAND
snmpget -mALL -v1 -cpublic snmp_agent_Ip_address sysName.0

@ https://www.geeksforgeeks.org/protocols-application-layer/

It consists of a set of standards for <mark style="background: #FF5582A6;">network management</mark> including:
- an application layer protocol
- a database schema
- a set of data objects
 ``

	FUNCTION
SNMP is used to:
- collect 
- organize the <mark style="background: #FF5582A6;">data</mark> of <mark style="background: #FF5582A6;">managed devices</mark> on<mark style="background: #ADCCFFA6;"> IP networks</mark> 
- modifies the information to change the behavior of the devices
- monitor and manage the network (main function)

@ https://www.educba.com/application-layer-protocols/