# Security Governance & Risk Mitigation Strategy

## 📌 Project Overview
This project is a comprehensive risk analysis of an enterprise-level security breach at "Fizza Cola." The organization suffered from both physical security failures and a malware outbreak. I was tasked with identifying the root causes and designing a governance strategy to prevent recurrence.

## 📉 Incident Analysis: The CIA Triad
The primary security objective compromised in this breach was **Availability**. 
* **The Breach:** Unauthorized access to the payroll admin office led to system outages and infected workstations.
* **The Impact:** Loss of availability resulted in financial inaccuracies, potential PII theft, and significant reputational damage.

## 🛡️ Proposed Mitigation Framework
I developed a **Defense-in-Depth** strategy to address both the technical and human factors of the breach:

| Vulnerability | Proposed Control | Design Principle |
| :--- | :--- | :--- |
| **Physical Intrusion** | Office Locking & Entry Logs | Layering |
| **Malware Entry** | MFA & Email Sandboxing | Fail-Safe Defaults |
| **Human Negligence** | Continuous Security Awareness | Usability & Education |

## 🔍 Visual Analysis
![Security Objective Analysis](images/fizza-cola-analysis.png)
*Above: Snippet of the strategic analysis identifying Availability as the critical point of failure.*



## 💡 Technical Deep Dive: The "Human Firewall"
A major focus of this project was the **Security Awareness Program**. 
* **The Logic:** Even the best technical controls fail if an employee leaves a door unlocked or clicks a phishing link. 
* **The Solution:** I proposed integrating security training into the onboarding process (within 60 days) and maintaining annual refreshers. This transforms employees from a "vulnerability" into a "sensor" for the security team.

## 📈 Lessons Learned
This project taught me that security is not just a "software problem." It is a combination of **Policy, People, and Physicality**. Effective governance requires a "Fail-Secure" mindset where systems default to protection during an outage rather than remaining open to threats.
