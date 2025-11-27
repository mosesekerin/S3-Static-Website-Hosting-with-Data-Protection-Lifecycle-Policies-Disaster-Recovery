# Ì≥Å **S3 Static Website Hosting with Data Protection, Lifecycle Policies & Disaster Recovery**

## Ì≥ù **Project Overview**

This project demonstrates how to host, secure, and manage a static website for a small caf√© business using **Amazon S3**.
It was built as part of a cloud challenge lab to simulate a real-world scenario in which a business transitions from zero cloud presence to a modern, secure, cost-optimized cloud architecture.

The website showcases the caf√©‚Äôs services while implementing **AWS best practices** for data protection, lifecycle management, and disaster recovery (DR).

---

## ÌæØ **Objectives**

By completing this project, I implemented the following:

### ‚úî **1. Host a Static Website on Amazon S3**

* Created and configured an S3 bucket for static website hosting.
* Uploaded website assets (HTML, CSS, images, etc.).
* Enabled static hosting and configured index and error documents.

### ‚úî **2. Protect Data Using Amazon S3**

* Implemented bucket policies to control access.
* Applied AWS-recommended security settings.
* Ensured the website only exposes the necessary public objects.

### ‚úî **3. Implement a Data Lifecycle Strategy**

* Designed lifecycle rules to automatically transition older objects to cost-efficient storage classes like S3 Standard-IA or S3 Glacier.
* Reduced long-term storage costs by automating archival.

### ‚úî **4. Set Up a Disaster Recovery Strategy**

* Configured S3 Cross-Region Replication (CRR) for redundancy.
* Enabled versioning to maintain object history.
* Ensured the website content remains recoverable in case of region failure.

---

## Ìøó **Architecture Diagram**

```
[Local Files] ‚Üí [S3 Bucket (Static Website)] ‚Üí [Public Website]

                   | Lifecycle Rules
                   ‚Üì
        [S3 Standard-IA / Glacier]

                   | CRR
                   ‚Üì
          [Backup Bucket in Another Region]
```

---

## Ìª† **Technologies Used**

* **Amazon S3**
* **S3 Bucket Policies (IAM)**
* **S3 Versioning**
* **Lifecycle Management Rules**
* **Cross-Region Replication**
* **Static Website Hosting**

---

## Ì∫Ä **How It Works**

1. Website files are uploaded to a public S3 bucket.
2. S3 serves the files as a static website.
3. Lifecycle policies optimize cost by moving older content to cheaper storage.
4. Versioning + CRR keeps a backup in another region for disaster recovery.
5. Visitors access the caf√©‚Äôs website via the S3 website endpoint.

---

## Ì≥Ç **Repository Structure**

```
/website
    index.html
    styles.css
    images/
    script.js

/documents
    architecture.png
    lifecycle-policy.json
    bucket-policy.json
```

---

## Ì≥ò **Key Learnings**

* Designing cloud solutions using AWS foundational services.
* Configuring secure static website hosting.
* Applying lifecycle and cost-optimization techniques.
* Understanding disaster recovery strategies in AWS.
* Following AWS Well-Architected best practices.

---

## Ì≤º **Why This Project Matters (For Recruiters)**

This project demonstrates real DevOps and cloud capability, including:

* Infrastructure configuration
* Data protection and security
* Storage cost management
* Reliability and disaster recovery
* Practical AWS implementation

It reflects the ability to build functional cloud solutions based on real business needs.

---

## Ì≥£ **Feel Free to Explore**

Pull requests, issues, or suggestions for improvement are welcome.
