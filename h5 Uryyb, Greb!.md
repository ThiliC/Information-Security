## h2 Uryyb, Greb!

### Read and Summary.

#### x) 
- € Schneier 2015: Applied Cryptography: Chapter 1: Foundations.

**Terminology in Applied Cryptography**  
- **Sender and Receiver**: When a sender wants to send a message to a receiver, it must be secured to ensure that an eavesdropper cannot read the message.

**Message and Encryption**  
- A message is **plaintext** (also called clear text).
- The process of disguising plaintext to hide its substance, turning it into ciphertext, is called **encryption**.
- The encrypted message, unreadable without decryption, is called **ciphertext**.
- The art and science of securing messages is called **cryptography**.
- The art and science of breaking ciphertext is known as **cryptanalysis**.
- The overall study of secure communications, including both cryptography and cryptanalysis, is called **cryptology**.

**Example**:  
If a sender needs to send "HELLO" **(plaintext)**, it is encrypted to "IFMMP" **(ciphertext)**. The process of disguising the message to hide its meaning is called **encryption**. Securing the message is referred to as **cryptography**. If someone figures out that "IFMMP" means "HELLO," they are performing **cryptanalysis**. The overall study of securing and breaking codes is called **cryptology**.

  ![image](https://github.com/user-attachments/assets/54a04c91-8b44-4009-9ac5-78e5bdd16c7c)

**Reference** 
- https://www.oreilly.com/library/view/applied-cryptography-protocols/9781119096726/08_chap01.html#chap01-sec006
- https://www.uobabylon.edu.iq/eprints/publication_10_31871_49.pdf
---
#### PGP - Send Encrypted and Signed Message - gpg
Let's see how we can use PGP encyption with "gpg" tool. 
```
   sudo apt-get update
   sudo apt-get install gpg micro psmisc
  ```
- Generate Key pairs.
```
  gpg --gen-key
```
As Tero's instructions I gave the same details, 
 - full name. "Tero Karvinen DEMO KEY" 
 - email address "tero@example.com.invalid"
   gave empty passwords and confirmed.
![image](https://github.com/user-attachments/assets/4a2f4fab-efe1-48a3-9dcc-aa0ec57ff2a3)

- Now This is my keypair

![image](https://github.com/user-attachments/assets/38f228af-1818-4e38-91a9-c47d72f96685)
- Export public Key
```
 cd
 gpg --export --armor --output tero.pub
```
This is my public key

![image](https://github.com/user-attachments/assets/f119f7f2-e40a-4fc0-b48d-f7d61a7fa3a9)
![image](https://github.com/user-attachments/assets/4c4ed38a-4106-4b10-99c1-46c0f182ef6b)
![image](https://github.com/user-attachments/assets/684867f4-5ec5-454f-9ad5-54d79c1ba241)
![image](https://github.com/user-attachments/assets/bcd32ced-a326-4f25-88d9-e98019edd3b2)
![image](https://github.com/user-attachments/assets/f736a291-4d8e-4934-8370-c111d45a9db3)
![image](https://github.com/user-attachments/assets/b088a463-e854-43bc-856b-e4dae0929f3b)
![image](https://github.com/user-attachments/assets/623f025a-2cef-4276-939c-959a0290faf4)

- Alice Sends a Secret Message
  
![image](https://github.com/user-attachments/assets/df34cfaa-60e6-454c-b11b-f16a1e4c92f6)
to saveand quit the message --> ctrl+s and ctrl Q

- Encrypted message was generated.

![image](https://github.com/user-attachments/assets/49c5eb48-ab85-44f9-b0cd-e65d64d06a96)

- Tero Decrypts and Verifies the Message
  
![image](https://github.com/user-attachments/assets/e36b1319-6051-41a5-adaa-d85c670f5dfd)

#### O)
The frequency of the letters of the alphabet in English
The inventor of Morse code, Samuel Morse (1791-1872), needed to know this so that he could give the simplest codes to the most frequently used letters. He did it simply by counting the number of letters in sets of printers' type. The figures he came up with were:	

![image](https://github.com/user-attachments/assets/9f00fa74-cfaa-4ab4-9fba-c9ad92e8d796)

Further, for English, based on both historical data and linguistic analysis, the six most common letters are:

E,A,R,I,O,T

Explanation:
- E: The most common letter in the English language, occurring frequently in various word structures, both in vowels and endings (like "the," "be," "she").
- A: A fundamental vowel that appears in many basic words ("and," "apple," "cat").
- R: A highly frequent consonant used in common words like "are," "run," "red."
- I: Another common vowel seen in short words like "is," "it," and "in."
- O: A vowel that appears in many important words ("on," "not," "to").
- T: A consonant that is common in English due to its use in articles, pronouns, and verbs ("the," "to," "at").
- 
These letters are dominant in English text because they occur frequently in small, everyday words and are essential for sentence construction.

**Reference** - https://www3.nd.edu/~busiforc/handouts/cryptography/letterfrequencies.html
              - https://en.wikipedia.org/wiki/Letter_frequency

#### b) Open and cloudless Password Manager. 
**Reference** - https://www.passwordmanager.com/best-offline-password-managers/

I used **KeePassXC**
It is a powerful free suite of security tool for managing passwords. It includes security protocols and is updated constantly. All the feature are usable offline. Encyption and storage happends on the device and only decrypt by master password. 
No access loss to any features if we loss internet connections. It also can be directly run from a USB device. 

-Install KeePassXC
```
sudo apt update
sudo apt install keepassxc
```

![image](https://github.com/user-attachments/assets/e7aa2b73-38ad-430f-9d15-3744596cd9cb)

![image](https://github.com/user-attachments/assets/28f9f203-1840-4ad1-86ea-23639a19d573)

- In this need to **"Create New Database"** to create a new password vault. 
- Set master password. - This will be the only password the user need to remember. The strength of the password should be critical so that it protects all other stored passwords. 
- The database is stores locally on the machine, not in the cloud.


#### Why password manager is needed. 
- Many people reuse the same passwords in multiple accounts which easily leads to attacks.
  if one site/account fets hacked, the attackers can use the password to log into all the accounts. But password manager helps to create unique, strong passwords for each service, reducing the risk.

- Brute fore attack - trying many combinations to guess a password. By using the password manager, users make brute forcing extremly difficult. It can give passwords over 12 characters. 

- Phishing protections.- When using a password manager prevents the "auto fill" loging informations.
- Password Leaks and Data Breaches - Attackers might try your stolen password elsewhere. Since password managers encourages unique passwords for each service, a breach at one site won’t affect others.





