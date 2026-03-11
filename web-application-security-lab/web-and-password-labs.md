# Password Security and Web Security Labs

This file documents hands-on practice with password cracking tools.

--------------------------------------------------

LAB 5 – Password Cracking using John the Ripper

Objective

Understand password cracking techniques and the importance of strong passwords.

Tool Used

John the Ripper

Steps Performed

1. Created a password hash using OpenSSL.

Command

openssl passwd -1 password123

This generates an MD5 hash.

2. Saved the generated hash in a text file.

Example file

hash.txt

3. Executed John the Ripper to attempt password cracking.

Command

john hash.txt

4. Allowed John to run dictionary attack using its default wordlist.

5. Displayed cracked password results.

Command

john --show hash.txt

Observations

The password was successfully cracked using a dictionary attack.

Learning Outcome

Learned how weak passwords can be cracked using automated tools and wordlists.

This highlights the importance of strong password policies.

--------------------------------------------------

LAB 6 – Basic Web Security Testing

Objective

Understand basic web application security testing techniques.

Tools Used

Burp Suite  
OWASP Juice Shop  
DVWA

Steps Performed

1. Installed vulnerable web application (Juice Shop or DVWA).

2. Configured Burp Suite proxy settings.

3. Intercepted HTTP requests from browser.

4. Observed request parameters such as cookies and form data.

5. Analyzed how web applications process user input.

Observations

Observed HTTP requests and responses between browser and server.

Interception allowed inspection of request headers and parameters.

Learning Outcome

Gained understanding of how web application traffic works and how vulnerabilities may appear in web applications.
