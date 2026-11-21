# week-3-pdf-password-recovery-lab
A practical cybersecurity lab demonstrating PDF password recovery using John the Ripper (Johnny GUI) and NetworkWalks online tools on Windows 10.


# PDF Password Recovery Lab – Week 3

## Overview

This repository documents my Week 3 practical project in Cybersecurity and Ethical Hacking.

The objective was to understand how password recovery works by testing two different approaches against an authorized, password-protected PDF lab file.

I completed the practical on **Windows 10** using:

1. John the Ripper (JTR) with Johnny GUI.
2. NetworkWalks online Hash Calculator and Password Cracker.

Both methods were successfully completed, and the recovered password was tested by opening the protected PDF file.

## Objectives

- Understand the basic concept of password cracking.
- Extract a PDF password hash from a protected PDF file.
- Use John the Ripper through its graphical interface, Johnny.
- Use NetworkWalks tools to perform a password recovery attempt.
- Verify the recovered password by opening the protected PDF.
- Understand why password complexity is important.

## Environment

| Component | Details |
|---|---|
| Operating System | Windows 10 |
| File format | Password-protected PDF |
| Method 1 | John the Ripper (JTR) |
| Graphical interface | Johnny |
| Method 2 | NetworkWalks Hash Calculator |
| Password recovery tool | NetworkWalks Password Cracker |
| Attack approach | Password guessing / dictionary-based recovery |

---

# Method 1 – John the Ripper (JTR) with Johnny GUI

## Introduction

John the Ripper is a password security auditing and recovery tool. Johnny provides a graphical interface that makes it possible to use John the Ripper without entering commands manually.

In this practical, I used Johnny to load an extracted PDF hash and perform a password recovery attack.

## Tools Used

- John the Ripper: https://www.openwall.com/john/
- Johnny GUI: https://openwall.info/wiki/john/johnny
- Online PDF Hash Extractor: https://www.onlinehashcrack.com/tools-pdf-hash-extractor.php

## Practical Steps

### 1. Download and install the tools

- Downloaded John the Ripper for Windows.
- Downloaded and installed the Johnny graphical interface.
- Opened Johnny after installation.

### 2. Configure Johnny

- Opened the Johnny settings.
- Browsed to the John the Ripper installation directory.
- Selected `john.exe` from the `run` folder.
- Configured Johnny to use the John executable.

### 3. Extract the PDF hash

- Opened the online PDF Hash Extractor.
- Uploaded the authorized password-protected PDF file.
- Generated and copied the extracted PDF hash.
- Checked that the hash started with `$pdf$`.

### 4. Save the extracted hash

- Opened Notepad.
- Pasted the extracted hash.
- Saved the text file as `hash1.txt`.

### 5. Load the hash into Johnny

- Opened Johnny.
- Selected **Open password file**.
- Browsed to `hash1.txt`.
- Loaded the extracted hash.

### 6. Start the password recovery attack

- Selected **Start new attack**.
- Waited for John the Ripper to process the hash.
- Observed the result displayed by Johnny.

### 7. Verify the result

- Opened the original protected PDF.
- Entered the recovered password.
- Confirmed that the PDF opened successfully.

---

# Method 2 – NetworkWalks Tools

## Introduction

The second practical used two online tools provided by NetworkWalks.

The Hash Calculator extracts the PDF hash, while the Password Cracker attempts to recover the password from that hash.

Both tools are accessed through a web browser, so no local software installation is required for this method.

## Tools Used

- NetworkWalks Hash Calculator: https://networkwalks.com/hash-calculator/
- NetworkWalks Password Cracker: https://networkwalks.com/password-cracker/

## Practical Steps

### 1. Open the Hash Calculator

- Opened the NetworkWalks Hash Calculator in a web browser.

### 2. Extract the PDF hash

- Uploaded the authorized locked PDF file.
- Waited for the tool to generate the hash.
- Copied the complete hash starting with `$pdf$`.

### 3. Recover the password

- Opened the NetworkWalks Password Cracker.
- Pasted the extracted PDF hash.
- Started the password recovery attempt.
- Waited for the tool to display the result.

### 4. Verify the result

- Opened the original protected PDF.
- Entered the recovered password.
- Confirmed that the PDF opened successfully.

## Screenshots

1. PDF hash extraction using NetworkWalks Hash Calculator.
2. Password recovery using NetworkWalks Password Cracker.
3. Successful PDF password verification.
---

# Results

Both practical methods were completed successfully.

| Method | Tools | Result |
|---|---|---|
| Method 1 | John the Ripper + Johnny GUI | Successful |
| Method 2 | NetworkWalks Hash Calculator + Password Cracker | Successful |

The recovered password was verified by opening the protected PDF file.

## Key Learnings

Through this practical, I learned how to:

- Extract a PDF password hash.
- Understand the role of hashes in password recovery.
- Configure and use John the Ripper through Johnny GUI.
- Load a hash file and start a password recovery attack.
- Use online tools to extract hashes and attempt password recovery.
- Verify the result by opening the protected document.
- Understand the importance of strong and complex passwords.

## Security Note

This project was conducted for educational purposes using authorized lab files.

Password recovery techniques should only be used on files and systems for which explicit permission has been granted.

## References

- NetworkWalks – Cybersecurity & Ethical Hacking Project Tasks.
- John the Ripper: https://www.openwall.com/john/
- Johnny GUI: https://openwall.info/wiki/john/johnny
- NetworkWalks Hash Calculator: https://networkwalks.com/hash-calculator/
- NetworkWalks Password Cracker: https://networkwalks.com/password-cracker/

---

**Project:** Week 3 – Cybersecurity & Ethical Hacking  
**Platform:** Windows 10  
**Documentation:** Practical steps and screenshots
