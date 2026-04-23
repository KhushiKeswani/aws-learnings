**Overview:**

Designed a custom virtual network on Amazon Web Services including subnets, routing, and traffic control using security layers.

**Architecture:**
Internet Gateway
      ↓
Public Subnet → EC2 (HTTP server)
      ↓
Route Table
      ↓
Security Group + NACL


**Step by Step guide:**

1. Created custom VPC
2. Configured public/private subnets
3. Attached Internet Gateway
4. Configured Route Tables
5. Launched EC2 inside subnet
6. Hosted HTTP server
7. Controlled traffic using:
        Security Groups
        Network ACLs

**Experiments Performed:**

1. Allowed HTTP → site accessible
2. Blocked port → site unreachable
3. Modified NACL rules → tested traffic behavior (on deny rule implementation in NACL even though security group is allowing, it won't be accessed)

**Screenshots:**

1. VPC creation
2. Subnet setup
3. NACL rules
4. Traffic flow diagram
5. Browser output

**Key Learnings:**

-> Difference between SG vs NACL
-> How traffic flows in cloud network
-> Subnet isolation
-> Real-world network debugging