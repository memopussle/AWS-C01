# Cloud Computing

## How Website Works

![how website works](img/website-work.png)

### What is a server composed of

![how website works](img/server-compose.png)

### IT Terminology

- Network: cables, routers and servers connected with each other
- Router: A networking device that forwards data packets between computer networks. They know where to send your packets on the internet!
- Switch: Takes a packet and send it to the correct server / client on your network

### Cloud Computing

- Cloud computing is the on-demand delivery of compute power, database storage, applications, and other IT resources
- Through a cloud services platform with **pay-as-you-go pricing**
- You can access as many resources as you need, almost **instantly**
- Simple way to access servers, storage, databases and a set of **application services**

#### AWS owns and maintains the network-connected hardware required for these application services, while you provision and use what you need via a web application.

### the Deployment Models of the Cloud

<table>
<tr>
    <td>Private Cloud</td>
    <td>Cloud services used by a
single organization, not
exposed to the public.</td>
    <td>Complete control</td>
    <td>Security for sensitive
applications</td>
    <td>Meet specific business
needs</td>
   <td>ex: rackspace</td>
</tr>
<tr>
    <td>Public Cloud</td>
    <td>Cloud resources owned
and operated by a third-
party cloud service provider delivered over
the Internet.</td>
   <td> Six Advantages of Cloud
Computing</td>
   <td>ex: Dropbox, AWS, GoogleCloud</td>
</tr>
<tr>
    <td>Hybrid Cloud</td>
    <td>Keep some servers on
premises and extend
some capabilities to the
Cloud</td>
     <td>Control over sensitive
assets in your private
infrastructure</td>
     <td>Flexibility and cost-
effectiveness of the
public cloud</td>
     <td>ex: your own database -> <- AWS</td>
</tr>
</table>

![Cloud models](img/modelsCloud.png)

### 5 Characteristics of Cloud Computing

| On-demand self service                                                                        | Broad network access                                                                                       | Multi-tenancy and resource pooling                                                                                                                      | Rapid elasticity and scalability                                                                                              | Measured service                                                        |
| --------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| Users can provision resources and use them without human interaction from the service provide | <ul><li>Resources available over the network</li><li>can be accessed by diverse client platforms</li></ul> | Multiple customers can share the same infrastructure and applications with security and privacy.Customers are serviced from the same physical resources | <ul> <li>Automatically and quickly acquire and dispose resources when needed</li><li>Quickly and easily scale based on demand | Usage is measured</li></ul> users pay correctly for what they have used |

### 6 Advantages of Cloud Computing

| Trade capital expense (CAPEX) for operational expense (OPEX)                                                                   | Benefit from massive economies of scale                        | Stop guessing capacity               | Increase speed and agility  | Stop spending money running and maintaining data centers | Go global in minutes                   |
| ------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------- | ------------------------------------ | --------------------------- | -------------------------------------------------------- | -------------------------------------- |
| <ul><li>Pay On-Demand: don’t own hardware</li><li>Reduced Total Cost of Ownership (TCO) & Operational Expense (OPEX)</li></ul> | Prices are reduced as AWS is more efficient due to large scale | Scale based on actual measured usage | Increase speead and agility | Stop spending money running and maintaining data centers | leverage the AWS global infrastructure |

### Types of Cloud Computing

<table>
  <tbody>
    <tr>
      <th>Infrastructure as a Service (IaaS)</th>
      <th align="center"> Platform as a Service (PaaS)</th>
      <th align="right">Software as a Service (SaaS)</th>
    </tr>
    <tr>
      <td>
      <ul>
        <li>Provide building blocks for cloud IT</li>
        <li>Provides networking, computers, data storage space</li>
        <li>Highest level of flexibility</li>
          <li> Easy parallel with traditional on-premises IT</li>
      <ul>
      </td>
      <td align="center">
        <ul>
        <li>Removes the need for your organization to manage the underlying infrastructure</li>
        <li>Focus on the deployment and management of your applications</li>
      <ul>
      </td>
      <td align="right">Completed product that is run and managed by the service provider</td>
    </tr>
  </tbody>
</table>

![comparison in cloud computing](img/comparison-types-compute-clouding.png)

![types of cloud-computing](img/example-types-cloud--computing.png)

### Pricing of the Cloud - Quick Overview
- AWS has 3 pricing fundamentals, following pay-as-you-go pricing model
- **Compute:**Pay for compute time
- **Storage:**Pay for data stored in the Cloud
- **Data transfer OUT of the Cloud:**Data transfer IN is free
- Solves the expensive issue of traditional IT

