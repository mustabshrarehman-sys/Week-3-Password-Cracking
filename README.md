Password Cracking with John the Ripper & Networkwalks Tools
Cybersecurity & Ethical Hacking Project | Networkwalks
Overview
During Week 3, I completed two hands-on password-cracking modules using four password-protected PDF lab files. The exercises introduced PDF hash extraction and dictionary-based password attacks through two approaches:
1. John the Ripper (JTR) with Johnny GUI
2. Networkwalks Hash Calculator and Password Cracker
The goal was to understand how password hashes can be extracted from protected PDF files, how password-cracking tools test password candidates, and why strong passwords are important.
Objectives
- Understand the difference between hashing and encryption.
- Extract password hashes from password-protected PDF files.
- Configure and use John the Ripper through Johnny GUI.
- Perform dictionary attacks using a browser-based tool.
- Verify recovered passwords by opening the protected PDF files.
- Identify the security risks of weak and commonly used passwords.
Tools Used
Tool	Purpose
John the Ripper	Password auditing and hash-cracking
Johnny GUI	Graphical interface for John the Ripper
PDF Hash Extractor	Extracts a hash from a protected PDF
Networkwalks Hash Calculator	Extracts PDF hashes in a browser
Networkwalks Password Cracker	Tests password candidates against a hash
Notepad	Saves the extracted hash as a text file
Windows PC / Web Browser	Lab environment


Module 1: Password Cracking with John the Ripper
Introduction
John the Ripper is a password-security auditing tool that supports multiple hash formats. Johnny is its graphical interface, making it easier to configure and run an attack.
Procedure
1. Install John the Ripper and Johnny
- Downloaded John the Ripper and Johnny GUI.
- Installed Johnny and opened the application.
- Located john.exe in John the Ripper's run folder.
Johnny configuration

2. Configure the John executable
In Johnny settings, browsed to and selected john.exe so the GUI could use the John the Ripper engine.

3. Extract the PDF hash
- Used a PDF hash-extraction tool on the provided locked PDF.
- Copied the extracted hash.
- Checked that the hash started with $pdf$.
Tool: Online PDF Hash Extractor

4. Save the hash
Pasted the complete hash into Notepad and saved it as hash1.txt.

5. Run the password attack
- Opened the hash file in Johnny using Open Password File.
- Selected hash1.txt.
- Started a new attack and waited for password candidates to be tested.

6. Verify the recovered password
Entered the recovered password into the protected PDF to confirm that the document opened successfully.

Module 1 outcome: The password of the provided PDF was successfully recovered using John the Ripper through Johnny GUI.
Module 2: Password Cracking with Networkwalks Tools
Introduction
This module used two browser-based Networkwalks tools. The Hash Calculator extracts the hash from a protected PDF, while the Password Cracker tests password candidates against that hash. This workflow did not require installing John the Ripper or Johnny.
Procedure
1. Open the Hash Calculator
Opened the Networkwalks Hash Calculator in a web browser.

2. Upload the protected PDF
Uploaded the provided locked PDF to the Hash Calculator.

3. Copy the extracted hash
Copied the complete hash value beginning with $pdf$.

4. Open the Password Cracker
Opened the Networkwalks Password Cracker in the browser.

5. Submit the hash and run the attack
Pasted the extracted hash into the Password Cracker and started the process. The tool tested password candidates until it found a match.

6. Verify the password
Entered the recovered password into the original PDF and confirmed that the file opened.

Module 2 outcome: The password of the provided PDF was successfully recovered using Networkwalks browser-based tools.
Overall Results
Across both modules, I practiced password recovery on four password-protected PDF files.
Module	Approach	Outcome
Module 1	John the Ripper with Johnny GUI	Password recovered
Module 2	Networkwalks Hash Calculator and Password Cracker	Password recovered
Additional practice	Repeated the workflow on two more PDFs	Two additional passwords recovered


Overall: Four PDF passwords successfully recovered during the exercises.
What I Learned
- Hashing: A hash is a one-way representation of data. Password cracking attempts to find an input that produces a matching hash; it does not simply reverse the hash.
- Hash extraction: A compatible tool can extract hash data from a password-protected PDF for auditing.
- Dictionary attacks: A dictionary attack tests password candidates from a wordlist and checks whether a candidate matches the target hash.
- John the Ripper: I learned to configure Johnny, load a hash file, and start an attack.
- Browser-based tools: I practiced extracting a PDF hash and testing password candidates without installing a local cracking application.
- Password security: Common, short, and reused passwords are more vulnerable to guessing and dictionary attacks.
Security Recommendations
- Use long, unique passwords for different accounts and files.
- Avoid common passwords and predictable patterns.
- Use a reputable password manager.
- Enable Multi-Factor Authentication (MFA) wherever available.
- Never test password recovery against files or systems without authorization.
Repository Structure
Week-3-Password-Cracking/
├── README.md
├── images/
│   ├── module-1/
│   └── module-2/
└── reports/
    ├── Module-1-John-the-Ripper.pdf
    └── Module-2-Networkwalks-Tools.pdf
Disclaimer
This work was completed for educational purposes as part of a cybersecurity training lab. Password-cracking techniques should only be used on files, accounts, and systems that you own or have explicit permission to test.
Conclusion
Week 3 provided practical experience with PDF hash extraction and dictionary-based password attacks. By using John the Ripper with Johnny GUI and Networkwalks browser-based tools, I learned how password-recovery workflows operate and why strong, unique passwords are essential for protecting information.
Project: Cybersecurity & Ethical Hacking
Training Platform: Networkwalks
Week: 03
Topic: Password Cracking
Tools: John the Ripper, Johnny GUI, Networkwalks Tools

#CyberSecurity #EthicalHacking #JohnTheRipper #PasswordSecurity #Networkwalks #InfoSec
