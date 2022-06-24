
# COM03-AWS100 - Launch a Hello World website on the internet

<p align="center">
<img src="https://user-images.githubusercontent.com/80279467/175496844-5d681f47-2bb0-46f0-b873-9794c6adaa96.jpeg"  ></p>

## Introduction

✍️ We use cloud in diversely and one of the main application of cloud is hosting websited on it so that we can access them fast and easily with no interruptions. 
## Prerequisite

✍️ we need to know about EC2 , Region , Availability zone, Subnets, AMIs, security groups, inbound/outbound rules, ect

## Cloud Research

- What is a region?  
 AWS has the concept of a Region, which is a physical location around the world where we cluster data centers. We call each group of logical data centers an        Availability Zone. Each AWS Region consists of multiple, isolated, and physically separate AZs within a geographic area.
- What is an availability zone? 
Availability Zones — An Availability Zone (AZ) is one or more discrete data centers with redundant power, networking, and connectivity in an AWS Region.
- What is a public subnet? 
A public subnet is a subnet that's associated with a route table that has a route to an internet gateway. A private subnet with a size /24 IPv4 CIDR block (example:     10.0. 1.0/24). This provides 256 private IPv4 addresses
- How many subnets can there be in one region? 
 1000
- How to launch EC2 instances in public / private subnets? 
In the AWS Management Console in the search box to the right of  Services, choose Compute and then choose EC2.
Note: Verify that your EC2 console is currently managing resources in the N. Virginia (us-east-1) region.  You can verify this by looking at the drop down menu at the top of the screen, to the left of your username. If it does not already indicate N. Virginia, choose the N. Virginia region from the region menu before proceeding to the next step.
Choose Launch instances 
- What are AMIs? 
An Amazon Machine Image (AMI) provides the information required to launch an instance, which is a virtual server in the cloud. An AMI includes:
A template for the root volume for the instance (for example, an operating system or an application server with applications)
Launch permissions that control which AWS accounts can use the AMI to launch instances
A block device mapping that specifies the volumes to attach to the instance when it is launched
- What are security groups? 
A security group acts as a virtual firewall for your EC2 instances to control incoming and outgoing traffic. Inbound rules control the incoming traffic to your instance, and outbound rules control the outgoing traffic from your instance. When you launch an instance, you can specify one or more security groups. If you don't specify a security group, Amazon EC2 uses the default security group. You can add rules to each security group that allow traffic to or from its associated instances. You can modify the rules for a security group at any time. New and modified rules are automatically applied to all instances that are associated with the security group. When Amazon EC2 decides whether to allow traffic to reach an instance, it evaluates all of the rules from all of the security groups that are associated with the instance.
- What are inbound/outbound rules? 
Inbound rules filter traffic passing from the network to the local computer based on the filtering conditions specified in the rule. Conversely, outbound rules filter traffic passing from the local computer to the network based on the filtering conditions specified in the rule.

## Cloud Service Provider
- Amazon Web Services

## Difficulty
- Level 100 (Introductory)

## Estimated Time
- One to Two hours. 

## Project's Author(s)

[Syed Auther](https://twitter.com/syedauther)

## Objectives

### You need to complete the following:
- Launch a linux based EC2 instance in any one region of your choice in a public subnet 
- Setup a security group that allows http/https connections from the Internet, and ssh from your IP address
- ssh into the EC2 instance
- setup a webserver on the EC2 instance
- add a simple hello world header to the index.html file 
- Hit the public IP address from a browser and confirm the site is served


## References
- [What Is Amazon EC2?](https://aws.amazon.com/ec2/faqs/)
- [Security Groups](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-security-groups.html#:~:text=A%20security%20group%20acts%20as,one%20or%20more%20security%20groups.)
- [Installing httpd](http://httpd.apache.org/docs/2.4/install.html)
- [ssh into ec2 - linux](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AccessingInstancesLinux.html)

## Ideas
- For windows users [Download and install Putty](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)
- Connecting to a Linux EC2 instance from Windows is not possible natively, you will need an ssh client such as Putty to connect , and you will need to follow these steps to [ssh into ec2 from windows](https://stackoverflow.com/questions/5264945/ssh-to-ec2-linux-instance-from-windows)
- You can also launch non linux EC2 instances for example windows servers, for which you will need to RDP into.  

## Tips
- Use t2.micro instances from the free tier as it will suffice for this static site 
- Use the default setting on the storage screen as 8GB of EBS storage will be enough for this project.
