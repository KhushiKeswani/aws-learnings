**Overview:**

This project demonstrates deployment of a CI server using Jenkins on a cloud VM and resolving real-world setup issues including dependency mismatches and resource constraints.

Architecture:
Local Machine → SSH → EC2 → Jenkins (Port 8080)

**Steps Performed:**

1. Launched EC2 instance
2. Configured Security Groups (port 22, 8080)
3. Installed Java (required by Jenkins)
4. Installed Jenkins and started service
5. Accessed Jenkins dashboard via public IP
6. Retrieved and configured admin credentials

**Challenges Faced:**

1. Jenkins failed to start → fixed Java version issue
2. Disk space issues → debugged /tmp constraints
3. Port access issues → corrected security group rules

**Screenshots:**

EC2 instance running
Jenkins dashboard
Terminal setup

**Key Learnings:**

-> Understanding of CI/CD tools like Jenkins
-> Linux debugging (services, logs, ports)
-> Cloud deployment fundamentals
-> Handling real-world infra issues