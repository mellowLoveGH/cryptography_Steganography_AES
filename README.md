# cryptography_Steganography_AES
use python, for steganography, conceal message within a file (image here). AES, baby block to encode &amp; decode AES



For AES:

Blocks, Bytes and Nibbles 
A block is 8 bits (or one byte, or one ASCII character). A key is 8 bits (or one byte). A block is treated as consisting of four nibbles, each nibble being two bits. 
 
A block is 8 bits: 1 2 3 4 5 6 7 8. 
 
Nibbles are: 1 2,     3 4,     5 6,     7 8. 
 
A nibble can be treated either as two bits or as a number in arithmetic modulo 4 (that is, a number in the range 0−3). 


Worked Example 1 
Block 132                    10 00 01 00 
Key 84                       01 01 01 00 
XOR block and key            11 01 00 00 
Swap last 2 nibbles          11 01 00 00 
S-Box                        01 00 10 10 
Key                          01 01 01 00 
XOR Block & Key              00 01 11 10 
Subtract 2nd 2 from 1st 2    01 11 11 10 
Swap last 2 nibbles          01 11 10 11 
S-Box                        00 01 11 01 
Key                          01 01 01 00 
XOR Block & Key              01 00 10 01 
 
Answer: 73, i.e. 'I'. 