## AWS Overview

### Cloud History
![Cloud history](img/example-types-cloud--computing.png)

### AWS Cloud Use Cases
- AWS enables you to build sophisticated, scalable applications
- Aplicable to a diverse set of industries
- Use cases include
  + Enterprise IT, backup & storage, Big data analytics,
  + Web hosting, Mobile & Social Apps

#### AWS Global Infrastructure
- AWS Regions
- AWS Availability Zones
- AWS Data Centers
- AWS Edge Locations /
Points of Presence

-> checkout infrastructure.aws

### AWS Regions
- AWS has Regions all around the world
- Names can be us-east-1, eu-west-3...
- A region is a **cluster of data centers**
- **Most AWS services are region-scoped**.So if you switch region, it will be refreshed

### How to choose AWS region
- Compliance with data governance and legal
requirements: data never leaves a region without
your explicit permission
- Proximity to customers: reduced latency. If you use different target region -> lagging
- Available services within a Region: new services
and new features aren’t available in every Region
-Pricing: pricing varies region to region and is
transparent in the service pricing page

| Compliance with data governance and legal requirements| Proximity to customers  | Available services within a Region    |Pricing   |
| :---:   | :---: | :---: |:---: |
data never leaves a region without your explicit permission | reduced latency (reduce lag)  | new services and new features aren’t available in every Region   |pricing varies region to region and is transparent in the service pricing page   |

### Availablity zones
- Each region has many (usually 3, min is 2, max is 6). Example:
  + ap-southeast-2a
  + ap-southeast-2b
  + ap-southeast-2c

- Each availability zone (AZ) is one or more
discrete data centers with redundant power,
networking, and connectivity
-They’re separate from each other, so that
they’re isolated from disasters
- They’re connected with high bandwidth,
ultra-low latency networking

![Availability Zones](img/AZ-availabilityzones.png)

### AWS Points of Presence (Edge Locations)
- Amazon has 216 points of presence (205 Edge Locations & || Regional Caches) in 84 cities across 42 countries
- Content is delivered to end users with lower latency

![Point of Presence](img/point-presence.png)

### Tour of AWS Console

![Tour of AWS Console](img/aws-console.png)

### Shared Responsibility Model diagram
![Shared Responsibility Model diagram](img/response-diagram.png)


## IAM - Users & Groups
- AM = Identity and Access Management, Global service
- Root account created by default, shouldn’t be used or shared
- Users are people within your organization, and can be grouped

- **Groups only contain users, not other groups**
- Users don’t have to belong to a group, and user can belong to multiple groups

![IAM groups](img/IAM-groups.png)

### IAM: Permissions
- Users or Groups can be
assigned JSON documents
called policies
- These policies define the permissions of the users
- In AWS you apply the least privilege principle: don’t give more permissions than a user needs. Ex: users can use uneccessary services-> cost and not secured

![IAM permissions](img/IAM-permissions.png)

### IAM Policies inheritance
![Policy inheritance - IAM](img/policies-inheritance.png)

### IAM Policies Structure

- Consist of:
  + Version: policy language version, always include "2012-10-17"
  + Id: an identifier for the policy
  + Statement: one or more individual statements (required)
    + Sid: an identifier for the statement
    + Effect: whether the statement allows or denies access (Allow, Deny)
    + Principal: account/user/role to which this policy applied to
    + Action: list of actions this policy allows or denies
    + Resource: list of resources to which this actions applied to
    + Condition: conditions for when this policy is in effect (optional)

  ![Policy Structure](img/policy-structure.png)

### Password Policy
- Strong passwords = higher security for your account
  - In AWS, you can setup a password policy:
  - Set a minimum password length
  - Require specific character types:
    - including uppercase letters
    - lowercase letters
    - numbers
    - non-alphanumeric characters
- Allow all IAM users to change their own passwords
- Require users to change their password after some time (password expiration)
- Prevent password re-use

### Multi Factor Authentication - MFA
- Users have access to your account and can possibly change configurations or delete resources in your AWS account
- **You want to protect your Root Accounts and IAM users**

 ![MFA](img/mfa.png)

- Main benefit of MFA: **if a password is stolen or hacked, the account is not compromised**

### MFAA devices options in AWS
 ![mfa options](img/mfa-options.png)

### How can users access  AWS?
- To access AWS, you have three options:
  - AWS Management Console (protected by password + MFA)
  - AWS Command Line Interface (CLI): protected by access keys
  - AWS Software Developer Kit (SDK) - for code: protected by access keys
