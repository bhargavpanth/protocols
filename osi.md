# OSI Model

I am going to briefly discuss the OSI model and what each of the layers are ultimately responsible for, from a backend/software engineer's perspective. I am not a network engineer by profession but I believe that a reasonable understanding of the protocol stack and their responsibilities will go a long way in helping us becoming better.

## What is the OSI model?

The *Open System Interconnection* or OSI (for short) forms the backbone of the internet as we know and use today. This model serves as an abstraction that is implemented on different computer systems running over the internet to communicate with one another.

## Why should you care as a backend engineer about the OSI model?

Think of the OSI as the framework on which the internet operates on. Gaining an understanding at a high level will help you in analysing what's going on underneath your application code.

## Layers of the OSI model

The OSI model consists of 7 layers. Starting from the underlying physical connections (Physical layer) up until the point where we handle HTTP requests (Application layer). Here's a quick summary of what each of the layers are responsible for (again, from a backend engineer's perspective). Think of this model as the Matrayoshka doll.

### Physical layer

This is the first layer (rather the layer furthest away from what a backend engineer could be bothered with) in the OSI model. The purpose of this layer is to transport the packets by converting it into bits (electric signals). On the whole, this layer is so far away for any practical purposes, you will find very little to no need in understanding the specifics. Often, any opportunity for improvement at this layer is a result of specific knowledge (maybe for a network engineer).

I might preface that one of the things you may way to know is that the Network Interface Controller/Network Card (NIC) sits in this layer. When a packet is sent to your machine, it is the job of the NIC to fetch the packet and check if it's meant to be sent to you or not.

Like I mentioned, there is very little for a backend engineer to do at this layer. No particular bottlenecks can be easily diagnosed with backend engineering skill-sets. Although, for those who are interested in packet sniffing or doing some kind of security testing, it might be worth deep diving a little bit more.

### Datalink layer

This layer sits right above the Physical layer. From the TCP/IP perspective, this layer can be thought of as the abstraction responsible for fetching the MAC address for a given IP address. This typically is done with the help of protocols such as Address Resolution Protocol (ARP) and Reverse Address Resolution Protocol (RARP) for incoming packets.

This layer is again slightly far from a backend developer and anyone wishing to build application at the top most layer, may find no use understanding.

### Network layer
### Transport layer
### Session layer
### Presentation layer
### Application layer
