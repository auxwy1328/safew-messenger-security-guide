# 🔒 SafeW Messenger Security Guide

<p align="center">
  <b>Complete security setup guide for SafeW encrypted messenger</b><br>
  Signal Protocol · ISO 27001 · End-to-End Encryption · Updated May 2026
</p>

---

## 📑 Table of Contents
- [Quick Security Setup](#-quick-security-setup-5-minutes)
- [Encryption Deep Dive](#-encryption-deep-dive)
- [2FA Setup Guide](#-2fa-setup-guide)
- [Privacy Configuration](#-privacy-configuration)
- [Recovery Codes](#-recovery-codes-management)
- [Full Tutorials](#-full-tutorials)
- [Security Checklist](#-security-checklist)

---

## ⚡ Quick Security Setup (5 Minutes)

```bash
Step 1: Enable Two-Factor Authentication
   Settings → Privacy & Security → Two-Step Verification → Set PIN

Step 2: Set Screen Lock
   Settings → Privacy → Passcode Lock → Create passcode

Step 3: Save Recovery Codes
   After enabling 2FA → Save recovery codes → Store in password manager

Step 4: Review Linked Devices
   Settings → Devices → Remove any unknown sessions

Step 5: Disable Message Previews
   Settings → Notifications → Show Preview → Off
```

## 🔐 Encryption Deep Dive

SafeW uses the **Signal Protocol** — the same battle-tested encryption used by Signal and WhatsApp.

```
                    Message Encryption Flow
┌─────────┐                                    ┌─────────┐
│ Sender  │──→ Double Ratchet ──→ X3DH ──→│Receiver │
└─────────┘       AES-256-CBC              └─────────┘
                  HMAC-SHA256
                  Curve25519
```

### Key Cryptographic Properties
| Property | Description |
|----------|------------|
| **Forward Secrecy** | Past messages safe even if key compromised |
| **Post-Compromise Security** | Future messages safe after key recovery |
| **Deniability** | No cryptographic proof of message origin |
| **Metadata Protection** | Sealed Sender hides who's messaging whom |

## 🔑 2FA Setup Guide

```python
# 2FA Security Levels

level_1 = "Password only"            # Basic, vulnerable to phishing
level_2 = "Password + SMS code"      # Better, but SIM-swap risk
level_3 = "Password + PIN"           # Good, offline verification
level_4 = "Password + Security Key"  # Best, hardware token required

# SafeW supports Level 3 & 4
```

### PIN Best Practices
- ❌ Don't use: birthday, phone number, "1234"
- ✅ Use: random 6-digit number
- ✅ Store in: 1Password / Bitwarden
- ❌ Don't store in: Notes app, screenshots

## 🛡️ Privacy Configuration

| Setting | Recommended | Why |
|---------|------------|-----|
| Profile Photo | Contacts Only | Prevent scraping |
| Last Seen | Nobody / Contacts | Privacy |
| Online Status | Same as Last Seen | Consistency |
| Group Invites | Contacts Only | Anti-spam |
| Voice Calls | Contacts Only | Anti-harassment |
| Read Receipts | Off (optional) | Privacy preference |

## 📝 Recovery Codes Management

```bash
# Recovery Code Storage (ranked by security)

1. Password Manager (1Password/Bitwarden)  ← Best
2. Encrypted local file (VeraCrypt)        ← Good  
3. Paper backup in safe place              ← Reliable
4. Split across trusted locations          ← Advanced

# NEVER store recovery codes in:
✗ Phone screenshot gallery
✗ Cloud notes (unencrypted)
✗ Email drafts
✗ WeChat/WhatsApp messages to yourself
```

## 📖 Full Tutorials

- **[SafeW 2FA Setup Complete Guide (2026)](https://safews.cn/safew-two-factor-authentication-guide-2026/)** — PIN, security key, recovery codes, real-world troubleshooting
- **[SafeW Download & Install All Platforms](https://safews.cn/safew-download-install-register-2026-3/)** — Windows, macOS, iOS, Android step-by-step
- **[SafeW vs Signal vs Telegram Comparison](https://safews.cn/safew-vs-signal-vs-telegram-comparison-2026/)** — Encryption, features, privacy compared

## ✅ Security Checklist

```
[ ] 2FA enabled with strong PIN
[ ] Recovery codes saved offline
[ ] Screen lock active
[ ] Unknown sessions terminated
[ ] Notification previews disabled
[ ] Profile photo → Contacts Only
[ ] Group invites → Contacts Only
[ ] App updated to latest version
[ ] Backup password saved separately
```

---

<p align="center"><sub>🛡️ Community-maintained · Not affiliated with SafeW · For educational purposes</sub></p>

## 🔗 Related Repositories
| Category | Repository |
|----------|-----------|
| Encrypted Messaging | [encrypted-messaging-apps-comparison](https://github.com/auxwy1328/encrypted-messaging-apps-comparison) · [encrypted-chat-apps-guide](https://github.com/auxwy1328/encrypted-chat-apps-guide) · [safew-messenger-security-guide](https://github.com/auxwy1328/safew-messenger-security-guide) · [telegram-power-user-guide](https://github.com/auxwy1328/telegram-power-user-guide) |
| Remote Desktop | [remote-desktop-tools-comparison](https://github.com/auxwy1328/remote-desktop-tools-comparison) · [remote-desktop-software-tools](https://github.com/auxwy1328/remote-desktop-software-tools) · [bitbrowser-fingerprint-guide](https://github.com/auxwy1328/bitbrowser-fingerprint-guide) |
| Productivity | [pdf-office-software-guides](https://github.com/auxwy1328/pdf-office-software-guides) · [sogou-input-method-tips](https://github.com/auxwy1328/sogou-input-method-tips) |
| Social Media | [social-media-app-tutorials](https://github.com/auxwy1328/social-media-app-tutorials) |
