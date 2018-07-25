# TCP-IP-Protocols

### What is a communication protocol?
Is a set of rules or sintaxis that allows two or more systems communicate and share data between them.

Each message has a specific meanning, intended to obtain a response from a range of possible predetermined responses for that particular situation.

### What is TCP-IP protocol?
TCP/IP provides end-to-end connectivity specifying how data should be formatted, addressed, transmitted, routed and received at the destination.

### How a TCP segment looks like?
![alt text](http://hcarrasco.cl/apps/protocols/tcp-model-segment.png)

We abstract from the header, using any modern programming language and work directly on the content of the "data" section

### My communication protocols 

As you can see, my protocols are embeded in the TCP-IP protocol in the data section.

I use it in two diferent ways based in a common structure:

##### 1) String based message:
I use it when data sended in segments will be  of variable length.

![alt text](http://hcarrasco.cl/apps/protocols/string-segment.png)

finnal message: ```<hc-ptcls;10010;temperature=30;speed=70;color=green;>```

##### 2) Bytes based message:
I use it when data sended in segments will be always of a constant length.

How we can't see the bytes, we represent the message as hexadecimal representation. Modern programming lenguajes provides functions to make this transformation (bytes to hex) easely. You can help you with a ascii table :)

![alt text](http://hcarrasco.cl/apps/protocols/bytes-segment.png)

finnal message: ```48432D5054434C5331303031313033303730303530391020```