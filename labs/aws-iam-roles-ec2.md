# Lab 2: IAM Roles and EC2 Permissions

## 📌 Objectives
- Create IAM Role with EC2 trust
- Attach policy for S3 read-only access
- Launch EC2 instance with role
- Verify permissions from EC2

---

## 🛠️ Steps Performed

| Step | Action |
|------|--------|
| 1 | Created IAM role `EC2S3ReadOnlyRole` with EC2 trust |
| 2 | Attached `AmazonS3ReadOnlyAccess` managed policy |
| 3 | Launched EC2 instance and attached the role |
| 4 | Connected to EC2 via SSH |
| 5 | Verified access to S3 buckets using `aws s3 ls` |

---

## ✅ Results

- EC2 instance successfully assumed IAM role.
- Verified S3 access using AWS CLI.

---

## 🖼️ Screenshot

> _Add a screenshot of your EC2 terminal output or role attached to instance._

---

## 🗂️ Status

✅ **Lab Completed Successfully**
