# week2-cloud-vpc-subnets
Custom VPC setup with public/private subnets, route tables, and IGW &amp; NAT Gateway

## 🔧 What I Did
- Created custom VPC
- Designed public/private subnets
- Configured route tables
- Set up NAT Gateway
- Verified EC2 connectivity

## 📸 Screenshots
### VPC Creation
![VPC Creation](screenshots/vpc-creation.png)

### Public Subnet
![Public Subnet](screenshots/public-subnet.png)

### Private Subnet
![Private Subnet](screenshots/private-subnet.png)

### Route Table (Public)
This route table is associated with my public subnet and includes a route to the Internet Gateway, enabling outbound internet access.
![Route Table Public](screenshots/route-table-public.png)

### Route Table (Private)
This route table is associated with my private subnet and includes a route to the NAT Gateway, allowing outbound internet access without exposing the subnet directly.
![Route Table Private](screenshots/route-table-private.png)

### NAT Gateway
This NAT Gateway is deployed in a public subnet and enables instances in the private subnet to access the internet securely.
![NAT Gateway](screenshots/nat-gateway.png)

### Internet Gateway
This Internet Gateway is attached to the VPC and enables internet access for resources in the public subnet.
![Internet Gateway](screenshots/internet-gateway.png)
