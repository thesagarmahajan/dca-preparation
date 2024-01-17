### Setting up swarm on AWS EC2
Step-1: Create security group
Inbound rules:
  - HTTP:80 FROM Anywhere
  - SSH: 22 FROM Anywhere
  - TCP:2377, 7946, and 4789 FROM Anywhere
    
Step-2: Create EC2 instances withgiven shell script
```bash
#!/bin/bash
yum update -y
yum install -y docker
systemctl start docker
chkconfig docker on
```
