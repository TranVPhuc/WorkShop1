---
title : "Web Server Structure"
date : "`r Sys.Date()`"
weight : 2
chapter : false
pre : " <b> 2.2. </b> "
---

#### Web Server Structure

In Amazon Web Services (AWS), you can deploy a web server structure in various ways, depending on your specific needs and the AWS services you want to use. Here's a common approach to deploy a web server structure on AWS:
![ws-structure](/images/2.2-ws-structure/simplewsstructure.png?featherlight=false&width=55pc)
The structure of a web server can be divided into the following basic components:
1. **EC2 (Elastic Compute Cloud)**:
> * The core component, responsible for processing requests and sending back results to users..
> * Can be configured according to requirements for CPU, RAM, storage capacity, etc
> * Common operating systems: Amazon Linux 2, Ubuntu Server, Windows Server.
> * irewall configuration to allow HTTP (port 80) and HTTPS (port 443) connections to the instance.

2. **RDS (Relational Database Service)**:
> * If your web application requires a database, you can use RDS to deploy relational databases such as MySQL, PostgreSQL, or SQL Server.
> * RDS provides features such as automatic backups, scalability based on demand, and data security.

3. **IAM (Identity and Access Management**):

> * Manage access permissions to AWS resources using IAM to ensure that only authorized users can access your resources.

4. **Auto Scaling và Elastic Load Balancing**:

> * Use Auto Scaling to automatically adjust the number of EC2 instances based on application demand.
> * Use Elastic Load Balancing to distribute traffic between EC2 instances and increase application scalability.
