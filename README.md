Phishing Awareness Analysis

Project Title :-

Phishing Awareness Analysis

📖 Description

This project is developed as part of Project 3 of the DecodeLabs Cyber Security Internship.

The purpose of this project is to analyze emails or messages and identify common indicators of phishing attempts.

The R program checks the given message for suspicious keywords, links, urgency or threatening language, and requests for sensitive information. Based on the detected indicators, it calculates a risk score and classifies the message as Low Risk, Medium Risk, or High Risk.

What does it exactly do?
- Detects common phishing-related keywords.
- Identifies suspicious links in messages.
- Detects links using HTTP instead of HTTPS.
- Identifies urgent or threatening language.
- Detects references to sensitive information such as passwords, OTPs, PINs, CVV, and banking details.
- Lists the red flags found in the message.
- Calculates a risk score.
- Provides a risk-level classification.
- Gives a basic safety recommendation to the user.

Technologies Used :-

- R Programming Language
- VS Code
- GitHub
 
How to Run :-
Open the project folder in VS Code, then open the terminal:
Terminal → New Terminal
Run this command:

Rscript phishing_analyzer.R

If your file is named PROJECT 3.R, use:

Rscript "PROJECT 3.R"

Then enter the email/message when prompted.
