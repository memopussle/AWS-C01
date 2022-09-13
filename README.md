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

![Point of Presence](img/aws-console.png)

### Shared Responsibility Model diagram
![Point of Presence](img/response-diagram.png)

