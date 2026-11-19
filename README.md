# NETWORKWALKS-Bright-Arthur-B084-WK3-PM1-PM2-Password-Cracking
# Password Recovery Using John the Ripper and NetworkWalks Web Utilities 

## 1. Project Overview

This practical exercise explored how to assess password protection on PDF documents in a controlled learning environment. We used two approaches: a locally installed password-auditing tool with a graphical interface and a set of browser-based utilities provided by NetworkWalks.

The exercise highlights an important security concept: a password-protected document may still be vulnerable when its password is predictable. The strength of the password, rather than the presence of a password prompt alone, is an important part of protecting a file.

## 2. Learning Goals

The main goals of this activity were to:

- Become familiar with John the Ripper (JTR) and its Johnny graphical interface.
- Understand, at a high level, how a password hash can be obtained from a protected PDF for an authorised security assessment.
- Observe how a dictionary-based password audit tests candidate passwords against an extracted hash.
- Explore the Hash Calculator and Password Cracker utilities available on the NetworkWalks website.
- Confirm the result by opening the supplied practice document with the recovered password.
- Recognise why long, unique, and difficult-to-guess passwords are important.

## 3. Practical Exercise A — Using John the Ripper and Johnny

### Software and Resources

- John the Ripper 1.9.0 Jumbo (Windows 64-bit)
- Johnny 2.2 graphical interface (Windows)
- Online PDF hash extraction utility: `onlinehashcrack.com`
- **Practice document:** `My Locked PDF1.pdf` (267 KB)

### Procedure and Evidence

**1. Prepared the practice document and required applications**

The supplied PDF and the required software were downloaded and made available for the exercise.

<img width="1241" height="156" alt="image" src="https://github.com/user-attachments/assets/c51da5b6-44fb-4211-8ccc-4d9447b3a83c" />

<img width="892" height="57" alt="image" src="https://github.com/user-attachments/assets/6d361bd1-3913-4dbd-857c-04721254a7f8" />

**2.Installed and linked Johnny to the John the Ripper application**

Johnny was configured to use the John the Ripper executable. This allows the graphical interface to manage the password-auditing process.


**3. Obtained the PDF hash**

The PDF hash was extracted from the practice document. A hash is a transformed representation used by password-protection systems; it is not the original password itself.

![PDF hash extraction](screenshots/q3.png)

**4. Imported the hash into Johnny**

The extracted hash was loaded into Johnny so that the application could assess candidate passwords against it.

![Hash imported into Johnny](screenshots/q4.png)

**5. Conducted the password audit**

The password-auditing process was started, and the application identified a matching password candidate.

![Password audit result](screenshots/q5.png)

**6. Checked the result against the original document**

The recovered password was used to open the supplied PDF, confirming that the result worked for the practice file.

![PDF access verification](screenshots/q6.png)

**Outcome:** The password recovered for this training document was `good-luck`.

> **Note:** The screenshots document the stages of the exercise. The recovered password is included only as a result from this supplied practice file; do not publish passwords belonging to real users or confidential documents.
