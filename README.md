# RC4 Stream Cipher — Virtual Lab Simulation

An interactive, zero-backend **Virtual Labs** web simulation demonstrating the **RC4 (Rivest Cipher 4)** symmetric stream cipher, including step-by-step visualization of its 256-byte state array (`S-Box`), Key-Scheduling Algorithm (KSA), and Pseudo-Random Generation Algorithm (PRGA).


---

## Team Members
* **Akshaya C V**
* **Srinija C S G**
* **Tanisha S**

---

## About the Algorithm
**RC4 (Rivest Cipher 4)** is a symmetric stream cipher designed by Ron Rivest in 1987. Unlike block ciphers (such as AES or DES) that divide data into fixed-size blocks, RC4 encrypts and decrypts data **one byte at a time**, allowing it to handle inputs of any length or character set without padding.

### Core Phases
1. **Key-Scheduling Algorithm (KSA):** Initializes an identity permutation array `S[0..255]` and scrambles it using the secret key through 256 index swaps.
2. **Pseudo-Random Generation Algorithm (PRGA):** Mutates the state array `S` dynamically to generate one pseudo-random keystream byte (`K`) per byte of input data.
3. **Bitwise XOR ($\oplus$):**
   * **Encryption:** $C_i = P_i \oplus K_i$
   * **Decryption:** $P_i = C_i \oplus K_i$

---

## Features
* **100% Frontend Execution:** Built purely with HTML5, CSS3, and Vanilla JavaScript—no backend server or external dependencies required.
* **Interactive S-Box Visualizer:** Real-time $16 \times 16$ state matrix highlighting pointers (`i`, `j`, and `t`) during KSA and PRGA execution, with step-by-step and auto-play animation controls.
* **Universal Input Support:** Uses UTF-8 encoding (`TextEncoder`/`TextDecoder`) to encrypt and decrypt arbitrary text, numbers, whitespace, symbols, and emojis into Hexadecimal and Base64 formats.
* **RFC 6229 Verification:** Includes a one-click official IETF test vector preset to verify standard keystream output.
* **Complete Virtual Lab Modules:** Includes **Aim**, **Theory**, **Procedure**, **Simulation**, **Self-Evaluation Quiz**, and **References**.

---

## How to Run Locally
1. Clone or download this repository:
   ```bash
   git clone [https://github.com/Tanisha-Selva/RC4.git](https://github.com/Tanisha-Selva/RC4.git)
