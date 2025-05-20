# Lab 3: IAM Policy Simulator and Permissions Boundaries

## 📝 Objective
Learn to use the IAM Policy Simulator, and implement permissions boundaries to restrict IAM access.

## 🧪 Tasks
- Use the IAM Policy Simulator to test access
- Create a custom policy with conditions
- Apply a permissions boundary to an IAM user

## ⚙️ Steps
1. Sign into AWS Console and open IAM
2. Go to **Policy Simulator** → simulate access for a user/role
3. Create a policy with `Condition` (e.g., time-based or IP restriction)
4. Attach the policy as a **permissions boundary**
5. Test behavior with and without boundary

## 📸 Screenshots
- ![Policy Simulator Example](../images/policy-simulator-example.png)

## ✅ Outcome
- Verified access via simulation
- Observed effect of permissions boundary on IAM user

## 🔗 Resources
- [AWS Docs: Permissions Boundaries](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies_boundaries.html)
