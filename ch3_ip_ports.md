# 3. IP Addresses & Ports

## 3.1 IP Addresses, versions 4 and 6

|`IPv6` full address|Compressed address|
|-|-|
|Example 1:<br>`2001:0db8:c9d2:0012:0000:0000:0000:0051`|Remove leading zeros:<br>$\to$ `2001:db8:c9d2:12:0:0:0:51`<br><br>Compress consecutive `0`s: `0:0:0` $\to$ `::`<br>$\to$ `2001:db8:c9d2:12::51`|
|Example 2:<br>`2001:0db8:ab00:0000:0000:0000:0000:0000`|`2001:db8:ab00:0:0:0:0:0`<br><br>Longest zero sequence, compress to `::`:<br>$\to$ `0:0:0:0:0` $\to$ `:::::` $\to$ `::`<br><br>`2001:db8:ab00::`|
|Example 3<br>`0000:0000:0000:0000:0000:0000:0000:0001`|`::1`: This is a **loopback address**<br><br>In `IPv4`, loopback address is:<br>$\to$ `127.0.0.1`<br><br>IPv4: `192.0.2.33`<br>$\to$ IPV6: `::ffff:192.0.2.33`|

### 3.1.1 Subnets (Network vs Hosts)
|IP address|Network|Hosts|
|-|-|-|
|Example 1<br>`192.0.2.12`|**Network**: 3-bytes (first 3), eg:<br>`192.9.2.0`<br><br>Note: Zero out(`0`) host (4th byte)|**Host**: Last (4th) literal byte:<br>`0`<br>aka `8-bits` aka `256` hosts|
|`Class A` Network| **Network**: One-byte |**Host**: 3 bytes, aka 24-bits of hosts, thats alot of of hosts for you, `16 million` hosts!|

### 3.1.2 Port Numbers


## 3.2 Byte Order

## 3.3 `struct` S

## 3.4 IP Addresses, Part Deux

### 3.4.1 Private (Or Disconnected) Networks