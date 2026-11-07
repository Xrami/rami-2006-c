# RSA Encryption Tool

**Version 8 — Python Cryptography Project**

## Overview

RSA Encryption Tool is a Python-based cryptography project that demonstrates RSA key generation and message encryption using large prime numbers.

The project generates RSA parameters, calculates the public exponent, encrypts a message, and saves the resulting values to a text file.

## Features

- Generates two large prime numbers (1048 bits each).
- Calculates the RSA modulus (`n`).
- Computes Euler's totient function (`φ(n)`).
- Generates a private exponent (`d`) using a 256-bit prime number.
- Calculates the public exponent (`e`) using modular inversion.
- Encrypts messages using modular exponentiation.
- Exports encryption results to `message.txt`.

## Cryptographic Process

The tool follows these steps:

1. Generate two large prime numbers: `p` and `q`.
2. Calculate the modulus:

   `n = p × q`

3. Calculate Euler's totient:

   `φ(n) = (p - 1) × (q - 1)`

4. Generate the private exponent `d`.
5. Calculate the public exponent:

   `e = d⁻¹ mod φ(n)`

6. Convert the plaintext message into an integer.
7. Encrypt the message:

   `c = mᵉ mod n`

8. Save the generated values into `message.txt`.

## Requirements

- Python 3
- PyCryptodome

## Installation

Install the required library:

```bash
pip install pycryptodome
```

## Usage

Clone the repository:

```bash
git clone https://github.com/Xrami/rami-2006-c.git
```

Navigate to the project directory:

```bash
cd rami-2006-c
```

Run Version 8:

```bash
python3 "encryption(8).py"
```

## Output

After execution, the program generates:

`message.txt`

The file contains:

- `n` — RSA modulus
- `e` — Public exponent
- `c` — Encrypted ciphertext

## Project Versions

This repository contains eight sequential versions of the encryption project, representing its development over time.

- Version 1
- Version 2
- Version 3
- Version 4
- Version 5
- Version 6
- Version 7
- Version 8 (Latest)

## Disclaimer

This project is intended for educational purposes and cryptography experimentation.

The implementation is a learning demonstration and should not be considered production-ready encryption software.

---

**Author:** Xrami  
**Language:** Python  
**Category:** Cryptography / RSA  
**Latest Version:** V8
