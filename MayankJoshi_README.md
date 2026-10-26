# Phishing Email Detector

**Project type:** Beginner cybersecurity awareness project  
**Language:** Python 3  
**Dependencies:** Python standard library only

## Overview
This command-line tool analyzes pasted email/message text for simple phishing indicators, including suspicious phrases, links, IP-address-based link hosts, and repeated exclamation marks. It returns a risk score out of 10, a risk label, and reasons for its assessment.

## Features
- Searches for common phishing-style phrases.
- Detects URL-like text.
- Flags links whose host appears to be an IPv4 address.
- Explains which indicators affected the score.
- Does not need an internet connection or third-party libraries.

## Setup and usage
1. Install Python 3.8 or newer.
2. Open a terminal in this folder.
3. Run:
   ```bash
   python phishing_email_detector.py
   ```
4. Paste the message text.
5. Type `END` on its own line and press Enter.

## Sample test
Paste:
```text
URGENT! Your account suspended. Verify your account now at http://192.0.2.10/login!!!
END
```
The tool should flag suspicious wording, a link, an IP-address host, and repeated exclamation marks. Scores depend on the rules in the source code.

## Files
- `phishing_email_detector.py` — main Python program
- `requirements.txt` — dependency list
- `README.md` — project instructions
- `Project_Report.docx` — project report
- `Phishing_Email_Detector.ipynb` — notebook version with a demo test

## Limitations
This is a simple educational rule-based detector, not a production security product. It does not verify sender identity, inspect attachments, visit websites, or use machine learning. It can produce false positives and false negatives. A low score does not prove that a message is safe.

## Safety
Never open a suspicious link just to test it. Do not enter passwords, OTPs, or bank details on a page reached from an unexpected message.
