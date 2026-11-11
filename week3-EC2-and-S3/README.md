# Week 3 — EC2 and S3 Certificates

##  Contents
- Introduction to Amazon EC2.pdf
- Introduction to Amazon S3.pdf

## What I Learned

### Amazon EC2 (Elastic Compute Cloud)
- EC2 provides on-demand, scalable virtual servers (instances) in the cloud.
- Instances are launched from AMIs (Amazon Machine Images), which are templates containing the OS and software.
- Instance types offer different combinations of CPU, memory, storage, and networking for different workloads.
- Key pairs are used for secure login (public key stored by AWS, private key kept by you).
- Security Groups act as a virtual firewall controlling inbound and outbound traffic.
- Storage options: Amazon EBS for persistent storage, Instance Store for temporary data.
- Pricing models: On-Demand, Spot, Reserved Instances, and Savings Plans.

### Amazon S3 (Simple Storage Service)
- S3 is object storage: data is stored as objects inside buckets.
- Each object has a unique key (name) within its bucket.
- Designed for 99.999999999% (11 nines) durability.
- Buckets and objects are private by default; access is granted via Bucket Policies, IAM Policies, or ACLs.
- Versioning keeps multiple versions of an object, protecting against accidental deletion or overwrite.
- S3 offers strong read-after-write consistency.
- Common use cases: backup and restore, data lakes, static website hosting, archiving, and analytics.

## 🔗 Related
- [Back to main repository](../README.md)
