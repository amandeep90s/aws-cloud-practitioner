# Introduction to Amazon EC2

Amazon Elastic Compute Cloud (EC2) is a core AWS compute service that allows you to deploy virtual servers in your AWS environment. Below are the key components and features of EC2:

---

## 1. Amazon Machine Images (AMIs)

- **Definition**: Pre-configured templates for launching EC2 instances.
- **Types**:
  - AWS-managed AMIs (e.g., Amazon Linux, Ubuntu, Windows).
  - Custom AMIs: Create your own templates with pre-installed applications and configurations.
  - AWS Marketplace AMIs: Vendor-provided AMIs with specific configurations.
  - Community AMIs: Public AMIs shared by others.
- **Use Case**: Simplifies deployment and supports auto-scaling by quickly launching instances with predefined configurations.

---

## 2. Instance Types

- Define the size and performance of an instance based on:
  - **vCPUs**: Number of virtual CPUs.
  - **Memory**: RAM size.
  - **Storage**: Capacity and type (e.g., SSD or magnetic).
  - **Network Performance**: Data transfer rate.
- **Instance Families**:
  - **General Purpose**: Balanced CPU, memory, and storage.
  - **Compute Optimized**: High-performance processors.
  - **Memory Optimized**: Large-scale in-memory applications.
  - **Accelerated Computing**: Hardware accelerators for floating-point calculations.
  - **Storage Optimized**: High IOPS and low-latency storage.
  - **HPC Optimized**: High-performance computing workloads.

---

## 3. Instance Purchasing Options

- **On-Demand Instances**: Pay per second, ideal for short-term or unpredictable workloads.
- **Spot Instances**: Use unused capacity at a discount but may be interrupted.
- **Reserved Instances**: Long-term commitments (1 or 3 years) with discounts.
  - **Standard**: Limited modifications, higher discounts.
  - **Convertible**: Flexible modifications, lower discounts.
- **On-Demand Capacity Reservations**: Reserve capacity without long-term commitments.

---

## 4. Tenancy

- **Shared Tenancy**: Default option; instances share hardware with other customers.
- **Dedicated Instances**: Exclusive hardware for your account.
- **Dedicated Hosts**: Full control over physical hosts, useful for licensing and compliance.

---

## 5. User Data

- Allows you to run commands or scripts during the first boot cycle of an instance.
- Example: Automatically install software or apply updates.

---

## 6. Storage Options

- **Persistent Storage**: Amazon Elastic Block Store (EBS).
  - Network-attached, durable, and supports snapshots.
  - Can be encrypted and detached/reattached to other instances.
- **Ephemeral Storage**: Instance store volumes.
  - Physically attached to the host, fast but temporary (data lost on stop/terminate).

---

## 7. Security

- **Security Groups**: Instance-level firewalls to control inbound and outbound traffic.
- **Key Pairs**:
  - Public key: Stored by AWS.
  - Private key: Used for authentication (e.g., SSH for Linux, decrypting Windows passwords).
  - Must be securely stored by the user.
- **Shared Responsibility Model**: Users are responsible for maintaining OS and security patches.

---

Amazon EC2 provides flexible, scalable, and secure compute resources to meet diverse application needs. Understanding its components and features helps optimize deployments and costs.
