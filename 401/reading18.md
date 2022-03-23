# Cryptography

## Encryption, Decryption & Hacking

[Source](https://www.khanacademy.org/computing/computers-and-internet/xcae6f4a7ff015e7d:online-data-security/xcae6f4a7ff015e7d:data-encryption-techniques/a/encryption-decryption-and-code-cracking)

Julius Caesar invented the `Caesar Ciper` for communicating with his allies.  
It can no longer be used to secure data, but it's simplicity allows for an easy introduction to encryption, decryption, and code cracking.

**Encrypting a message**:

`Caesar Cipher` is an alphabet shift. Original letters are replaced with a new letter depending on the shift amount.

Ex:

The alphabet is shifted by 6.

- Original Alphabet:  A B C D E F G
- Encrypted Alphabet: G H I J K L M

Encrypted word example:

S E C R E T  
Y K I X K Z

**Decrypting a message**:

You can decrypt an encrypted message when you know the shift

Simple example:

KL  
alphabet shifted by 3  
ABCDEFGHI  
DEFGHIJKL  
KL = hi

**Cracking the Cipher**:

"Code cracking"

When you don't know the shift and have to crack the cipher, there are three techniques:

- Frequency Analysis

  - Analyze frequency of letters in the message, compare them to the most popular/used letters in the language

- Known Plaintext

  - Plaintext is a term for an original unencrypted message. Knowing what a message starts with or contains at some point can help analyzing.

- Brute Force

  - Since there are only 25 possible shifts with the alphabet, a couple words could be compared and contrasted with each shift until one works.

## Ceasar Cipher

[Source](https://en.wikipedia.org/wiki/Caesar_cipher)

---

# Videos

## Cryptography Crash Course

[Source](https://www.youtube.com/watch?v=jhXCTbFnK8o)

---

# Additional Resources

## Introduction to Cryptography

[Source](https://thebestvpn.com/cryptography/)

**Polymorphism** - A cipher that makes a new set of results each time it is used. Each new encryption on the same data has different results.

Most common use is for encrypting software, computers, and cloud-based information.

Why Cryptography matters:

- Without cryptography, anything you send over the internet would be visible to anyone.

**The Four Types of Cryptography**:

Hashing

Symmetric Cryptography

Asymmetric Cryptography

Key Exchange Algorithms

**The Four Types of Cryptographic Functions**:

Authentication

Nonrepudiation

Confidentiality

Integrity

## How Computers Generate Random Numbers

[Source](https://www.howtogeek.com/183051/htg-explains-how-computers-generate-random-numbers/)

</br>

[<<<Back](README.md)