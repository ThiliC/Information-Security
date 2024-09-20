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






