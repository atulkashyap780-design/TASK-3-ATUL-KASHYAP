Phishing Awareness Analysis

Project Title :-

Phishing Awareness Analysis

📖 Description

This project is developed as part of Project 3 of the DecodeLabs Cyber Security Internship.

The purpose of this project is to analyze emails or messages and identify common indicators of phishing attempts.

The R program checks the given message for suspicious keywords, links, urgency or threatening language, and requests for sensitive information. Based on the detected indicators, it calculates a risk score and classifies the message as Low Risk, Medium Risk, or High Risk.

🔍 Key Features

- Detects common phishing-related keywords.
- Identifies suspicious links in messages.
- Detects links using HTTP instead of HTTPS.
- Identifies urgent or threatening language.
- Detects references to sensitive information such as passwords, OTPs, PINs, CVV, and banking details.
- Lists the red flags found in the message.
- Calculates a risk score.
- Provides a risk-level classification.
- Gives a basic safety recommendation to the user.

🛠️ Technologies Used

- R Programming Language
- VS Code
- GitHub

▶️ How to Run

1. Install R

Download and install R from the official R website:

https://cran.r-project.org/bin/windows/base/

2. Clone or Download the Repository

Download this repository to your computer and open the project folder in VS Code.

3. Open the R File

Open:

phishing_analyzer.R

4. Open the VS Code Terminal

Go to:

Terminal → New Terminal

5. Run the Program

Type:

Rscript phishing_analyzer.R

Press Enter.

6. Enter a Message

The program will ask:

Enter the email/message to analyze:

Enter the email or message you want to analyze and press Enter.

🧪 Example

Input

URGENT! Your account will be blocked. Verify your password immediately by clicking http://fake-login.com

Output

The program will identify multiple red flags such as:

- Suspicious keyword: urgent
- Suspicious keyword: verify
- Sensitive information: password
- Message contains a link
- Link uses HTTP instead of HTTPS
- Urgent/threatening language

The message will therefore receive a higher risk classification.

⚠️ Disclaimer

This project is an educational, rule-based phishing awareness analyzer. It identifies suspicious indicators based on predefined keywords and patterns. It should not be considered a replacement for professional email security systems or enterprise-level phishing detection solutions.

🎯 Project Objective

The main objective of this project is to develop cybersecurity awareness and understand how phishing messages can be analyzed by identifying suspicious links, keywords, and other red flags.

---

Developed as part of the DecodeLabs Cyber Security Internship — Project 3.
