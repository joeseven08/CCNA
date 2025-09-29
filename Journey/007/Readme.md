<!-- This is a template you can use for quick progress days. It removes a lot of the steps we encourage you to share in the longer template 000-DAY-ARTICLE-LONG-TEMPLATE.MD-->

# Switch Interfaces
## Network Topology

<img width="1177" height="584" alt="image" src="https://github.com/user-attachments/assets/5b8d483d-ffcf-4969-a037-ceedecf2b4f2" />

For this lesson, we use layer 2 switch. No IP asssigned to the switch.

## Show ip interface brief on switch

<img width="1166" height="593" alt="image" src="https://github.com/user-attachments/assets/ef3265d3-9cda-4599-8aab-20a506f4ab55" />

Here is the status in the switch of layer 2. The status is up and up because there is a device connected while down and down because there is no interface connected to the switch. There is no need to make the switch up.

## show interfaces status
<img width="1184" height="526" alt="image" src="https://github.com/user-attachments/assets/0c54ea2c-d0d3-4c4e-b1a0-2000c5c6e01f" />

- Duplex refers to how data is transmitted and received over a network link. It determines whether communication between two network devices happens in one direction at a time or both directions simultaneously.
1. Half Duplex

Data can only travel in one direction at a time.

Similar to a walkie-talkie: either you talk, or you listen — not both at once.

Characteristics:

- Older technology, common in hubs and very old switches.
- More collisions can occur since only one device can send data at a time.
- Lower performance than full duplex.

2. Full Duplex

Data can travel in both directions simultaneously.

Like a phone call: you can speak and listen at the same time.

Characteristics:

- Higher performance.
- No collisions because both devices have a dedicated send and receive path.
- Standard for modern Ethernet networks.

3. Auto (Default)

The switch negotiates the best duplex setting automatically with the connected device using Auto-Negotiation.

Best option if both devices support it.

Potential issue:

If one side is set to auto and the other side is set manually to full or half, a duplex mismatch can occur, leading to:

- Slow performance
- High error counts (like CRC errors or collisions)

Additional information:

<img width="1170" height="568" alt="image" src="https://github.com/user-attachments/assets/db78a9f7-e5bb-43d2-bbe2-948dddc48180" />

Collision will occur if:

<img width="1171" height="658" alt="image" src="https://github.com/user-attachments/assets/53a4d398-5536-4223-bf74-31ed27ac4425" />



## Configuring interface speed and duplex
<img width="1173" height="605" alt="image" src="https://github.com/user-attachments/assets/fc1041eb-081e-4175-a4b2-0dc1cf903a75" />