- Access Keys are generated through the AWS Console
- Users manage their own access keys
- Access Keys are secret, just like a password. Don’t share them
- Access Key ID ~= username
- Secret Access Key ~= password

#### AWS CLI
- A tool that enables you to interact with AWS services using commands in
your command-line shell
- Direct access to the public APIs of AWS services
- You can develop scripts to manage your resources
- It’s open-source https://github.com/aws/aws-cli
- Alternative to using AWS Management Console

 ![Point of Presence](img/mfa-options.png)
 
### AWS SDK
- AWS Software Development Kit (AWS SDK)
- Language-specific APIs (set of libraries)
- Enables you to access and manage AWS services
programmatically
- Embedded within your application
- Supports
  + SDKs (JavaScript, Python, PHP, .NET, Ruby, Java, Go, Node.js,
C++)
  + Mobile SDKs (Android, iOS, …)
  + IoT Device SDKs (Embedded C, Arduino, …)

- AWS CLI is built on AWS SDK for Python

### IAM Roles for Services
- Some AWS service will need to perform actions on your behalf
- To do so, we will assign permissions to AWS services
with IAM Roles
- Common roles:  
  + EC2 Instance Roles 
  + Lambda Function Roles 
  + Roles for CloudFormation 
  
  ![Policy Structure](img/IAM-roles.png)

### IAM Security Tools
 - IAM Credentials Report (account-level)
   + a report that lists all your account's users and the status of their various
credentials

 - IAM Access Advisor (user-level)
   + Access advisor shows the service permissions granted to a user and when those
services were last accessed.
   + You can use this information to revise your policies

### IAM Guidlines & Best Practices

- Don't use the root account except for AWS account setup
- One physical user = One AWS user
- Assign users to groups and assign permissions to group
- Create a strong password policy
- Use and enforce the use of Multi Factor Authentication (MFA)
- Create and use Roles for giving permissions to AWS services
- Use Access Keys for Programmatic Access (CLI / SDK)
- Audit permissions of your account with the IAM Credentials Report
- Never share IAM users & Access Keys

### Shared Responsibilitiy Model for IAM

  ![Shared Responsibilitiy Model for IAM](img/shared-reponse-IAM.png)

## Summary - IAM Section
 
 - **Users**: mapped to a physical user, has a password for AWS Console
 - **Groups**: contains users only
 - **Policies**: JSON document that outlines permissions for users or groups
 - **Roles**: for EC2 instances or AWS services
 - **Security**: MFA + Password Policy
 - **AWS CLI**: manage your AWS services using the command-line
 - **AWS SDK**: manage your AWS services using a programming language
 - **Access Keys**: access AWS using the CLI or SDK
 - **Audit**: IAM Credential Reports & IAM Access Advisor
 
 
### EC2 Instance Storage Section
- An EBS (Elastic Block Store) Volume is a network drive you can attach to your instances while they run
- It allows your instances to persist data, even after their termination
- They can only be mounted to one instance at a time (at the CCP level)
- They are bound to a specific availability zone
- Analogy: Think of them as a “network USB stick” 
- Free tier: 30 GB of free EBS storage of type General Purpose (SSD) or Magnetic per month

### EBS Volume
-  It’s a network drive (i.e. not a physical drive)
    - It uses the network to communicate the instance, which means there might be a bit of latency
    - It can be detached from an EC2 instance and attached to another one quickly
- It’s locked to an Availability Zone (AZ)
  - An EBS Volume in us-east-1a cannot be attached to us-east-1b
  - To move a volume across, you first need to snapshot it
- Have a provisioned capacity (size in GBs, and IOPS)
  - You get billed for all the provisioned capacity
  - You can increase the capacity of the drive over time

### EBS Overview

  ![EBS Volume - Example](img/EBS%20Volume.png)

### EBS – Delete on Termination attribute

 ![EBS- Delete on Termination attribute](img/EBS%20-%20Delete%20on%20Termination.png)

- Controls the EBS behaviour when an EC2 instance terminates
  - By default, the root EBS volume is deleted (attribute enabled)
  - By default, any other attached EBS volume is not deleted (attribute disabled)
- This can be controlled by the AWS console / AWS CLI
- **Use case: preserve root volume when instance is terminated**

### EBS Snapshots
- Make a backup (snapshot) of your EBS volume at a point in time
- Not necessary to detach volume to do snapshot, but recommended
- Can copy snapshots across AZ or Region

![EBS snapshots](img/ebs%20snapshots.png)

