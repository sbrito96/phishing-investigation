# Phishing Investigation and Mitigation

## 📌 Project Overview
This project showcases my ability to analyze phishing emails, investigate DNS records and implement mitigation strategies simulating a real-world security incident.

## 1️⃣ Email Phishing Analysis
An HR Manager named Preston H. receives an email from his security enterprise vendor requesting verification of his login details.

### 📧 Email Example:

**Subject:** 🚨 Urgent Action Required: Account Verification Needed  

**Sender Details:**  
IT Support  
it-support@company-secure.com  

**Recipient Details:**  
Preston H.  
prestonh@companyexample.com  

**Body:**  

> Dear Preston H.,  
> To comply with our new security policies, all employees must verify their corporate accounts within **24 hours**.  
> Please click the link below to proceed with the verification:  
> [Verify My Account](http://company-login.secure-verification.com)  
> Failure to verify your account may result in restricted access.  
>
> Best regards,  
> IT Security Team  

---

## 🔍 Signs of Phishing Attempts

### 🚨 Urgent Actions Required
- **Subject:** 🚨 Urgent Action Required: Account Verification Needed  
- **Message:** Verify the account within 24 hours or risk losing access.  

These are signs of cybercriminals trying to rush the recipient into taking immediate action without verifying the legitimacy of the request.

### 🔗 Suspicious Landing Page and Link
When hovering over the **"Verify My Account"** text in the email body, a preview of the destination URL appears at the bottom left before clicking the link. This URL does not resemble an official company login page.  

![image](https://github.com/user-attachments/assets/cb3986f6-9892-4d54-b2f1-dd81d0c4a5ef)  

![Screenshot 2025-02-24 132100](https://github.com/user-attachments/assets/0b61c37e-b98a-4cd6-b329-35c3e7268702)  

### ⚠️ Redirecting to a Fake Login Page
A company following best security practices will **never** send users a direct link to manage sensitive information, such as **login credentials**. Instead, they will encourage users to manually visit their official website or app, log in, and take the necessary actions.  

---

## 2️⃣ DNS & Email Authentication Check

To verify if the sender's domain enforces security policies like DMARC, I ran a DNS lookup using **MXToolbox**.

### **Results:**
- ❌ **No DMARC Record Found** → The domain does not have DMARC configured, meaning it does not enforce authentication policies for emails sent from this domain.
- ❌ **No DNS Record Found** → The domain itself is not properly registered or does not have valid mail exchange (MX) records.
- ⚠ **DMARC Policy Not Enabled** → Even if a DMARC record existed, it is not set to reject or quarantine unauthorized emails.

![image](https://github.com/user-attachments/assets/21524089-014d-49b2-9835-0f90e570d27a)

Results example of a real DNS: google.com

![image](https://github.com/user-attachments/assets/8cde5dc4-87a5-4ca1-9206-0e6c9e7f5789)


### 3️⃣ Analyze Malicious Links
**Objective:** Identify fraudulent links without clicking on them.

🔹 **Tool:**
- [VirusTotal](https://www.virustotal.com/)

📌 **Example Analysis Result:**
```
The link http://company-login.secure-verification.com is flagged as phishing by multiple security companies.
```
![image](https://github.com/user-attachments/assets/8d542d63-d080-43e1-a8ef-08154b75e355)


### 4️⃣ Document Mitigation and Response
**Objective:** Report the phishing attempt and propose countermeasures.

### **📌 Report Submission**
- The phishing attempt was reported to:
  - **Internal IT Security Team** for internal awareness and investigation.
  - **Google Safe Browsing** to flag the malicious link.
  - **Anti-Phishing Working Group (APWG)** to share intelligence with security researchers.

### **🚀 Immediate Actions Taken**
- **Blocked the malicious domain** `company-login.secure-verification.com` at the network level.
- **Informed employees** via an internal security alert about the phishing attempt.
- **Updated email security filters** to detect similar phishing patterns.

### **🔐 Future Prevention Measures**
- **Employee Awareness Training**: Conduct phishing simulations and educate staff on identifying threats.
- **Enable Multi-Factor Authentication (MFA)**: To prevent credential theft from leading to unauthorized access.
- **Regularly Monitor Phishing Threats**: Use automated tools to scan for new phishing domains.

### 5️⃣ Conclusion
This phishing investigation and mitigation project demonstrates my ability to analyze and respond to cybersecurity threats effectively. By combining technical tools and security awareness organizations can prevent phishing attacks and enhance their defense mechanisms.

## ⚠️ Ethical Disclaimer
🚨 **This project is for educational purposes only. No real phishing attacks were conducted.** 🚨

