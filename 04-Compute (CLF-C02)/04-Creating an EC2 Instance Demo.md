# Creating an EC2 Instance Demo

This demo walks through the process of creating an EC2 instance in the AWS Management Console.

---

## Steps to Create an EC2 Instance:

### 1. Launch an Instance

- Navigate to **Services > Compute > EC2**.
- Click **Launch instance**.
- Enter a name for your instance (e.g., `MyInstance`).
- Add tags if needed (e.g., project, cost center).

---

### 2. Select an Amazon Machine Image (AMI)

- Choose an AMI from:
  - **Quick Start AMIs**: Pre-configured options like Amazon Linux, macOS, or Windows.
  - **AWS Marketplace AMIs**: Vendor-provided AMIs with specific configurations.
  - **Community AMIs**: Public AMIs shared by others.
  - **Custom AMIs**: Your own pre-configured templates.
- For this demo, select the **Amazon Linux 2023 AMI**.

---

### 3. Choose an Instance Type

- Select an instance type based on:
  - **vCPUs**, **Memory**, **Storage**, and **Network Performance**.
- Use the **Compare instance types** tool to filter and sort options.
- For this demo, select the **t2.micro** instance (free tier eligible).

---

### 4. Configure Key Pair

- Select an existing key pair or create a new one.
- Download the private key and keep it secure.

---

### 5. Configure Network Settings

- Select a **VPC** and **subnet**.
- Choose whether to assign a public IP address.
- Configure a **security group**:
  - Add rules for inbound traffic (e.g., SSH on port 22, HTTP on port 80).
  - Specify allowed IP ranges (e.g., `10.0.1.0/24`).

---

### 6. Configure Storage

- Default: 8 GB **gp3 root volume**.
- Options:
  - Adjust IOPS, encryption, or delete-on-termination settings.
  - Add additional volumes or shared file systems (e.g., EFS, FSx).

---

### 7. Advanced Settings

- Configure options like:
  - **Spot Instances**: Specify max price and interruption behavior.
  - **IAM Instance Profile**: Grant permissions to interact with AWS services.
  - **Auto-recovery**: Recover instance if system checks fail.
  - **User Data**: Add scripts to run at launch (e.g., `yum update -y`).

---

### 8. Launch the Instance

- Review the summary panel (e.g., AMI, instance type, storage, security group).
- Click **Launch instance**.
- Verify the instance state changes from **Pending** to **Running**.

---

## Status Checks

- **System Status Checks**:
  - Monitor the underlying host (e.g., power, network, hardware issues).
  - Resolution: Stop and restart the instance to move to a new host.
- **Instance Status Checks**:
  - Monitor the instance itself (e.g., network misconfigurations, memory issues).
  - Resolution: Troubleshoot and fix the issue manually.

---

## Key Takeaways

- EC2 instances are highly configurable, allowing you to tailor them to your needs.
- Security groups and key pairs are critical for securing access.
- Status checks help identify and resolve issues with your instance or its host.

---

For hands-on experience, explore labs to practice creating EC2 instances for Linux and Windows.
