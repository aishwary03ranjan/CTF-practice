# CTF Practice — Cryptography Tools

A collection of 17 Python scripts covering classical ciphers and encodings commonly seen in beginner CTF challenges. Built while learning cryptography fundamentals and preparing for CTF-style problem solving.

## Files

### Caesar Cipher (5 versions)
- Caesar Cipher ASCII decoder — decodes using ASCII arithmetic, handles upper/lower case separately
- Caesar Cipher lower() and decoder — decodes using alphabet string position lookup
- Caesar Cipher all shift decoder — brute forces all 26 possible shifts when the key is unknown
- Caesar Cipher encode+decode — single function handling both encryption and decryption
- Caesar Cipher encode after reversing — reverses the message before applying the cipher, an original variation

### ROT13 (3 versions)
- Implementing ROT13 through python built in codecs — uses Python's built-in codecs module
- ROT13 encode and verify — manual implementation that verifies encoding twice returns the original message
- ROT13 with frequency analysis — applies ROT13 and analyses letter frequency in the output, a real cryptanalysis technique

### Vigenère Cipher (3 versions)
- Vigenère Cipher to encode and decode — single function handling both modes using a repeating keyword
- Vigenère Cipher Brute force — tries common CTF keywords automatically when the key is unknown
- Vigenère Chiper decoder through alphabet — decodes using alphabet string position lookup

### Base64 (3 versions)
- Base64 decode only — straightforward decoder, the most common CTF use case
- Base64 multiple round decoder — decodes Base64 that has been encoded multiple times in a row
- Base64 detect and decode — automatically detects whether a string is valid Base64 and decodes or encodes accordingly

### XOR Cipher (3 versions)
- XOR basic single character key — encodes and decodes using a single character key
- XOR multi character key — uses a multi-character key that cycles like Vigenère, output shown in hex
- XOR hex input decoder — decodes XOR-encoded hex strings, the format most commonly given in CTFs

## About

My name is Aishwary Ranjan. I am a Class XII graduate (2026) with a strong interest in mathematics and cybersecurity. I scored 95.15 percentile in JEE Mains and 89 marks in JEE Advanced 2026, which sparked my curiosity towards cryptography and its mathematical foundations.

I built this repository as part of my cybersecurity learning journey, starting from classical ciphers and progressing towards CTF challenge preparation. I am also actively learning through TryHackMe and CyLab Security Academy (picoCTF).

## What I learned

- How classical ciphers (Caesar, Vigenère) use modular arithmetic to shift letters
- The difference between encoding (Base64), encryption (ciphers), and bitwise operations (XOR)
- How to brute force unknown keys when no key is given, a core CTF skill
- How frequency analysis can be used to crack ciphers without knowing the key
- Practical Python skills: string manipulation, ASCII/character conversion, and working with hex and bytes
