# MySecretsManager

A secure, single-file web application for managing passwords, secrets, tokens, and other sensitive information with AES-256 encryption.

## Features

- 🔐 **AES-256 Encryption**: All data is encrypted using the Web Crypto API with PBKDF2 key derivation
- 💾 **Import/Export**: Encrypted backup files with timestamps
- 🗂️ **Multiple Categories**: Organize secrets as Passwords, Tokens, Secrets, or Custom types
- 🔍 **Search & Filter**: Quickly find secrets with real-time search and category filters
- 🎲 **Password Generator**: Generate strong passwords with customizable options
- 📊 **Password Strength Indicator**: Visual feedback on password security
- 📋 **Copy to Clipboard**: One-click copying of sensitive values
- 🎨 **Modern UI**: Beautiful, responsive design that works on all devices
- 🔒 **Privacy First**: All data stored locally in browser with no external dependencies

## Getting Started

1. Open `MySecretsManager.html` in any modern web browser
2. Enter a master password to unlock the application
3. Start adding your secrets!

## Usage

### First Time Setup
- Open the application and enter a master password
- This password will be used to encrypt all your data
- **Important**: Remember your master password - there's no recovery option!

### Adding Secrets
1. Click "➕ Add Secret"
2. Select a category (Password, Token, Secret, or Custom)
3. Fill in the required information
4. Use the password generator for strong passwords
5. Click "💾 Save Secret"

### Managing Secrets
- **Search**: Type in the search box to filter secrets by name, username, URL, or notes
- **Filter**: Use category buttons to show only specific types
- **Copy**: Click "📋 Copy" to copy passwords/tokens to clipboard
- **Edit**: Click "✏️ Edit" to modify existing secrets
- **Delete**: Click "🗑️ Delete" to remove secrets (with confirmation)

### Import/Export
- **Export**: Click "💾 Export" to create an encrypted backup file with timestamp
- **Import**: Click "📁 Import" or use the login screen import to restore from backup
- Backups are encrypted with your master password
- Files are named: `secrets-backup-YYYY-MM-DDTHH-MM-SS.txt`

### Security
- All data is encrypted using AES-256-GCM
- Master password is never stored, only used for encryption/decryption
- Data is stored in browser's localStorage when locked
- Lock the app with "🔒 Lock" when done

## Security Features

- **Web Crypto API**: Uses browser's native cryptography (AES-256-GCM)
- **PBKDF2**: 100,000 iterations for key derivation
- **Salt & IV**: Unique salt and initialization vector for each encryption
- **No External Dependencies**: No CDNs or third-party services
- **Client-Side Only**: All encryption happens in your browser

## Browser Compatibility

Works in all modern browsers that support:
- Web Crypto API
- ES6+ JavaScript
- localStorage

Tested on: Chrome, Firefox, Safari, Edge

## Technical Details

- **Single File**: Entire application in one HTML file
- **No Server Required**: Pure client-side application
- **Offline Capable**: Works without internet connection
- **Responsive Design**: Mobile and desktop friendly

## Tips

1. **Use a strong master password** - it protects all your secrets
2. **Export regularly** - keep encrypted backups safe
3. **Don't share your master password** - it can't be recovered
4. **Use password generator** - create strong, unique passwords
5. **Lock when done** - always lock the app when stepping away

## License

This is a personal secrets manager application. 
