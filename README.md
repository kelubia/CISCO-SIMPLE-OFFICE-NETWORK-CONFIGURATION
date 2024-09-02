# CISCO-SIMPLE-OFFICE-NETWORK-CONFIGURATION


REQUIREMENTS:
- design multiple end host for two departments (Delivery and Accounting) on two separate subnets
- Assign appropriate number of Routers and Switches to the Network
- Configure subnet mask, Gateways and IP Address-192.168.40.0 
- Test connectivity between ACCOUNTS AND DELIVERY departments end hosts 
- End hosts in DELIVERY departments should be able to ping and transfer data to the ACCOUNTS department.

# Network Address= 192.168.40.0
# No. of subnets= 2
# 2^n= No. of Subnets == 2^n=2
# n=1 (the 1 variable represents the number of borrowed Network bits)

255.255.255.255
11111111.11111111.11111111.10000000 = /25
255.255.255.128 = SUBNET MASK

SUBNET-MASK   BLOCK-SIZE
128--------------128
192--------------64
224--------------32
240--------------16
248--------------8
252--------------4
254--------------2
255--------------1

1st subnet
-----------------------------------------------------------------------
Subnet Mask = 255.255.255.128
network ID = 192.168.40.0
Range of Valid Host= 192.168.40.1 - 192.168.40.126
broadcast ID= 192.168.40.127


2nd subnet
-----------------------------------------------------------------------
Subnet Mask = 255.255.255.128
network ID = 192.168.40.128
Range of Valid Host= 192.168.40.129 - 192.168.40.254
broadcast ID= 192.168.40.255

![1](https://github.com/user-attachments/assets/5f361923-9b25-4895-aed5-420c37309a31)


# configure Router Default Gateway interface IP address
# Router= 192.168.40.1

![2](https://github.com/user-attachments/assets/c8fb1249-9d3c-4acb-adc4-4e9f667d8e18)
![3](https://github.com/user-attachments/assets/ee7e4aa6-8284-45e0-a072-3886ce39ac78)


# Assign IP address to ACCOUNTS SUBNET End-host and test communication 

![4](https://github.com/user-attachments/assets/66fd0351-7b9c-4f87-9cd4-37b0ac4744e7)
![5](https://github.com/user-attachments/assets/660535c5-eea8-4ced-8980-8c522b302f46)
![6](https://github.com/user-attachments/assets/aa95c4f9-cc86-4d29-be80-bb38860622ec)




# Assign IP address to DELIVERY SUBNET End-host and test communication 

![7](https://github.com/user-attachments/assets/d2aac450-6d8e-4295-be94-d7e1d5be42da)
![8](https://github.com/user-attachments/assets/59e3d9d4-5875-408b-b732-363eae248e1a)
![9](https://github.com/user-attachments/assets/de1b9744-5725-415c-84f6-bb0bde67a052)



# Test communication btw Accounts - Delivery
[PING] Accounts (PC0) - Delivery (PC2)

![10](https://github.com/user-attachments/assets/14f31fcb-312c-4c68-9c50-744b57504c64)

[PING] Accounts (PC1) - DELIVERY (Printer)

![11](https://github.com/user-attachments/assets/371036f9-0781-4916-a705-4b5e76e4d27b)


[PING] DELIVERY (PC2) - Accounts (Printer) 

![12](https://github.com/user-attachments/assets/8c7f41e4-34e7-48e4-8221-7e05763511ce)


[PING] DELIVERY (PC3) - Accounts (PC0) 
### 12

