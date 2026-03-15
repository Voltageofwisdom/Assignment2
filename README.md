# Assignment2
Perform a vulnerability scan on a demo website using online scanners like OWASP ZAP. 
Analyze a phishing attack scenario and identify key indicators of compromise.

  1: VULNERABILITY SCAN ON A DEMO WEBSITE ( http://demo.testfire.net ) USING AN ONLINE TOOL ( nikito ) ON MY LINUX TERMINAL.
   I opened my linux terminal and inputted the command ( nikito -h http://demo.testfire.net )  
and it gave this results 
    The anti-clickjacking X-Frame-Options header is not present
   The X-Content-Type-Options header is not set. This could allow the user agent to render the content of the site in a different fashion to the MIME type.

   Invicti detected a missing Content-Type header which means that this website could be at risk  of a MIME-sniffing attacks.

   2: ANALYZING OF A PHISHING SCENARIO AND IDENTIFICATION OF KEY FACTORS OF COMPROMISE.

1. Phishing Attack Scenario
   A university student receives an email that appears to come from the IT department of the school. The email states:
“Your university email account will be suspended today due to unusual activity. Click the link below to verify your account immediately.”
The email contains a link labeled “Verify Account.”
When the student clicks the link, it opens a website that looks identical to the university login page. The student enters their username and password.
The attacker then captures these credentials and uses them to access the student’s email account. From there, the attacker sends phishing emails to other students and may access confidential files.

2. Key Indicators of Compromise (IOCs)
   1. Suspicious Email Address
The sender’s email looks similar to the official email but contains slight changes.
Example:
Legitimate: it-support@university.edu
Phishing: it-support@university-security.com
 Small spelling differences or extra characters are common phishing signs.

   2. Urgent or Threatening Language
The email creates pressure or panic to make the victim act quickly.
Examples:
“Your account will be suspended immediately.”
“Verify your account within 24 hours.”
Attackers use urgency so users do not verify the message.

  3. Suspicious Links
The hyperlink appears legitimate but actually redirects to a malicious website.
Example:
Displayed link:
www.university.edu/login
Actual link:
www.university-security-login.com
Hovering over the link usually reveals the real destination.

  4. Fake Login Page
The phishing site copies the design of the real login page but is hosted on a different domain.
Indicators include:
Slight design differences
Unsecured connection (no HTTPS)
Unusual URL

  5. Unexpected Attachments
Phishing emails may include malicious attachments such as:
.exe
.zip
.docm (macro-enabled files)
Opening these can install malware.

  6. Unusual Account Activity
After the compromise, signs may include:
Login from unfamiliar locations
Password changes
Emails sent without the user’s knowledge


3. Impact of the Phishing Attack:
    If successful, phishing can lead to:
Account takeover
Data theft
Financial fraud
Spread of malware
Unauthorized access to systems.

4. Prevention Measures
To prevent phishing attacks:
Verify the sender’s email address
Hover over links before clicking
Enable multi-factor authentication (MFA)
Avoid downloading suspicious attachments
Report phishing emails to the IT/security team.
