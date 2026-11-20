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
<img width="145" height="110" alt="jonny 2" src="https://github.com/user-attachments/assets/0613d5d0-bace-4b14-9009-36b4188c3e15" />

<img width="1132" height="1000" alt="jonny4" src="https://github.com/user-attachments/assets/a113ef0e-a75d-470e-a021-d8d86efa8c13" />

**3. Obtained the PDF hash**

The PDF hash was extracted from the practice document. A hash is a transformed representation used by password-protection systems; it is not the original password itself.

<img width="1022" height="757" alt="jonny 5" src="https://github.com/user-attachments/assets/54b29043-c3e9-4a00-be73-d117c2da0668" />

**4. Imported the hash into Johnny**

The extracted hash was loaded into Johnny so that the application could assess candidate passwords against it.


**5. Conducted the password audit**

The password-auditing process was started, and the application identified a matching password candidate.

<img width="972" height="1022" alt="jonny6" src="https://github.com/user-attachments/assets/8161101a-bdad-4215-a1d2-6914262a9e21" />

**6. Checked the result against the original document**

The recovered password was used to open the supplied PDF, confirming that the result worked for the practice file.

<img width="892" height="920" alt="jonny 7" src="https://github.com/user-attachments/assets/4a2108e2-6d8c-4752-b1ca-2348faea04db" />

**Outcome:** The password recovered for this training document was `good-luck`.


## 4. Practical Exercise B — NetworkWalks Online Utilities

### Tools and Practice File

- NetworkWalks Hash Calculator: `https://networkwalks.com/hash-calculator`
- NetworkWalks Password Cracker: `https://networkwalks.com/password-cracker`
- **Practice document:** [My Locked PDF2.pdf](https://github.com/user-attachments/files/35117931/My.Locked.PDF2.pdf)

### Procedure and Evidence

**1. Identified the correct PDF for the second exercise**

The designated practice document was selected before beginning the web-based assessment.

<img width="342" height="77" alt="image" src="https://github.com/user-attachments/assets/7a706505-b262-434f-a5df-fc1a1ba49ae0" />

**2. Generated the hash with the Hash Calculator**

The Hash Calculator generated the hash for the supplied PDF. This step prepares the information required by the password-auditing utility.
<img width="1067" height="925" alt="jonny 8" src="https://github.com/user-attachments/assets/d785f460-7712-4618-ad5f-8e6d8cb04ae7" />
**3. Submitted the extracted hash to the Password Cracker**

The resulting hash was transferred to the NetworkWalks Password Cracker for the next stage of the exercise.
<img width="937" height="605" alt="jonny8" src="https://github.com/user-attachments/assets/114996c5-8bf4-4e46-8543-518531fa61be" />

**4. Started the password assessment**

The web utility processed the submitted hash as part of the practical demonstration.

<img width="887" height="901" alt="jonny9" src="https://github.com/user-attachments/assets/cde57fb2-bef5-4d5f-a4fd-c4c0f6c3facf" />

**5. Reviewed the result**

The utility reported a successful password recovery for the supplied training document.
<img width="871" height="732" alt="jonny10" src="https://github.com/user-attachments/assets/6326cd70-e3eb-4c6d-9d48-8e3b39c630e9" />


**6. Validated access to the PDF**

I tested the recovered password by opening the original practice PDF. This final check helped confirm that the result was valid.

<img width="716" height="792" alt="jonny 10" src="https://github.com/user-attachments/assets/2b213609-8b73-40a6-a9a8-88f86be95838" />


## 5. What the Exercise Demonstrates

Although both practicals dealt with the same general concept, they used different working environments:

| Area | John the Ripper and Johnny | NetworkWalks web utilities |
|---|---|---|
| Working environment | Locally installed Windows applications | Browser-based tools |
| Hash preparation | PDF hash extracted using an online utility | Hash Calculator |
| Password assessment | John the Ripper managed through Johnny | NetworkWalks Password Cracker |
| Verification | Opened the supplied PDF with the recovered password | Opened the supplied PDF with the recovered password |

A password hash allows an auditing tool to test candidate passwords without simply reading the original password from the hash. In a dictionary-based assessment, candidate words and phrases are checked until a match is found or the available candidates are exhausted. A predictable password can therefore be much easier to recover than a long, unique one.

## 6. Key Lessons and Security Takeaways

- **Password predictability matters:** Common words, familiar phrases and simple patterns may be easier to guess during a password audit.
- **Hashing is not encryption:** A hash is a one-way representation used for verification. Password-auditing tools compare candidate passwords by processing them and checking for a match.
- **Different tools can demonstrate the same principle:** A desktop application and a browser-based utility can provide different interfaces for examining password strength.
- **Verification is important:** A reported match should be checked against the authorised practice document rather than accepted without confirmation.
- **Use unique passwords:** Reusing one password across multiple files or accounts increases the impact if that password is discovered.

## 7. Responsible Use and Practical Notes

- Carry out password assessments only on files you own or have clear permission to test.
- Use designated training documents and controlled lab environments.
- Avoid uploading confidential, personal, or business documents to third-party online services. Use approved tools and follow the relevant data-handling rules.
- Do not use recovered passwords to access another person's files or accounts.
- For important documents, use a long, unique password and store it securely.

## 8. Final Reflection

This week's practical work provided exposure to two approaches for examining the security of password-protected PDF files. Working with John the Ripper and Johnny introduced the locally installed tool workflow, while the NetworkWalks utilities demonstrated a browser-based alternative.

The key lesson is that password protection is only as dependable as the password chosen. A document protected with a predictable password may be at greater risk than one secured with a long and unique passphrase. The exercise also reinforced the importance of authorised testing, careful handling of files, and verification of results.
