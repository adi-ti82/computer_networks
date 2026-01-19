# 4.1. Bandwidth
- a potential measurement of data transfer.
- Bandwidth ia the maximum data-carrying capacity of a communication channel per unit time.

### Two different measuring values: 
- 1) Bandwidth in Hertz: 
  - tells how wide the frequency pipe is.
  - Basically, range of frequency a signal or channel occupies.
  - Bandwidth(Hz) = f<sub>high</sub> - f<sub>low</sub>
  
  
- 2) Bandwidth in bits/sec:
   - tells how much daat flows through the pipe.
   - number of bits transmitted per sec.
 
     
### Units:
- bps: bits per sec
- Kbps: kilobits per sec
- Mbps: megsbits per sec
- Gbps: gigabits per sec

###Examples:
- 100 Mbps bandwidth means:- up to 100 million bits can be transmitted per sec through the channel.

### Explain like a five:-
-Analogy is similar like more water can cross through a thick pipe at a time but only a little through thin one.
- In our case, water is the data packets and pipe is communication channel like wire, fiber cable or even air.
- So, Bandwidth is the maximum amount of data packets (water) that can cross the channel at a time.
- The more the data (water) flow the higher is the bandwidth.

### Isn't it a fact that air is huge (infinite), then why are we limited to 10Mbps or 100 Mbps etc?
### Understand:-
- Data isn't sent directly throught air, we uses EM waves to do so.
- Data is converted to Radio waves, which uses specific frequency bands and these bands are finite.

### We are limited to a fixed capacity because:
- 1) more frequency width = more bandwidth but Spectrum is finite.
- 2) Noise is there in air and it limits how much data we can safely pack.
- 3) Shared Medium, more users less bandwidth per user.
 

# Relationship: 
  - an increase in bandwidth in hertz means an increase in bandwidth in bits per second

# 4.2 Throughput
 - Actual measurement of how fast we can send data over a network.
 -  'Throughput'  is always less than or equal to 'Bandwidth'.

### Why less than Bandwidth: 
  - Noise and Errors
      - Noise corrupts bits and corrupted bits are retransmitted.
  - Proptocol Overhead:
      - Data packet has ( consume bandwidth but do not carry user data)
          - headers
          - control messages (???)
  - Hardware and Software limits
  - Conestion and Collisions.
  - etc.

### Example: 
- A link has a bandwidth of 1 Mbps, but the devices connected to the end of the link may handle only 200 kbps

# Latency (Delay)
- how long it takes for an entire message to completely arrive at the destination from the time the first bit is sent out from the source.
- Latency = propagation time + transmission time + queuing time + processing delay

  ### i) Propagation time:
   - time required for a bit to travel from the source to the destination.
   - Propagation time = Distance / (Propagation Speed)
   - The propagation speed of electromagnetic signals depends on the medium and on the frequency of the signal.

 ### ii)Transmission time:
   - a time between the first bit leaving the sender and the last bit arriving at the receiver.
   - Transmission time = (Message size in bit) / Bandwidth

### iii) Queuing Time
   - the time needed for each intermediate or end device to hold the message before it can be processed.
   - The queuing time is not a fixed factor; it changes with the load imposed on the network. When there is
     heavy traffic on the network, the queuing time increases. An intermediate device, such
     as a router, queues the arrived messages and processes them one by one.
     
### iv) Processing delay:
 - The time intermediate device (like router) takes to process the packet header.

   
            



