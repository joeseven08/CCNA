<!-- This is a template you can use for quick progress days. It removes a lot of the steps we encourage you to share in the longer template 000-DAY-ARTICLE-LONG-TEMPLATE.MD-->

# VLAN Part 3: Multilayer Switch

## Configuring Native VLAN on a Router

<img width="1171" height="505" alt="image" src="https://github.com/user-attachments/assets/28033bf8-76fe-4594-b4da-8b3555ac2836" />

<img width="1179" height="536" alt="image" src="https://github.com/user-attachments/assets/f64407df-aa5b-41d5-ad92-0140aab0ec8b" />

## Multilayer Switching

### Icon

<img width="1116" height="507" alt="image" src="https://github.com/user-attachments/assets/af3364cb-f754-4fa3-92bc-369bf7db831c" />

### Definition

<img width="1163" height="644" alt="image" src="https://github.com/user-attachments/assets/1dbbb842-3b22-45b5-84df-3b3cf351eb90" />

### Topology example

<img width="1173" height="586" alt="image" src="https://github.com/user-attachments/assets/76a88c82-e77c-47d8-8917-df4aaa5723fa" />


### SVI (Switch Virtual Interface)

<img width="1186" height="539" alt="image" src="https://github.com/user-attachments/assets/ab749b70-3618-4fed-b8a1-d7d89ee90566" />



## Lab
<img width="840" height="607" alt="image" src="https://github.com/user-attachments/assets/ae3d1b46-b067-41ea-a661-459da372c543" />

### Step 1
- Check R1 interface

<img width="713" height="181" alt="image" src="https://github.com/user-attachments/assets/7d522e06-0ac0-4242-af1e-9411ea73f8ab" />

- Delete g0/0.10, g0/0.20, g0/0.30

<img width="691" height="184" alt="image" src="https://github.com/user-attachments/assets/79621748-6e0d-4eb1-8644-bf242f06aa30" />

- Configure the IP address on g0/0

<img width="519" height="64" alt="image" src="https://github.com/user-attachments/assets/f2dd4da7-df39-4714-8686-0ce58f045c5f" />

- Go to the switch and set default configuration for the trunk cable directed to R1

<img width="703" height="200" alt="image" src="https://github.com/user-attachments/assets/d45c4a95-2d20-4c31-aa32-f610aff0c60c" />

- Add an ip address to g1/0/2 by make the inteface enter no switchport

<img width="641" height="353" alt="image" src="https://github.com/user-attachments/assets/b1e29d4b-dd36-4340-abff-7ac365325acb" />

- Configure the default route

<img width="693" height="271" alt="image" src="https://github.com/user-attachments/assets/eeb1ffe9-7700-455b-925f-45e15636a191" />

*Make sure the ip routing command has been done.

<img width="717" height="305" alt="image" src="https://github.com/user-attachments/assets/de285c0e-16f6-4cc4-af35-daee7950f2db" />


### Step 2: Configure the SVI on SW2

- Add ip address in each vlan by first enable the int / svi (switch virtual interface)
<img width="730" height="302" alt="image" src="https://github.com/user-attachments/assets/7a866bcd-1c19-4d62-8ab1-7b9ca56799af" />

- Make sure the vlan is in up/up state

<img width="704" height="281" alt="image" src="https://github.com/user-attachments/assets/9358ba06-76c3-412a-a74a-12aa234c8ab5" />

- Test ping from PC7 to PC3

<img width="674" height="419" alt="image" src="https://github.com/user-attachments/assets/445a9820-7250-4378-b6fd-4e79b638f066" />

- Test ping from PC7 to the internet

<img width="669" height="219" alt="image" src="https://github.com/user-attachments/assets/8a708aaf-9f95-4690-8823-d9f91d07d6b2" />