### EBS Snapshots 
- EBS Snapshot Archive
  - Move a snapshot to an "archive tier" that is 75% cheaper
  - Takes within 24 to 72 hours for restoring the archive

- Recycle Bin for EBD Snapshots
  - Setup rules to retain deleted snapshots so you can recover them after an accidental deletion
  - Specify retention (from 1 day to 1 year)

### AMI Overview
- AMI = Amazon Machine Image
- **AMI are a customization of an EC2 instance**
 - You add your own software, configuration, operating system, monitoring…
 - Faster boot / configuration time because all your software is pre-packaged
 - AMI are built for a specific region (and can be copied across regions)
 - You can launch EC2 instances from:
   - A Public AMI: AWS provided
   - Your own AMI: you make and maintain them yourself
   - An AWS Marketplace AMI: an AMI someone else made (and potentially sells)

![AMI](img/ami.png)

### EC2 Image Builder
- Used to automate the creation of Virtual Machines or container images
- => Automate the creation, maintain, validate and test EC2 AMIs
- Can be run on a schedule (weekly, whenever packages are updated, etc…)
- Free service (only pay for the underlying resources)

![EC2 Image Builder](img/ec2-image-builder.png)

### EC2 Instance Store
- EBS volumes are network drives with good but “limited” performance
- If you need a high-performance hardware disk, use EC2 Instance Store
- Better I/O performance
- EC2 Instance Store lose their storage if they’re stopped (ephemeral)
- Good for buffer / cache / scratch data / temporary content
- Risk of data loss if hardware fails
- Backups and Replication are your responsibility 

### Local EC2 Instance Store (high performance hardware attached volume)
![EC2 instance store](img/ec2-instance-store.png)

### EFS - Elastic File System
- Managed NFS (network file system) that can be mounted on 100s of EC2
- EFS works with Linux EC2 instances in multi-AZ
- Highly available, scalable, expensive (3x gp2), pay per use, no capacity planning

![ EFS - Elastic File System](img/efs.png)

### Difference between EBS vs EFS

![EBS vs EFS](img/ebs%20vs%20efs.png)

| EBS    |EFS |
| ----------- | ----------- |
| To transfer EBS to different AZ, you have to make a copy of it (EBS snapshot),  and restore that copy to wanted AZ     | EFS makes a shared file system. All instances in AZs and mount the same EFS file |

### Shared Responsibility Model for EC2 Storage
|AWS   |User|
| ----------- | ----------- |
| <ul><li>Infrastructure</li><li>Replication for data for EBS volumes & EFS drives</li><li>Replacing faulty hardware</li><li>Ensuring their employees cannot access your data</li></ul>    | <ul><li>Setting up backup / snapshot procedures</li><li>Setting up data encryption</li><li>Responsibility of any data on the drives</li><li>Understanding the risk of using EC2 Instance Store</li></ul>    |

### Amazon FSx – Overview 
- Launch 3rd party high-performance file systems on AWS
- Fully managed service. ex: FSx for Lustre, FSx for Windows File Server, FSx for NetApp ONTAP

### Amazon FSx for windows File Server
- A fully managed, high reliable, and scalable **Windows native** shared file system
- Built on Windows File Server
- Supports SMB protocol & Windows NTFS
- Integrated with Microsoft Active Directory
- Integrated with Microsoft Active Directory
- Can be accessed from AWS or your on-premise infrastructure


![Amazon FSx](img/fsc.png)

### Amazon FSx for Lustre
- A fully managed, high-performance, scalable file storage for High Performance Computing (HPC)
- The name Lustre is derived from “Linux” and “cluster”
- Machine Learning, Analytics, Video Processing, Financial Modeling, …
- Scales up to 100s GB/s, millions of IOPS, sub-ms latencies

![Amazon FSx Lustre](img/fsx-lustre.png)

### EC2 Instance Storage - Summary
- EBS volumes:
  - Network drives attached to one EC2 instance at a time
  - Mapped to an Availability Zones 
  - Can use EBS Snapshots for backups / transferring EBS volumes across AZ 
- AMI: create ready-to-use EC2 instances with our customizations
- EC2 Image Builder: automatically build, test and distribute AMIs
- EC2 Instance Store: 
  - High performance hardware disk attached to our EC2 instance 
  - Lost if our instance is stopped / terminated
- EFS: network file system, can be attached to 100s of instances in a region
- EFS-IA: cost-optimized storage class for infrequent accessed files 
- FSx for Windows: Network File System for Windows servers
- FSx for Lustre: High Performance Computing Linux file system