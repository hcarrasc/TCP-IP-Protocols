# Communication Protocols

### What is a communication protocol?
Is a set of rules or sintaxis that allows two or more systems communicate and share data between them.

Each message has a specific meanning, intended to obtain a response from a range of possible predetermined responses for that particular situation.

### What is TCP-IP protocol?
TCP/IP provides end-to-end connectivity specifying how data should be formatted, addressed, transmitted, routed and received at the destination.

### How a TCP segment looks like?

<img src="http://hcarrasco.cl/apps/protocols/tcp-model-segment.png" width="450" height="208"/>

We abstract from the header, using any modern programming language and work directly on the content of the "data" section

### My Internet communication protocols:

As you can see, my protocols are embeded in the TCP-IP protocol in the data section.

I use it in two diferent ways based in a common structure:

##### 1) String based message:
I use it when data sended in segments will be  of variable length.

<img src="http://hcarrasco.cl/apps/protocols/string-segment.png" width="250" height="422"/>

finnal message: ```<hc-ptcls;10010;temperature=30;speed=70;color=green;>```

##### 2) Bytes based message:
I use it when data sended in segments will be always of a constant length.

How we can't see the bytes, we represent the message as hexadecimal representation. Modern programming lenguajes provides functions to make this transformation (bytes to hex) easely. You can help you with a ascii table :)

<img src="http://hcarrasco.cl/apps/protocols/bytes-segment.png" width="350" height="230"/>

finnal message: ```48432D5054434C5331303031313033303730303530391020```

### Bluetooth Protocols

The wireless data exchange standard Bluetooth uses a variety of protocols. Core protocols are defined by the trade organization Bluetooth SIG. Additional protocols have been adopted from other standards bodies [[wikipedia.org](https://en.wikipedia.org/wiki/List_of_Bluetooth_protocols)]

##### Logical link control and adaptation protocol (L2CAP): 
It passes packets to either the Host Controller Interface (HCI) or on a hostless system, directly to the Link Manager/ACL link.


### Space Communication Protocols

NASA article: [nasa.gov](https://www.nasa.gov/centers/ames/research/technology-onepagers/secure_space_communication.html)

Communication protocol standards for space data systems: [Proceedings of the IEEE](https://ieeexplore.ieee.org/document/56941/) (Volume: 78, Issue: 7, **Jul 1990**)

##### Disruption Tolerant Networking: 
Communicating from Earth to any spacecraft is a complex challenge, largely due to the extreme distances involved. When data are transmitted and received across thousands and even millions of miles, the delay and potential for disruption or data loss is significant. Delay/Disruption Tolerant Networking (DTN) is NASA’s solution to reliable internetworking for space missions. [nasa.gov](https://www.nasa.gov/content/dtn)

##### Protocols used by Curiosity land rover

CCSDS.org: [Blue Books](https://public.ccsds.org/publications/BlueBooks.aspx)




