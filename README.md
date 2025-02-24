<h1>Phishing Investigation and Mitigation</h1>

<h2>📌 Project Overview</h2>

This project simulates a real-world phishing attack targeting corporate employees, demonstrating how to analyze and mitigate the threat step by step.

<h2>1: Email Phishing Analysis </h2>

An HR Manager named Preston H. receives an email from his security enterprise vendor to verify its login details

<h3>Email Example:</h3>

<strong> Subject: </strong> 🚨 Urgent Action Required: Account Verification Needed

<strong> Sender details: </strong>

IT Support  
it-support@company-secure.com

<strong> Recipient details: </strong>

Preston H.  
prestonh@companyexample.com

<strong> Body: </strong>

Dear Preston H.

To comply with our new security policies, all employees must verify their corporate accounts within <strong>24 hours</strong>.

Please click the link below to proceed with the verification:

<a href="http://company-login.secure-verification.com">Verify My Account</a>

Failure to verify your account may result in restricted access.

Best regards, </br> 
IT Security Team


<h3>Signs of phishing attempts</h3>

- Urgent actions needed: 

Subject: 🚨 Urgent Action Required: Account Verification Needed  
Verify the account in less than 24 hours or we risk losing access  

These are signs of bad actors rushing you to take an action without reflecting first if they are legit

- Not trustworthy landing page and link

When hovering over the <strong> "Verify My Account"</strong> text on the email's body, we can see at the bottom left a preview of the destination URL before clicking the link and it does not seem like an official login page of a company  
![image](https://github.com/user-attachments/assets/cb3986f6-9892-4d54-b2f1-dd81d0c4a5ef)  

![Screenshot 2025-02-24 132100](https://github.com/user-attachments/assets/0b61c37e-b98a-4cd6-b329-35c3e7268702)  

- Redirecting to a login page and entering credentials: A company following best security practices will never send its users directly a link where they manage sensitive information, for example, <strong> login credentials</strong>, instead they encourage you to go to their official web or app, log in manually and do the actions needed








