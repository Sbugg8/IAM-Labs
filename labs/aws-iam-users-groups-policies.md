# IAM Lab: Users, Groups, and Policies (AWS)

## 🔍 Goals 

Understand the core components of AWS Identity and Access Management by:
- Creating IAM users and groups
- Attaching managed policies
- Testing permissions using the AWS Management Console

---

## 🛠️ Tools Used

- AWS Management Console
- AWS IAM
- IAM Policy Simulator (optional)

---

## 📝 Steps Taken

1. **Created IAM Users**
   - Created `dev_user1` and `dev_user2`
   - Disabled console access for one user to simulate CLI-only accounts

2. **Created IAM Group**
   - Named it `DevTeam`
   - Attached `AmazonS3ReadOnlyAccess` managed policy

3. **Added Users to Group**
   - Added both users to the `DevTeam` group

4. **Tested Permissions**
   - Logged in as `dev_user1`
   - Verified access to S3 buckets but no permission to write or delete

5. **Edited Inline Policy**
   - Created and attached a custom inline policy to `dev_user1` for limited EC2 Describe actions

---

## ❗ Issues Faced

- Received "Access Denied" error when testing EC2 actions → Resolved by attaching correct inline policy
- Forgot to enable console access initially for testing → Updated user settings

---

## 💡 Key Takeaways

- IAM groups simplify permission management
- Managed policies are easy to start with; inline policies offer fine-tuned control
- Least privilege principle: always test permissions with minimal access
- IAM Policy Simulator is helpful to test without needing live access attempts

---

## 📸 Screenshots

> _(Optional — add if you took any screenshots of your setup. Can link like: `![Alt text](../images/iam-users.png)`)_  

---

## 📚 References

- [AWS IAM Documentation](https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html)
- [IAM Policy Simulator](https://policysim.aws.amazon.com/)

