# Privacy Policy

**Last Updated**: Nov 6, 2025

We understand the importance you place on personal privacy and are committed to providing you with a secure and reliable recording environment. This Privacy Policy aims to clearly explain how we protect your data security and privacy when you use our recording application.

Our core principle is: **Your data belongs only to you**. All processing is done locally on your device. We do not collect, upload, or access any of your personal information or recording content.

---

### 1. We Do Not Collect Any Information

This application is designed to strictly follow the "Privacy by Design" principle, ensuring maximum protection of your privacy.

- **No Personal Identifiable Information Collection**: We do not request, record, or access any information that can identify you personally, such as your name, email address, phone number, or geographical location.

- **No Recording Content Access**: All your recording files and their content are stored entirely locally on your device. We or any third party cannot access, listen to, or analyze your recordings under any circumstances.

- **No Third-Party Tracking**: We do not integrate any third-party advertising, analytics, or tracking services (SDKs). This means your usage behavior will not be shared with any external entities.

- **No Internet Connection Required**: The core functions of the application (recording, storage, encryption) can all operate offline without an internet connection.

---

### 2. How We Protect Your Data Security

We provide you with a layered security model. Your regular recordings are stored locally in unencrypted form for quick access. For sensitive recordings that require higher security, we provide a "Safe" feature.

#### 1. The Safe: Your Private Data Fortress

- **Optional Enhanced Security**: You can choose to move any recording into the "Safe". Only recordings stored in the Safe will be encrypted.

- **Independent Access Control**: The Safe is protected by independent **Face ID / Touch ID or PIN code** authentication. This verification is only used to access the Safe and does not lock the entire application, ensuring convenience for daily use.

#### 2. Encryption Core: Secure Enclave & Elliptic Curve Cryptography (ECC)

When you choose to encrypt a recording (i.e., move it into the Safe), we use industry-leading encryption technology to protect it.

- **Secure Storage of Master Key**:
  
  - When the application is first launched, a unique master private key is generated within your device's **Secure Enclave**.
  
  - **Secure Enclave** is a hardware-based security coprocessor that ensures the master private key never leaves this hardware chip. No software (including this application and the operating system itself) can directly read or export it.
  
  - This master key is bound to your device and this application. If the application is deleted, this master key will be permanently destroyed.

- **Recording File Encryption Process**:
  
  - When you move a recording into the Safe, the system uses an **Elliptic Curve Cryptography (ECC) based key agreement mechanism (ECDH)**.
  
  - The system generates a temporary, one-time key pair for this encryption operation.
  
  - By performing key agreement between this temporary key and the master key stored in the Secure Enclave, a symmetric encryption key (AES-256-GCM) dedicated to encrypting this specific recording is derived.
  
  - This symmetric encryption key only exists briefly in memory and is immediately discarded after use. It is never stored.

#### 3. Data Encryption Standard: AES-256-GCM

- Each of your recordings in the Safe is independently encrypted using **AES-256-GCM**, one of the most powerful symmetric encryption algorithms currently available.

- GCM mode not only provides confidentiality (preventing eavesdropping) but also provides **authenticity verification**, effectively resisting data tampering.

**Summary**: Your regular recordings are stored locally for easy access, while your most important recordings can receive hardware-level security protection through the Safe. This hybrid encryption model of "Asymmetric Encryption (ECC) + Symmetric Encryption (AES)", combined with Secure Enclave, means that each encrypted recording has its own unique, dynamically generated encryption key, while the root of decrypting it all—the master key—is securely locked in hardware.

---

### 3. Network Permissions & In-App Purchases

To support the continued development of the application, we offer the option to unlock all premium features through a one-time purchase, which is valid for a lifetime.

- **Sole Purpose of Network Access**: The **only purpose** for which this application requests network access permissions is to communicate with the App Store to process your in-app purchase requests, verify purchase receipts, and restore purchases.

- **No Data Transmission**: We promise that network permissions will **never** be used to upload, synchronize, or analyze any of your personal information or recording data. All your data always remains on your local device.

---

### 4. Your Rights & Control

We firmly believe that users should have complete control over their data.

- **Full Ownership**: You have 100% ownership and control over all recording data you create (whether encrypted or not).

- **Access & Export Anytime**: You can access, play, and export your recordings within the application at any time.

- **Complete Deletion Right**: You can delete recordings from the application at any time. We also provide a recycle bin feature. After you confirm "Permanent Delete", the relevant files will be completely and irreversibly removed from your device.

---

### 5. Policy Changes

We may update this Privacy Policy from time to time to reflect changes in our services or legal requirements. We will notify you of any significant changes through in-app notifications. We recommend that you regularly review this policy to stay informed about the latest privacy protection measures.

---

### 6. Contact Us

If you have any questions, comments, or suggestions regarding this Privacy Policy, please contact us through the support channels within the application.
