<!-- This is a template you can use for quick progress days. It removes a lot of the steps we encourage you to share in the longer template 000-DAY-ARTICLE-LONG-TEMPLATE.MD-->

# The Life of a Packet: Day 10

## Things covered

- The entire process of sending a packet to a remote destination
- Including ARP, encapsulation, de-encapsulation, etc.

### ARP (ChatGPT)

ARP stands for Address Resolution Protocol. It's a fundamental protocol in computer networking, specifically used in IPv4 networks.

What ARP Does:

ARP maps a device's IP address (logical address) to its MAC address (physical address), which is needed for devices to communicate on a local area network (LAN).

How ARP Works (Simple Example):

Let’s say Computer A wants to send data to Computer B on the same network:

Computer A knows the IP address of Computer B but not its MAC address.

It sends an ARP request to the network:

“Who has IP 192.168.1.20? Tell 192.168.1.10.”

Computer B (which owns that IP) responds with an ARP reply:

“192.168.1.20 is at AA:BB:CC:DD:EE:FF.”

Now Computer A can send frames directly to Computer B using its MAC address.



## The process

![image](https://github.com/user-attachments/assets/fbe42bdc-6431-4cbf-a059-57a12490ab05)


Goal: PC1 wants to ping PC4 and static routing has been set like above.

Process:
1. PC1 to R1

  ARP Request

  ![image](https://github.com/user-attachments/assets/e8d83224-ca55-4b08-9c3e-a79311d738ff)

     
  ARP Reply

![image](https://github.com/user-attachments/assets/3580b482-af88-49d9-8c35-a8a7c839afc2)
     
3. R1 to R2

ARP request

![image](https://github.com/user-attachments/assets/31433a45-7d06-4e3f-bd3d-19f1768700d9)


ARP Reply

![image](https://github.com/user-attachments/assets/6dfb28a4-b76d-4506-a6c4-ad0d9fae566e)

4. R2 to R4

ARP request

![image](https://github.com/user-attachments/assets/8cbfd293-527d-4a35-8c22-393c0e6d6699)

ARP reply

![image](https://github.com/user-attachments/assets/e941eb29-c228-4086-8c5a-31f6ef1a4dd9)

5. R4 to PC4

ARP request

![image](https://github.com/user-attachments/assets/53c16dd7-7a1b-4204-b149-7ebb00bef52c)

ARP reply

![image](https://github.com/user-attachments/assets/2558f2a0-c304-407a-bed0-4515ea9107c4)


## Lab

[Twitter](https://twitter.com/_notwaving/status/1327785265092579328?s=20)
