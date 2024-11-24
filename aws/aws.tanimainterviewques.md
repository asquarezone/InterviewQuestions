1). What is AWS?

Amazon Web Services (AWS) provides on-demand computing resources and services in the cloud, with pay-as-you-go pricing.

For example, you can run a server on AWS that you can log on to, configure, secure, and run just as you would a server that's sitting in front of you


2). What you can do with AWS?

Store public or private data.
Host a static website. These websites use client-side technologies (such as HTML, CSS, and JavaScript) to display content that doesn't change frequently. A static website doesn't require server-side technologies (such as PHP and ASP.NET).
Host a dynamic website or web app. These websites include classic three-tier applications, with web, application, and database tiers.
Support students or online training programs.
Process business and scientific data.
Handle peak loads.

AWS Questions
AWS Questions


3). What is the Security group?

A security group acts as a virtual firewall for your instance to control inbound and outbound traffic. You can specify one or more security groups when you launch your instance.

When you create a security group, you add rules that control the inbound traffic that's allowed, and a separate set of rules that control the outbound traffic.



All other traffic is discarded. You can modify the rules for a security group at any time and the new rules are automatically enforced


4). What is Amazon Route 53?


Amazon Route 53 is a highly available and scalable cloud Domain Name System (DNS) web service. It is designed as an extremely reliable and cost-effective way to route visitors to websites by translating domain names (such as www.example.com) into the numeric IP addresses (such as 192.0.2.1) that computers use to connect to each other.


AWS assigns URLs to your AWS resources, such as your EC2 instances.



However, you might want a URL that is easy for your users to remember. For example, you can map your domain name to your AWS resource. If you don't have a domain name, you can search for available domains and register them using Amazon Route 53.


If you have an existing domain name, you can transfer it to Amazon Route 53. Amazon Route 53 enables you to organize your DNS records using hosted zones. When you create a hosted zone, you receive four name servers to help ensure a high level of availability.


Ads

5). What is a Load balancer?

A load balancer distributes traffic to multiple instances. You can achieve even higher levels of fault tolerance by using your load balancer with instances in multiple Availability Zones.


As instances are launched and terminated, the load balancer automatically directs traffic to the running instances. Elastic Load Balancing also performs health checks on each instance. If an instance is not responding, the load balancer can automatically redirect traffic to healthy instances.


6). What is an instance store volume?


Amazon EC2 provides instance store volumes for many types of EC2 instances. The disks for these volumes are physically attached to the same host computer as the instance, so access to these volumes is very fast.

There is no additional charge to use the instance store volumes provided by the instance type, but you can incur data transfer charges for data transferred to and from the instance.



An instance store volume is usable only from a single instance and only during its lifetime. For instance, for types that support multiple instance store volumes, you can stripe your data across multiple volumes.

The data on an instance store volume is erased when the instance terminates. If an application uses instance store volumes for persistent data, it must periodically replicate the data or copy it to durable storage.


7) What is AWS import and Export?

Use AWS Import/Export to transfer data to or from AWS (Amazon S3 buckets, Amazon EBS snapshots, or Amazon Glacier vaults), using portable storage devices.

This is a good option if it would be too costly or slow (more than a week) to transfer your data to AWS over the Internet.
