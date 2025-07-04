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

the route table has noow been configured

<img width="1206" alt="Screenshot 2025-06-20 at 3 58 24 pm" src="https://github.com/user-attachments/assets/aab61e69-8ec6-41b2-a071-4ff7924514b6" />


Navigate to the NAT Gateway section and click on the create NAt Gateway

<img width="1412" alt="Screenshot 2025-06-20 at 3 59 36 pm" src="https://github.com/user-attachments/assets/759b8b2e-b6c1-4fbc-bdfd-9d0c6f45a097" />
chose the private.

<img width="1415" alt="Screenshot 2025-06-20 at 4 01 24 pm" src="https://github.com/user-attachments/assets/59865973-38d6-4bfe-a928-1a1e25cc4a41" />

<img width="1391" alt="Screenshot 2025-06-20 at 4 05 03 pm" src="https://github.com/user-attachments/assets/b6859230-1f89-49c0-b869-1db7e75a22ed" />


Your NAT Gateway has been created sucessfully

<img width="1209" alt="Screenshot 2025-06-20 at 4 06 18 pm" src="https://github.com/user-attachments/assets/d34ce73f-95aa-4da4-a479-063a37dbe90c" />

edit your subnet association 


<img width="644" alt="Screenshot 2025-06-20 at 4 43 11 pm" src="https://github.com/user-attachments/assets/873ce1bd-bb6c-4560-b7e7-aab0ff484dec" />

Now, provide a name for both your VPC and the peering connection in AWS.
Naming your resources helps keep your network infrastructure organized, especially when managing multiple VPCs and connections. A descriptive name makes it easier to identify the purpose of each component at a glance.

<img width="693" alt="Screenshot 2025-06-20 at 4 39 25 pm" src="https://github.com/user-attachments/assets/9398ddae-e04f-438b-a66a-180962d24f0c" />

Then you will see  this 


<img width="644" alt="Screenshot 2025-06-20 at 4 43 11 pm" src="https://github.com/user-attachments/assets/abcdac6f-1c8e-4136-801c-4c7e8dc7f38a" />

<img width="644" alt="Screenshot 2025-06-20 at 4 43 33 pm" src="https://github.com/user-attachments/assets/35f182d6-f2c0-4684-9343-87cb993a83f0" />

Now you can accept.

<img width="463" alt="Screenshot 2025-06-20 at 4 44 20 pm" src="https://github.com/user-attachments/assets/7eb04a9d-ed31-4748-967e-390f0f246aaa" />

now click on main route table ID of the accpeter VPC

<img width="645" alt="Screenshot 2025-06-20 at 4 45 50 pm" src="https://github.com/user-attachments/assets/3d754999-5bfc-4cec-a99c-ef56e2d6eb22" />

choose the route table

<img width="646" alt="Screenshot 2025-06-20 at 4 47 31 pm" src="https://github.com/user-attachments/assets/24ba24cf-e91d-459c-a730-27efec2353f8" />

add route 
<img width="646" alt="Screenshot 2025-06-20 at 4 47 31 pm" src="https://github.com/user-attachments/assets/fd568aa7-352a-452a-81c7-3172a1be45b2" />


Go to PVC and selete request.

<img width="646" alt="Screenshot 2025-06-20 at 4 52 00 pm" src="https://github.com/user-attachments/assets/a622387c-2ddd-496d-8cc4-258099243f2d" />

choose the table , then navigate to the routes and click edit route.

<img width="646" alt="Screenshot 2025-06-20 at 4 57 31 pm" src="https://github.com/user-attachments/assets/97748d95-08df-475f-b40e-ce285d674a9d" />
