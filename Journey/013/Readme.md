<img width="800" height="557" alt="image" src="https://github.com/user-attachments/assets/df5fd275-8cb8-4831-9c99-9f4f21512d9e" /><!-- This is a template you can use for quick progress days. It removes a lot of the steps we encourage you to share in the longer template 000-DAY-ARTICLE-LONG-TEMPLATE.MD-->

# VLAN Part 2

## Trunk

<img width="1177" height="646" alt="image" src="https://github.com/user-attachments/assets/f5740626-9356-4f8f-ac71-5ffaa6ef596a" />



<img width="1202" height="680" alt="image" src="https://github.com/user-attachments/assets/da95bb6d-f2bf-4ede-9b35-ded682182f33" />


<img width="1192" height="648" alt="image" src="https://github.com/user-attachments/assets/b5ad1f1b-54de-466b-9a03-a835b2df96ce" />

<img width="1182" height="658" alt="image" src="https://github.com/user-attachments/assets/fd855df8-c1ea-4588-a547-cd81e9b2d81f" />

Native vlan mismatch

<img width="1198" height="673" alt="image" src="https://github.com/user-attachments/assets/2664887f-4efe-4253-bd77-3fe3a8fed1d1" />


Trunk Configuration:

- Topology

<img width="1207" height="668" alt="image" src="https://github.com/user-attachments/assets/d055bfbe-e8bd-47f5-bdb1-b47280af6f82" />

- Confguring g0/0 switch interface to trunk mode

<img width="1176" height="379" alt="image" src="https://github.com/user-attachments/assets/924547d7-faa6-4155-ae6c-9fdda8690b7e" />

- Make sure

<img width="777" height="603" alt="image" src="https://github.com/user-attachments/assets/e7a678b5-e04d-4b05-b928-03e24ea87245" />

- Adding another vlan

 <img width="1080" height="527" alt="image" src="https://github.com/user-attachments/assets/581a550f-ec82-49b7-9517-b83ae4e74145" />

- Changing native vlan

<img width="1114" height="554" alt="image" src="https://github.com/user-attachments/assets/efabbc8a-4549-4e9b-afd4-448e88948d0c" />

- Router configuration

  <img width="1184" height="560" alt="image" src="https://github.com/user-attachments/assets/50b2bbe8-1321-47e1-9702-c090e4ba8dae" />

- 
## Lab Practice

<img width="800" height="557" alt="image" src="https://github.com/user-attachments/assets/a6ae19ce-2eb4-4d25-9e87-034a93c7c165" />


**Switch 1 configuration**

- Access mode for switch interface directed to the pc
  
<img width="492" height="196" alt="image" src="https://github.com/user-attachments/assets/8da9fdd0-18b4-4039-8c2e-3e4a5d2c699b" />

- Trunk mode for switch interface directed to the SW2

<img width="777" height="343" alt="image" src="https://github.com/user-attachments/assets/e99ab30b-65ad-4ae2-b650-e9e74dcb9eb8" />


- vlan brief

<img width="671" height="260" alt="image" src="https://github.com/user-attachments/assets/db0f9337-5edd-4a8b-bb4e-0d6b318e13c8" />

**Switch 2 configuration**

- Access mode for switch interface directed to the pc

<img width="626" height="279" alt="image" src="https://github.com/user-attachments/assets/c9c38f76-e150-4771-8e26-8db7218e29c1" />

- Trunk mode for switch interface directed to R1

<img width="753" height="562" alt="image" src="https://github.com/user-attachments/assets/180f995c-43ec-4491-9e79-68fed0c84b40" />

- Creating vlan 30 in order that it appears

<img width="731" height="217" alt="image" src="https://github.com/user-attachments/assets/2e8a6e42-fa40-4e67-8efb-db440f687d7c" />

- Trunk mode for switch interface directed to SW 1

<img width="761" height="163" alt="image" src="https://github.com/user-attachments/assets/9b0a8b27-011b-4e5f-a14e-8f61b87270fb" />

**R1 Configuration**

- activate g0/0, create vlan 10,20,30 (set the dot1q) , set the ip address

<img width="794" height="638" alt="image" src="https://github.com/user-attachments/assets/6de33673-2a6c-4f88-817a-f1606155a33d" />

**Connection test from PC**

- From PC 7 (VLAN 10 on switch 2) to PC 1 (VLAN 10 on switch 1)

<img width="613" height="227" alt="image" src="https://github.com/user-attachments/assets/ee1a2748-9266-4eda-81da-75ff75db7d03" />

- PC 7 (VLAN 10) to PC 5 (VLAN 20)

<img width="616" height="236" alt="image" src="https://github.com/user-attachments/assets/6104f01a-02df-4637-b5f8-ce9c51b375af" />

- PC 7 (VLAN 10) to PC 3 (VLAN 30)

<img width="541" height="223" alt="image" src="https://github.com/user-attachments/assets/c6fddcf0-69f5-4e6e-8b57-29bac2b0aacc" />
