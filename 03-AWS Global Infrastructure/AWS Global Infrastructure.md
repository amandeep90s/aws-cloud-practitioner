# AWS Global Infrastructure

AWS Global Infrastructure is designed to provide a resilient, highly available, secure, and low-latency solution for customers. Below are the key components:

---

## 1. Availability Zones (AZs) and Regions

- **Regions**: Physical locations worldwide where AWS clusters data centers.
- **Availability Zones (AZs)**: Isolated locations within a Region, consisting of multiple data centers.
- Resources in the same AZ Code Name across accounts may not be physically located in the same AZ.

---

## 2. Edge Locations

- Deployed in major cities and highly populated areas.
- Used by services like **AWS CloudFront** and **AWS Lambda@Edge** to cache data and reduce latency.
- Example: A user in Europe accessing a website hosted in Ohio is redirected to the nearest Edge Location for faster access.

---

## 3. Regional Edge Caches

- Larger caches between CloudFront Origin servers and Edge Locations.
- Retain data longer than Edge Locations, reducing latency when data is no longer available at the Edge Location.

---

## 4. Local Zones

- Provide core AWS services (Compute, Storage, Networking, Database) near major cities without nearby AWS Regions.
- Useful for:
  - Applications requiring single-digit millisecond latency.
  - Data residency requirements.
- Connected to a parent Region via a high-speed connection.
- **Dedicated Local Zones**: Fully managed infrastructure for exclusive use, useful for industries with strict governance controls.

---

## 5. Wavelength Zones

- Embedded within 5G mobile broadband networks in telecom providers' data centers.
- Enable ultra-low latency for 5G applications like live video streaming and gaming.
- Available through providers like Verizon (US), KDDI (Japan), SK Telecom (South Korea), Vodafone (UK/Germany), and Bell (Canada).

---

## 6. Outposts

- Brings AWS cloud capabilities to on-premises data centers.
- Includes AWS hardware for running native AWS services (e.g., EC2, S3, RDS).
- Available as rack-mountable servers (1U/2U) or full racks (42U).
- Fully managed by AWS, including patching and updates.

---

## Summary

Understanding AWS Global Infrastructure components like AZs, Regions, Edge Locations, Regional Edge Caches, Local Zones, Wavelength Zones, and Outposts helps you design resilient, secure, and low-latency solutions for your customers.
