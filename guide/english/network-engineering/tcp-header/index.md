---
title: TCP Header
---
## TCP Header Format

The Transfer Control Protocol (TCP) is is one of the commonly used protocols in the Internet Protocol (IP) suite along with [UPD](https://guide.freecodecamp.org/network-engineering/udp-header) 

The TCP uses a header as part of packaging data to be transferred through the network, below is a table with the TCP header fields, and their explanation. 

![TCP Header](https://66.media.tumblr.com/653f8c823065419f47a187519c0a18e9/tumblr_pssncuvMRP1vwzlb5o1_540.png)

  1 - Source Port (16 bits): The port of the application on the device sending the data  
  2 - Destination Port (16 bits): The port of the application on the device receiving the data  
  3 - Sequence Number (32 bits): Used to identify the segment's data  
  4 - Acknowledgement Number (32 bits): Sequence number of next byte expected from the other side  
  5 - Data Offset (4 bits): Specifies the length of the header, therefore pointing at where the data starts   
  6 - Reserved (4 bits): Not used, always set to zero  
  7 - Flags (8 bits): Use to mark specific things about the data such as beginning and end of session  
  8 - Receive Window (16 bits): Specifies the number for bytes the receiver is willing to accept   
  9 - Checksum (16 bits): Used for error checking the header and data  
 10 - Urgent Data Pointer (16 bits): Indicates the offset from the current sequence number, where the segment of non-urgent data begins  
 11 - Options (Variable Length): includes TCP options, such as Maximum Segment Size (MSS) or Window Scaling  
 12 - Application Data (Variable Length) 

#### More Information:
- Computer Networking a Top Down Approach: http://www-net.cs.umass.edu/kurose-ross-ppt-6e/  
- TCP Header Explained https://www.lifewire.com/tcp-headers-and-udp-headers-explained-817970


