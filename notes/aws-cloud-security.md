# ☁️ AWS Cloud Security Notes

**Topic:** Amazon Web Services (AWS) Cloud Security
**Last Updated:** May 2026

---

## 🌐 Cloud Computing Basics

Cloud computing means using servers, storage, and services over the 
internet instead of owning physical hardware.

### Three Service Models
| Model | What It Means | AWS Example |
|---|---|---|
| **IaaS** | You manage the OS and up | EC2 (virtual servers) |
| **PaaS** | You manage only your app | AWS Lambda |
| **SaaS** | Provider manages everything | Gmail, Salesforce |

### The Shared Responsibility Model
This is one of the most important concepts in AWS security:

| AWS is responsible for... | You are responsible for... |
|---|---|
| Physical data centers | Your data |
| Hardware and networking | Access controls (IAM) |
| Hypervisor and host OS | Operating system patches (on EC2) |
| Managed service security | Encryption settings |

> 💡 Think of it like renting an apartment: the landlord maintains 
> the building, but you lock your own door.

---

## 🔐 AWS Identity & Access Management (IAM)

IAM controls **who can access what** in your AWS environment.

### Core IAM Components
| Component | What It Does |
|---|---|
| **User** | A person or app with AWS credentials |
| **Group** | A collection of users with shared permissions |
| **Role** | Temporary permissions assigned to services or users |
| **Policy** | A JSON document defining what is allowed or denied |

### Key IAM Best Practices
- ✅ Never use the root account for daily tasks
- ✅ Enable MFA (Multi-Factor Authentication) on all accounts
- ✅ Follow **Least Privilege** — only give the access someone needs
- ✅ Rotate access keys regularly
- ✅ Use roles instead of long-term credentials where possible

---

## 🖥️ EC2 Security Basics

EC2 (Elastic Compute Cloud) = virtual servers in the cloud.

### Security Controls for EC2
| Control | Purpose |
|---|---|
| **Security Groups** | Act as a virtual firewall — control inbound/outbound traffic |
| **Key Pairs** | SSH access using a public/private key instead of a password |
| **IAM Roles** | Give EC2 instances permission to access other AWS services |
| **EBS Encryption** | Encrypt the storage attached to your EC2 instance |

---

## 🪣 S3 Security Basics

S3 (Simple Storage Service) = object storage (files, backups, data).

### S3 Security Best Practices
- ✅ **Block Public Access** — turn this on unless public access is required
- ✅ **Bucket Policies** — control who can read/write to your bucket
- ✅ **Versioning** — keep previous versions of files in case of deletion
- ✅ **Encryption at rest** — encrypt data stored in S3
- ✅ **CloudTrail logging** — track who accessed or modified your bucket

---

## 🌐 VPC (Virtual Private Cloud)

A VPC is your own private, isolated section of the AWS cloud.

### Key VPC Components
| Component | What It Does |
|---|---|
| **Subnet** | Divides your VPC into public and private sections |
| **Internet Gateway** | Allows traffic in/out of your VPC from the internet |
| **NAT Gateway** | Lets private subnet resources access the internet safely |
| **Route Table** | Directs where network traffic should go |
| **Security Groups** | Instance-level firewall (stateful) |
| **NACLs** | Subnet-level firewall (stateless) |

---

## 👁️ AWS Monitoring & Logging

| Service | What It Does |
|---|---|
| **CloudWatch** | Monitors metrics, logs, and sets alarms |
| **CloudTrail** | Records every API call made in your AWS account |
| **AWS Config** | Tracks configuration changes to resources |
| **GuardDuty** | Threat detection using machine learning |
| **Security Hub** | Central dashboard for all security findings |

---

## 🏗️ AWS Well-Architected Framework — Security Pillar

The Well-Architected Framework has 6 pillars. The **Security Pillar** covers:

1. **Identity & Access Management** — control who can do what
2. **Detection** — identify security events quickly
3. **Infrastructure Protection** — protect networks and compute
4. **Data Protection** — encrypt and classify your data
5. **Incident Response** — prepare for and respond to events
6. **Application Security** — build security into your apps

---

## 🔑 Key Terms to Know

| Term | Definition |
|---|---|
| **Least Privilege** | Only grant the minimum access needed |
| **MFA** | Multi-Factor Authentication — second layer of login security |
| **Encryption at Rest** | Data is encrypted when stored |
| **Encryption in Transit** | Data is encrypted while moving (
