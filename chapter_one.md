# Chapter One

## What's the internet?

### A service view

* Communication infrastructure
  * Enables distributed applications
  * Web, VoIP, email, games, e-commerce, social nets
* Communication services
  * provides programming interface to apps
  * hooks that allow sending and receiving app programs to "connect" to the internet
  * provides service options, analogous to postal service

### Nuts and Bolts View

* hosts or end systems
    * billions of connected devices running network apps
* communication links
    * fiber, copper, radio, satellite
* routers & switches
    * forwards packets (chunks of data)
* internet "network of networks"
    * Interconnected ISPs
* internet standards
    * IETF: Internet Engineering Task Force
    * RFC: Request for Comments
* IEEE for links/hardware
    * Ethernet, 802.11
* protocols
    * control sending, receiving of messages
    * TCP, IP, HTTP, Skype, 802.11

## What's a protocol?
* An established format of Communication
* Must understand the language. For example, English
* Human Example
    * H1: Hi
    * H2: Hi
    * H1: What is the time?
    * H2: 2:00
* Computer Example
    * TCP Connection Request
    * TCP Connection Response
    * Get `some_url`
    * Respond with `some_url`'s data

## Closer look at Structure
* Network edge
    * Your device, servers
* Access networks, physical media
    * Wired, wireless

## Access Networks
* Asks the question: How do we connect end systems to the edge router?

## The network core

**The** fundamental question: How is data transferred through the net?
* circuit-switching: dedicated circuit per call: telephone nets
* packet-switching: data send thru net in discrete "chunks"

## Packet-switching: Store and forward
* Takes L/R seconds to transpit L-bit packet into link at R bps
* _store and forward_ entire packet must arrive at router before it can be transmitted on next link
* end-end delay = 2L/R assuming zero propagation delay

Time between two endpoints is calculated by taking `L/R` and adding `d/s` where `L` is the number of bits in the packet, `R` is the number of bits the hardware can send per second, `d` is the distance and `s` is the speed a packet travels over the wire
