<!-- This is a template you can use for quick progress days. It removes a lot of the steps we encourage you to share in the longer template 000-DAY-ARTICLE-LONG-TEMPLATE.MD-->

# Subnetting: Day 13 to Day 15
## Things covered
- CIDR (Classless Inter-Domain Routing)
- The process of subnetting
- FLSM (Fixed-Length Subnet Masks)
- VLSM (Variable-Length Subent Masks)

### CIDR

- When the internet was first created, the creators did not predict that the internet would become as large as it is today.
- This resulted in wasted address space.
- The IETF (Internet Engineering Task Force) introduced CIDR in 1993 to replace the 'classful' addressing system.
- With CIDR, the requirement of..

Class A = /8

Class B = /16

Class C = /24

... were removed.

- This allowed larger networks to be split into smaller networks, allowing greater efficiency.
- These smaller networks are called 'subnetworks' or 'subnets'.

### Counting on how many usable addresses per subnet

![image](https://github.com/user-attachments/assets/3bc68851-0538-4104-a0f0-3aa0e1ee90c2)

### FLSM 

All of subnets use the same prefix length (ie. subnetting a class c network into 4 subnets using /26).

### VLSM

The process of creating subnets of different sizes, to make your use of network more efficient. Below is the example:

![image](https://github.com/user-attachments/assets/0f78b6bd-f955-40d3-ba5e-ceb273654373)

*The steps:*

1. Assign the largest subnet at the start of the address space.
2. Assign the second largest after it.
3. Repeat the process until all subnets have been assigned.

So, here is the result.

![image](https://github.com/user-attachments/assets/455bed01-7d33-4bf2-ae94-0ddba2b25b8b)


## Lab

![image](https://github.com/user-attachments/assets/f303f2d7-204c-40ce-b922-4abb4f779e7d)
