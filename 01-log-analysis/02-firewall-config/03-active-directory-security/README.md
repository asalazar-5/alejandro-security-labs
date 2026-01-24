# Lab 03 – Active Directory Security & Authentication Monitoring

## Objective
The goal of this lab is to demonstrate hands-on experience with identity and access management (IAM) by configuring and securing an Active Directory environment. This lab focuses on user management, authentication monitoring, and detecting suspicious login behavior—key responsibilities in SOC and Security Analyst roles.

---

## Tools Used
- Windows Server (Domain Controller)
- Windows 10/11 Client VM
- Active Directory Users and Computers
- Group Policy Management
- Windows Event Viewer

---

## Lab Environment
- One Windows Server VM configured as a Domain Controller
- One Windows Client VM joined to the domain
- Security auditing enabled on authentication events

---

## Step-by-Step Implementation

### Step 1: Configure Active Directory Domain Controller
1. Install Windows Server and promote it to a Domain Controller.
2. Create a new domain and verify AD services are running.
3. Join a Windows client VM to the domain.

📸 **Screenshot:** Active Directory Users and Computers console.

---

### Step 2: Create Users, Groups, and Permissions
1. Create multiple user accounts.
2. Create security groups (IT, HR, Users).
3. Assign users to appropriate groups.
4. Apply least-privilege access controls.

📸 **Screenshot:** AD user and group configuration.

---

### Step 3: Configure Security Policies
1. Configure password complexity and expiration policies.
2. Enable account lockout thresholds.
3. Apply policies via Group Policy Management.

📸 **Screenshot:** Group Policy settings.

---

### Step 4: Simulate Authentication Events
1. Attempt failed logins using incorrect credentials.
2. Trigger account lockouts.
3. Observe authentication behavior across users.

📸 **Screenshot:** Failed login and lockout events in Event Viewer.

---

### Step 5: Analyze Authentication Logs
1. Review Windows Security logs.
2. Identify:
   - Failed login attempts
   - Account lockouts
   - Unusual login behavior
3. Document findings and potential response actions.

📸 **Screenshot:** Event Viewer showing authentication logs.

---

## Findings
- Failed authentication attempts were clearly logged.
- Account lockout policies effectively mitigated brute-force attempts.
- Logs provided actionable data for incident investigation.

---

## Lessons Learned
- Identity-based attacks are a common threat vector.
- Strong authentication policies significantly reduce risk.
- Log analysis is essential for detecting account abuse.

---

## Security+ Alignment
- Identity and access management (IAM)
- Authentication and authorization
- Account policies and monitoring
- Logging and auditing

---

## Interview Talking Points
- “I built and secured an Active Directory environment and monitored authentication events.”
- “I detected failed logins and account lockouts using Windows security logs.”
- “This lab mirrors how SOC teams investigate identity-based attacks.”

---

## Next Steps
- Forward AD logs to a SIEM for correlation.
- Implement MFA in the environment.
- Create alerts for repeated failed login attempts.

