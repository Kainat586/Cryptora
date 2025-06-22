# 🔐 Cryptora – Secure Messaging Platform

Cryptora is a **secure messaging web application** designed to protect sensitive communication through **multiple encryption and decryption techniques**. The project was developed as a part of an academic initiative to explore modern cryptographic approaches and ensure confidentiality, integrity, and control over shared data.

---

## 📌 Features

- ✅ **AES-256 Encryption/Decryption**
- ✅ **Password-Protected Secure Messaging**
- ✅ **QR Code Based Encrypted Message Sharing**
- ✅ **LSB & DCT Image Steganography**
- ✅ **Self-Destructing Messages (Time/Single View Based)**
- ✅ **Role-Based Access (Soldier / Officer / Admin)**
- ✅ **JWT-Based Session Authentication**
- ✅ **Email OTP Verification (initial version)**
- ✅ **User Activity and Logs (Admin Panel)**

---

## 🔧 Technologies Used

### Frontend
- HTML5 / CSS3 / JavaScript
- Tailwind CSS
- html5-qrcode (QR Code Scanning)

### Backend
- Node.js (Express.js)
- Crypto (AES Encryption/Decryption)
- QR Code Generator (`qrcode`)
- JWT Authentication
- Multer (for image processing)
- Sharp (for image compression)
- File System (`fs`) for message storage

---

## 🔐 Encryption Methods Used

### 🔸 AES-256-CBC
- Used for encrypting text and messages with user-provided password
- Format: `iv_in_hex:encrypted_base64`
- Key derived from password using SHA-256

### 🔸 Steganography
- **LSB (Least Significant Bit)**: Hide message in the pixel bits of PNG images
- **DCT (Discrete Cosine Transform)**: Embed message inside JPEG files via frequency coefficients

### 🔸 QR Code Encryption
- AES-encrypted messages are embedded inside QR codes
- QR codes can be scanned via webcam using html5-qrcode

---

## 🛡️ Roles & Access Control

- **Soldier**: Can receive and scan encrypted messages via QR code
- **Officer**: Can create, encrypt, and share messages
- **Admin**: Manages users, logs, roles, and system monitoring

---

## 📂 Project Structure

cryptora/
├── backend/
│ ├── controllers/
│ ├── routes/
│ ├── utils/
│ ├── models/
│ └── server.js
├── frontend/
│ ├── index.html
│ ├── encrypt.html
│ ├── decrypt.html
│ ├── styles/
│ └── js/
## 🚀 How to Run

### 1. Clone the repository
git clone https://github.com/your-username/cryptora.git
cd cryptora
2. Install backend dependencies
cd backend
npm install
npm start
cd ../frontend
# Open index.html manually or use Live Server
📝 Future Improvements
🔐 Add RSA or hybrid cryptography (AES + RSA)

🌍 Deploy on cloud (e.g., Render, Vercel, Netlify)

🖼️ Enhance steganography GUI

📱 Build mobile version (React Native / Flutter)

🙋‍♀️ Author
Kainat Khuram
BS Software Engineering '27, UET Lahore
Frontend Developer | InfoSec Enthusiast

📌 License
This project is for educational purposes only. All rights reserved © 2025.
