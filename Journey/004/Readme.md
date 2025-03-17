<!-- This is a template you can use for quick progress days. It removes a lot of the steps we encourage you to share in the longer template 000-DAY-ARTICLE-LONG-TEMPLATE.MD-->

# Intro to the CLI & Basic Device Security: Day 4

## Intro to the CLI
- Command Line Interface : the interface you use to configure Cisco
- How to connect to a cisco device: use rollover cable
- User EXEC mode, Priviledge EXEC mode, Global Configuration mode
- enable password, service password-encryption, secret
- show configuration
- save configuration

## Lab: Basic Security Device
![image](https://github.com/user-attachments/assets/641bea80-8e50-492d-ba53-b79e56e0a072)

1.Change the hostnames of the router and switch to the appropriate names (R1, SW1)
     ##Use the 'hostname' command in global configuration mode##
     
Router>enable

Router#conf t

Enter configuration commands, one per line.  End with CNTL/Z.

Router(config)#hostname R1

2.  Configure an unencrypted enable password of 'CCNA' on both devices
R1(config)#enable password CCNA

3. Exit back to user EXEC mode and test the password
R1>enable
Password: 
R1#

4.  View the password in the running configuration
R1#show run
Building configuration...

Current configuration : 711 bytes
!
version 15.1
no service timestamps log datetime msec
no service timestamps debug datetime msec
no service password-encryption
!
hostname R1
!
!
!
enable password CCNA
!
!
!
!
!
!
ip cef
no ipv6 cef

5. Ensure that the current password, and all future passwords, are encrypted
R1#conf t
Enter configuration commands, one per line.  End with CNTL/Z.
R1(config)#service pass
R1(config)#service password-encryption 

6. View the password in the running configuration
R1(config)#do show run
Building configuration...

Current configuration : 716 bytes
!
version 15.1
no service timestamps log datetime msec
no service timestamps debug datetime msec
service password-encryption
!
hostname R1
!
!
!
enable password 7 08026F6028
!
!
!

7. Configure a more secure, encrypted enable password of 'Cisco' on both devices
R1(config)#enable secret Cisco

8. Exit back to user EXEC mode and then return to privileged EXEC mode.
    Which password do you have to use?
R1>enable
Password: 
Password: 
R1#

The successful password is the password from secret.

9. View the passwords in the running configuration.
     What encryption type number is used for the encrypted 'enable password'?
     What encryption type number is used for the encrypted 'enable secret'?

hostname R1
!
!
!
enable secret 5 $1$mERr$YlCkLMcTYWwkF1Ccndtll.
enable password 7 08026F6028
!



10. Save the running configuration to the startup configuration
R1#write
Building configuration...
[OK]

## Youtube Vids

[Intro to the CLI](https://www.youtube.com/watch?v=IYbtai7Nu2g&list=PLxbwE86jKRgMpuZuLBivzlM8s2Dk5lXBQ&index=8)

[Basice Device Security](https://www.youtube.com/watch?v=SDocmq1c05s&list=PLxbwE86jKRgMpuZuLBivzlM8s2Dk5lXBQ&index=9)

