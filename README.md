# Secure Document Vault System

## Overview
Secure Document Vault System is a secure web-based platform designed to allow users to upload, store, manage, encrypt, sign, and verify sensitive digital documents securely.

The project focuses on implementing modern cybersecurity concepts and best practices including:
- Authentication & Authorization
- JWT Security
- OAuth Login
- Two-Factor Authentication (2FA)
- Role-Based Access Control (RBAC)
- AES-256 File Encryption
- SHA-256 Integrity Verification
- Digital Signatures
- HTTPS Secure Communication
- MITM Traffic Analysis using Wireshark

The system simulates a real-world enterprise secure document management platform.

---

# Features

## Authentication & User Management
- User Registration & Login
- Secure Password Hashing (bcrypt / Argon2)
- Password Policy Enforcement
- JWT-Based Authentication
- Google/GitHub OAuth Login
- Two-Factor Authentication (2FA)
- Logout Functionality

## Role-Based Access Control (RBAC)
### Admin
- Manage users
- Manage roles & permissions

### Manager
- Review uploaded documents
- Verify document integrity

### User
- Upload documents
- View personal documents
- Download documents
- Delete documents

---

# Secure Document Management
- Upload files securely
- Download documents
- Delete documents
- View document metadata
- File type validation
- File size validation

---

# Document Encryption
All uploaded documents are encrypted before storage using AES-256 encryption to ensure confidentiality and protect files from unauthorized access.

---

# Digital Signatures & Integrity Verification
For every uploaded document:
- Generate SHA-256 hash
- Create digital signature
- Store document signature securely
- Verify whether documents were modified after upload

---

# HTTPS Secure Communication
The application uses HTTPS certificates to secure communication between the client and server and prevent data interception.

---

# MITM Demonstration using Wireshark
The project includes a demonstration showing:
1. HTTP traffic capture
2. Exposure of sensitive data over HTTP
3. HTTPS traffic capture
4. How HTTPS encrypts transmitted data

---

# Technologies Used

## Frontend
- HTML
- CSS
- JavaScript
- Bootstrap / React (optional)

## Backend
- Node.js / Express.js (or any backend framework)

## Database
- MySQL / MongoDB

## Security Libraries
- bcrypt / Argon2
- JWT
- Passport.js OAuth
- Speakeasy / Google Authenticator
- Crypto libraries for AES encryption
- SHA-256 hashing libraries

## Tools
- Git & GitHub
- Postman
- Wireshark

---

# System Roles

| Role   | Permissions |
|--------|-------------|
| Admin  | Manage users and roles |
| Manager | Review and verify documents |
| User | Upload and manage personal documents |

---

# Project Structure

```bash
Secure-Document-Vault/
│
├── frontend/
├── backend/
├── database/
├── uploads/
├── encrypted_files/
├── screenshots/
├── wireshark/
├── README.md
└── package.json
