
# Socket

File Descriptor: an **integer** associated with an **open file**

File can be:
- network connection
- FIFO
- pipe
- terminal
- Everything in UNIX is a file

Call `socket()` system routine:
- returns: **socket descriptor**
- communciate via: `send()` & `recv()`

|Sockets|Types|Example|How|
|-|-|-|-|
|**Internet** Sockets|Stream Sockets: `SOCK_STREAM`<br>- reliable two-way connected comm streams<br>- error-free<br>|`telnet`, `ssh`<br><br>Web browsers use HTTP which uses stream coekts to get pages<br>`DARPA` Intenet addresses|High level data transmission quality via:<br>- `TCP` or `Tranmission Control Protocol`|
|**Internet** Sockets|Datagram Sockets: `SOCK_DGRAM` (or connectionless sockets)<br><br>Connectionless means do not have to maintain **open connection** (compared to stream sockets)|3 things:<br>- build a packet<br>- put IP header (with dest info)Other applications<br><br>- `tftp`<br>- `dhcpcd` (DHCP client)<br>- multiplayer games, streaming audio, video conf etc|Uses `IP` or `Internet Protocol` for routing<br><br> `UDP` or `User Datagram Protocol`|

|**Unix** Sockets|asdf|Path names on a local node|||

