TryHackMe – Reversing ELF

1. Overview

This repository contains my practical work and learning experience from the Reversing ELF challenge on TryHackMe.

The main objective was to understand how Linux ELF executables work and use static reverse engineering techniques to analyze the binary and discover hidden input values.

Challenge Details:

- Platform: TryHackMe
- Room: Reversing ELF
- Category: CTF / Reverse Engineering
- Difficulty: Beginner
- Operating System: Kali Linux
- Tools Used: Ghidra, Linux Terminal

2. Objective

The objective of this challenge was to analyze a Linux executable, understand its internal program logic, and identify the required password and secret code through static analysis.

3. Tools Used

Tool| Purpose
Kali Linux| Testing environment
Ghidra| Static reverse engineering
Linux Terminal| Executing and analyzing binaries

4. Practical Methodology

Step 1: Download and Extract the Challenge

I downloaded the challenge files from TryHackMe and extracted the provided archive using the Linux terminal.

Step 2: Execute the Binary

I executed the ELF binary to understand its behavior and identify the inputs required by the application.

Step 3: Import the Binary into Ghidra

I created a new project in Ghidra and imported the executable. After importing, I allowed Ghidra to perform its initial analysis.

Step 4: Analyze the Main Function

After the analysis was complete, I navigated to the "main()" function.

I examined the decompiled code, string references, and password validation logic to understand how the application checks user input.

Step 5: Discover the Password

By examining the comparison operations and relevant string references, I identified the password required by the application.

Discovered Password:

Sup3rS3cr3tP455W0rd

Step 6: Analyze the Secret Code Validation

Next, I examined the function responsible for validating the second input.

I followed the program flow and inspected the comparison logic to understand how the application verifies the secret code.

Step 7: Discover the Secret Code

By analyzing the validation function and its comparison values, I identified the required decimal secret code.

Discovered Secret Code:

1337

5. Final Findings

Input| Discovered Value
Password| "Sup3rS3cr3tP455W0rd"
Secret Code| "1337"

6. Key Learnings

Through this challenge, I gained practical knowledge of:

- Linux ELF executable analysis.
- Static reverse engineering.
- Ghidra navigation and decompilation.
- Understanding the "main()" function.
- Identifying strings and hidden values.
- Analyzing conditional branches.
- Understanding password and input validation logic.

7. Conclusion

The Reversing ELF challenge was a useful beginner-level reverse engineering exercise.

I learned how to inspect Linux executable files, understand application logic, and identify hidden validation values using Ghidra.

Instead of relying on random guessing, I used static analysis to understand how the application works internally.

This practical experience helped me improve my understanding of Linux binary analysis and reverse engineering.

---

Author: Jash Kania

Platform: TryHackMe

Focus Areas: Cybersecurity | Reverse Engineering | Linux | Binary Analysis

Disclaimer: This write-up is for educational purposes and documents my learning experience in an authorized TryHackMe CTF environment.
