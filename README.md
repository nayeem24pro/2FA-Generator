# 2FA TOTP Generator

A simple, lightweight, browser-based TOTP (Time-Based One-Time Password) generator for Facebook, Instagram, and other services that support RFC 6238 compatible 2FA authentication.

## Features

- Generate 6-digit TOTP codes locally in your browser
- Supports Base32 secret keys
- Automatic code refresh every 30 seconds
- Visual countdown timer
- No server required
- No data transmission
- Mobile-friendly interface
- Works offline after loading

## Screenshot

Displays:
- Secret Key input field
- 6-digit authentication code
- Refresh countdown timer
- Security warning for users

## How It Works

1. Enter your Base32 2FA secret key.
2. The application decodes the secret key.
3. An HMAC-SHA1 hash is generated using the current time window.
4. A 6-digit TOTP code is displayed.
5. The code automatically refreshes every 30 seconds.

## Usage

### Option 1: Open Directly

Download or clone the repository and open:

```text
2fa-generator.html
```

in any modern web browser.

### Option 2: GitHub Pages

1. Upload the file to GitHub.
2. Enable GitHub Pages.
3. Open the generated Pages URL.

## Requirements

- Modern browser with Web Crypto API support
- Chrome
- Edge
- Firefox
- Safari

## Security

- All calculations happen locally in your browser.
- Secret keys are never sent to any server.
- No external libraries are used.
- No tracking or analytics.

### Important

Only enter your own 2FA secret keys.

Never share your secret key with anyone.

Facebook, Instagram, Google, or any legitimate service will never ask for your 2FA secret key.

## Project Structure

```text
.
├── 2fa-generator.html
└── README.md
```

## Technologies Used

- HTML5
- CSS3
- JavaScript (Vanilla)
- Web Crypto API

## Supported Services

Any service using standard TOTP authentication, including:

- Facebook
- Instagram
- Google
- GitHub
- Discord
- Binance
- X (Twitter)
- Dropbox
- Microsoft Accounts

## License

MIT License

Copyright (c) 2026 nayeem24pro

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files to deal in the Software without restriction.
