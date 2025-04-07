# General AWS Terminology

Understanding AWS terminology is essential for navigating and using AWS services effectively. Below are some key terms:

---

## 1. Account

- AWS services are housed within an **Account**.
- Types:
  - **Master Payer Account**: Contains billing data.
  - **Linked Account**: Does not contain billing data.
- AWS Organizations can manage multiple accounts.

---

## 2. Reserved Instance (RI)

- A commitment to use a specific cloud resource (type, location, size) for 1 or 3 years in exchange for a discounted rate.
- Types:
  - **AURI**: All Upfront Reserved Instance.
  - **PURI**: Partial Upfront Reserved Instance.
  - **NURI**: No Upfront Reserved Instance.

---

## 3. Savings Plans (SP)

- Similar to Reserved Instances but more flexible.
- Applied only to compute usage.

---

## 4. EC2 (Elastic Compute Cloud)

- AWS' virtual machine offering.
- **Instance Types**:
  - **Family**: Designated by a letter (e.g., "m").
  - **Generation**: Designated by a number (e.g., "5").
  - **Size**: Ranges from nano to 2xlarge (e.g., `m5a.4xlarge`).

---

## 5. IAM (Identity and Access Management)

- AWS' system for granting and governing permissions within the cloud platform.

---

## 6. Tags

- Metadata attached to AWS resources to provide contextual information (e.g., type, environment, owner, cost center).
- Uses:
  - Identifying resources.
  - Driving automation.
  - Dividing costs.
- Governance policies often require specific tags for all resources.

---

## 7. Console

- Web-based portal for managing AWS accounts and accessing services.

---

## 8. Convertible vs. Standard RIs

- **Standard RIs**: Cannot be converted or changed during their term.
- **Convertible RIs**: Can be converted to different specifications but offer a lower discount.

---

## 9. Region

- A physical location where AWS clusters data centers.
- Consists of multiple **Availability Zones (AZs)**:
  - AZs are isolated but closely situated for low latency and high performance.
  - AZs are made up of multiple physical data centers.

---

This terminology provides a foundation for understanding and working with AWS services effectively.
