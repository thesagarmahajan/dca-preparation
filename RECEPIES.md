### Setting up swarm on AWS EC2
Shellscript to setup docker in EC2
```bash
yum update -y
yum install -y docker
systemctl start docker
chkconfig docker on
```
