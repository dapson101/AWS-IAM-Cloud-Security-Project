
AWS IAM Cloud Security Project  
1. Project Overview 
I completed this project on cloud security controls in Amazon Web Services (AWS), focusing on 
Identity and Access Management (IAM). The goal was to create a least‑privilege policy, attach it 
to a user group, and verify that the policy correctly restricts actions on two Amazon EC2 
instances (audit and sales). 
2. Tools & Concepts 
● AWS IAM – users, groups, policies, account alias 
● Amazon EC2 – instance tagging and lifecycle actions 
● JSON policy syntax – Effect, Action, Resource 
● Principle of least privilege and policy testing 
3. Tagging Strategy 
I applied a descriptive tag to each EC2 instance: 
Instance | Tag Key            
| Tag Value 
audit       
sales       
| Environment  | Audit 
| Environment  | Sales 
4. Creating the IAM Policy 
I authored the following JSON policy to block instance stop/start actions on the audit server but
