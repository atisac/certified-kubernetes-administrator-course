# TLS Basics
  - Take me to [Video Tutorial](https://kodekloud.com/topic/tls-basics/)
  
In this section, we will take a look at TLS Basics

## Certificate
- A certificate is used to guarantee trust between 2 parties during a transaction.
For example: when a user tries to access the web server, TLS certificates ensure that the communication between them is encrypted.

So you must encrypt your data using an encryption key. the data is encrypted using a key which is basically a set of random numbers and alphabets. 
You add the random number into the data and encrypt it into a format that cannot recognized 
 and then sent it to the server.
 The hacker sniffing the network gets the data but cannot do anything with it. However same is the case with the server receiving the data it can not decrypt the  data without a key. So the copy of the key must be sent to the server
  ![cert1](../../images/cert1.PNG)
  
  
## Symmetric Encryption
- It is a secure way of encryption, but it uses the same key to encrypt and decrypt the data and the key has to be exchanged between the sender and the receiver, there is a risk of a hacker gaining access to the key and decrypting the data.

  ![cert2](../../images/cert2.PNG)
  
## Asymmetric Encryption
- Instead of using single key to encrypt and decrypt data, asymmetric encryption uses a pair of keys, a private key and a public key.

  ![cert3](../../images/cert3.PNG)
  
  ![cert4](../../images/cert4.PNG)
  
  ![cert5](../../images/cert5.PNG)
  
  ![cert6](../../images/cert6.PNG)
  

#### How do you look at a certificate and verify if it is legit?
- who signed and issued the certificate.
- If you generate the certificate then you will have it sign it by yourself; that is known as self-signed certificate.

  ![cert7](../../images/cert7.PNG)
  
#### How do you generate legitimate certificate? How do you get your certificates singed by someone with authority?
- That's where **`Certificate Authority (CA)`** comes in for you. Some of the popular ones are Symantec, DigiCert, Comodo, GlobalSign etc.

  ![cert8](../../images/cert8.PNG)
  
  ![cert9](../../images/cert9.PNG)
  
  ![cert10](../../images/cert10.PNG)
  
## Public Key Infrastructure
   
   ![pki](../../images/pki.PNG)
   
## Certificates naming convention

  ![cert11](../../images/cert11.PNG)
  
  

  
   

  
  
  

  
  
  
  
  
  

  
  
