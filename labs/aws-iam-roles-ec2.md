# IAM Lab: Roles & EC2 Permissions (AWS)

## 🔍 Goal

Learn how to:
- Create an IAM role with specific permissions
- Attach the role to an EC2 instance
- Use the role to access AWS services (like S3) without long-term credentials

---

## 🛠️ Tools Used

- AWS Management Console
- AWS IAM
- EC2 instance (Amazon Linux 2)
- AWS CLI

---

## 📝 Steps Taken

1. **Created IAM Role**
   - Trusted entity: EC2
   - Attached `AmazonS3ReadOnlyAccess` managed policy
   - Role name: `EC2ReadOnlyS3Role`

2. **Launched EC2 Instance**
   - Amazon Linux 2 AMI
   - t2.micro
   - Attached `EC2ReadOnlyS3Role` during launch

3. **Connected to EC2 via SSH**
   - Used EC2 key pair to connect to the instance

4. **Verified Access with AWS CLI**
   - Ran `aws s3 ls` → success!
   - Verified no write/delete access to S3

---

## ❗ Issues Faced

- Forgot to attach role at EC2 launch → had to stop instance and attach role later
- AWS CLI not installed by default → used `sudo yum install aws-cli -y`

---

## 💡 Key Takeaways

- IAM roles let services like EC2 assume temporary credentials
- No need to hardcode access keys — much safer
- Trust policies define **who** can assume the role
- Permissions policies define **what** the role can do

---

## 📸 Screenshots

> _(Optional — add screenshots of role creation or EC2 testing here)_

---

## 📚 References

- [IAM Roles for EC2](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_use_switch-role-ec2.html)
- [AmazonS3ReadOnlyAccess Policy](https://docs.aws.amazon.com/AmazonS3/latest/userguide/access-control-overview.html)

