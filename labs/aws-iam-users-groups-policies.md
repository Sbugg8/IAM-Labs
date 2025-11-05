# IAM Users, Groups, and Policies

**Status:** In progress

**Objective:** Create a lab user and group, attach a policy, and verify access in a sandbox.

## Steps performed
1. Snapshot sandbox / VM before changes.
2. Created user `labuser1`.
3. Created group `LabAdmins` and added `labuser1`.
4. Attached `AdministratorAccess` for initial testing (will narrow to least-privilege later).

## Evidence
### 🧾 Verification Screenshots

**1. IAM User Creation in Progress**  
![User creation screenshot](../images/lab1-user-creation.png)

**2. IAM User Successfully Created**  
![User created screenshot](../images/lab1-user-created.png)

**3. Policy Attached (ReadOnlyAccess)**  
![Policy attachment screenshot](../images/lab1-attach-policy.png)

**4. Failed S3 Bucket Creation (Permission Denied)**  
![Failed bucket screenshot](../images/lab1-failed-bucket.png)


## Notes
- Verified user appears in console; interactive login verification is pending due to sandbox login constraints.
- Next: replace AdministratorAccess with a least-privilege policy and re-test.

## Next steps
1. Complete login verification as `labuser1`.  
2. Create and test a least-privilege policy for the required actions.  
3. Re-scan and add final screenshots; move file to `completed/` when fully verified.
