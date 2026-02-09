# Role-Based Access Control (RBAC) & Identity Management

## 📌 Project Overview
In this project, I developed a structured **Role-Based Access Control (RBAC) Matrix** to manage user permissions for a cloud-based SaaS environment. The goal was to ensure that users—ranging from HR representatives to system auditors—had exactly the access they needed to perform their jobs, and nothing more.

## 🛡️ Security Design Principles
This project focuses on the **Principle of Least Privilege (PoLP)**. By granularly defining roles, I reduced the "Trust Surface" of the organization, ensuring that a compromise of one account would not lead to a total data breach.

### **Key Technical Deliverables:**
* **Access Control Matrix:** A visual mapping of roles to permissions (View, Create, Modify, Delete, None).
* **Cross-Functional Permissioning:** Balancing access for HR (Employee Data), Clinicians (Patient Data), and Admins (System Logs).

## 🔍 Visual Proof of Concept
![RBAC Matrix Chart](images/RBAC-Matrix.png)
*Above: A screenshot of the finalized permission matrix showing the distribution of access across different organizational tiers.*

## 💡 Technical Deep Dive: Preventing Lateral Movement
In this scenario, I specifically designated **Janet** as the primary SaaS administrator while restricting **Norman** (the auditor) to "View-Only" access for backup logs. 
* **The Logic:** If an auditor's account is compromised, the attacker cannot delete logs to hide their tracks. 
* **The Result:** This maintains **Integrity** and **Accountability** within the system's audit trail.

## 📈 Lessons Learned & Refinement
Initially, I overthought the access requirements for specific roles. Through the refinement process, I learned that:
1. **Less is More:** It is safer to deny access by default and grant it as needed rather than granting broad access and trying to restrict it later.
2. **The Human Element:** Understanding the actual workflow of a user (like Simone in HR) is vital to creating a matrix that doesn't hinder business operations while staying secure.
