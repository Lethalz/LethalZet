# Subnetting

Subnetting:

  1. Classful:
  
  Classes A, B, C, D, and E:
  
*  Class A: Ranges from 0.0.0.0/8 to 127.0.0.0/8, designed to support extremely large networks with more than 16 million host addresses.
*  Class B: Ranges from 128.0.0.0/16 to 191.255.0.0, designed to support the needs of moderate to large size networks with up to approximately 65,000 host addresses.
*  Class C: Ranges from 192.0.0.0/24 to 223.255.255.0/24, designed to support small networks with a maximum of 254 hosts.
*  Class D: Multicast block consisting of 224.0.0.0 to 239.0.0.0.
*  Class E: Class E experimental address block consisting of 240.0.0.0-255.0.0.0.

  2. Classless:
  
   *  VLSM (Variable Length Subnet Mask): Allows a network space to be divided into unequal parts.
   *  CIDR (Classless Inter-Domain Routing) notation (IPv4 vs. IPv6): Is a way to allow more flexible allocation of Internet Protocol (IP) addresses than was possible with the original system of IP address classes.

/24 /16 /8 are the the classful subnets. The number determines how many numbers are part of the network ID.

So if you subnet to /25 your taking away another bit from the total 32 bits in a IP

`32-25` that equals 7 

So you have seven bits for hosts minus 2 for the Network id(lowest possible IP in subnet) abd the Broadcast ID (Highest possible IP in subnet)

## Converting Decimal to binary

|Value | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1|
|-------|----|----|----|----|----|----|----|----|

Using this Chart you can change decimal numbers to binary and vice versa
 
Highest number you can get in a byte (8bits) is 256

So lets take the number 69 and use the chart 

Does 69 go into 128? **No** So the Value of 128 is 0

|Value | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1|
|-------|----|----|----|----|----|----|----|----|
|Bit| 0 |

Does 69 go into 64? **yes** So `69-64`equals 5 so we have 5 bits left

Try to go through all the numbers with this method and youll get your final byte

|Value | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1|
|-------|----|----|----|----|----|----|----|----|
|Bit    | 0  |1   |0   |0   |0   | 1  |0   |1| 

5 Goes into 4 which means we have to turn on the bit then we had 1 left which didnt go into 2 but does go into 1

## Converting Binary to Decimal

Just use the same chart and punch in your byte

|Value | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1|
|-------|----|----|----|----|----|----|----|----|
|Bit    | 1  |0   |1   |1   |0   | 1  |0   |1| 

Then just use the value to add up to your decimal solution

`128+32+16+4+1` = 181 

So we know the decimal notation of this binary number is 181






