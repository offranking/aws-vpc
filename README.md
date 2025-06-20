# aws-vpc
AWS VPC - Private Cloud


This project demonstrates how to effectively utilize our VPC (Virtual Private Cloud) on AWS.
In this section, we focus on creating the VPC itself laying the foundation for secure, isolated networking within the AWS cloud. This step is essential for setting up resources like subnets, routing tables, and gateways, allowing us to manage traffic and network architecture with precision and flexibility.


<img width="1206" alt="Screenshot 2025-06-20 at 1 13 48 pm" src="https://github.com/user-attachments/assets/98211603-1403-48b1-ad17-fdf25766354d" />

Creating the VPC.

<img width="1424" alt="Screenshot 2025-06-20 at 1 19 55 pm" src="https://github.com/user-attachments/assets/ea7a9b2a-0e7a-4100-b94f-ffc095a45dd2" />
Seleteing "VPC" options and specify the IPv4 clock

<img width="1424" alt="Screenshot 2025-06-20 at 1 23 37 pm" src="https://github.com/user-attachments/assets/36604f20-8eeb-4e26-a00c-1f68228b9947" />

Here is the PVC i created.
<img width="1271" alt="Screenshot 2025-06-20 at 1 29 49 pm" src="https://github.com/user-attachments/assets/718089fa-f6d5-48b2-8357-cbde3cb94e1c" />

Select the ID of the PVC

<img width="1155" alt="Screenshot 2025-06-20 at 1 33 03 pm" src="https://github.com/user-attachments/assets/89f82118-0e13-41fc-9d47-82590036c8ea" />


In this section, I’m specifying the IPv4 CIDR block for the subnet, selecting the desired Availability Zone, and then clicking the “Add Subnet” button to include it in the VPC configuration.

<img width="1171" alt="Screenshot 2025-06-20 at 1 38 30 pm" src="https://github.com/user-attachments/assets/5fad6532-6d97-46b9-93e6-2eda54ea28a3" />

<img width="1171" alt="Screenshot 2025-06-20 at 1 43 10 pm" src="https://github.com/user-attachments/assets/7e1e7078-1c1f-4711-8523-c4d6b5ceedde" />

my subnet is being created

<img width="1191" alt="Screenshot 2025-06-20 at 3 20 51 pm" src="https://github.com/user-attachments/assets/9a968bfe-4d09-4ec4-bbdf-c64c1be5d78c" />

Navigate to the Internet Gateway section within the AWS VPC dashboard.
From here, you can create and manage an Internet Gateway, which is essential for enabling your VPC to connect to the internet. This step is crucial if you plan to allow public access to resources such as EC2 instances within your VPC.

<img width="1413" alt="Screenshot 2025-06-20 at 3 24 58 pm" src="https://github.com/user-attachments/assets/7c772678-b30d-49b6-a089-cdb8749ffa7f" />

my internet gateway is being successful created

<img width="1209" alt="Screenshot 2025-06-20 at 3 28 08 pm" src="https://github.com/user-attachments/assets/0c6416ba-7403-4cc2-8cb8-bfb0550d5ea0" />

To enable internet connectivity, you must attach the Internet Gateway to the VPC you previously created.
This step is essential for allowing resources within your VPC—such as EC2 instances—to access the internet and be accessible from outside. Attaching the gateway establishes a path for inbound and outbound traffic between your VPC and the web.

<img width="1209" alt="Screenshot 2025-06-20 at 3 30 54 pm" src="https://github.com/user-attachments/assets/986fb2b7-a9bc-437c-86c0-073947a920e1" />

<img width="1209" alt="Screenshot 2025-06-20 at 3 32 50 pm" src="https://github.com/user-attachments/assets/5abff9da-607c-49d2-800d-c2044f4b5055" />


Attach it to the VPC

<img width="1424" alt="Screenshot 2025-06-20 at 3 34 16 pm" src="https://github.com/user-attachments/assets/88f1671c-58ce-4123-aa26-c3f2acd59b82" />

<img width="1197" alt="Screenshot 2025-06-20 at 3 35 25 pm" src="https://github.com/user-attachments/assets/2b690898-1248-44db-b007-608d91da05b2" />


Finally, click on the Create  routing "button to proceed.

<img width="1430" alt="Screenshot 2025-06-20 at 3 39 01 pm" src="https://github.com/user-attachments/assets/52028402-5876-4106-8ee1-6d75c0b360f5" />

choose the public and click on save association


<img width="1421" alt="Screenshot 2025-06-20 at 3 46 20 pm" src="https://github.com/user-attachments/assets/bc93b65e-8cdb-400e-b77c-65372507a674" />

Navigate to Routes and click on Edit routes

<img width="1194" alt="Screenshot 2025-06-20 at 3 48 13 pm" src="https://github.com/user-attachments/assets/d0950258-b6c2-40a8-ac06-c6e567181719" />

click onadd route


<img width="1429" alt="Screenshot 2025-06-20 at 3 51 42 pm" src="https://github.com/user-attachments/assets/0f7a0fd9-32fe-484b-b2c4-a9a6c001d9be" />

Selete Destination as 0.0.0.0/0. indicationg that every Ipv4 address can access this subnet

<img width="1429" alt="Screenshot 2025-06-20 at 3 53 28 pm" src="https://github.com/user-attachments/assets/dfdb2b43-c50e-4eb9-a639-8d1f198467f7" />








