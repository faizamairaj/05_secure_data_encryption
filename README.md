🔐 Secure Data Encryption App — Summary
Overview:
This is a user-friendly, secure web application built using Streamlit, designed to encrypt, store, and retrieve sensitive information safely using modern cryptographic techniques.

✅ Key Features:
🔒 AES Encryption with Fernet:

Uses symmetric encryption from the cryptography library to securely store user secrets.

The encryption key is auto-generated and stored securely in a .key file.

🔑 Password Protection:

Each secret is protected with a user-defined passkey, which is hashed using SHA-256 before storing.

This ensures that even if the database is compromised, the passkey remains secure.

🗄️ SQLite Database:

Secrets are saved in a local SQLite database (simple_data.db) with three fields: label, encrypted_text, and passkey.

👤 Unique Labels:

Each secret is associated with a unique label (like a username or identifier) to manage multiple entries safely.

📥 Store Secret:

Users can input a label, a secret message, and a passkey. The message is encrypted and stored securely.

📤 Retrieve Secret:

Users can input the label and passkey to decrypt and view their previously saved secret.

🧠 Smart Feedback:

User-friendly messages guide users through the process with emojis, success indicators, and error alerts (e.g., label already exists, incorrect passkey, etc.)

🧰 Technologies Used:
Python

Streamlit

SQLite3

Cryptography (Fernet)

Hashlib (SHA-256)

💡 Use Cases:
Personal password manager

Small encrypted note storage

API key or token vault

Educational demo for beginners in encryption or app security


