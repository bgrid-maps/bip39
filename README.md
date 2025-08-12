# BIP39 Wordlists

## 📄 Data Format

Each file contains a JSON array with exactly 2048 unique words:tory contains the official BIP39 (Bitcoin Improvement Proposal 39) wordlists in multiple languages, optimized for use in the **BGRID** mapping system.

## 📋 Description

BIP39 defines a standard for generating deterministic mnemonic phrases that can be used to generate cryptocurrency wallets. This repository provides the official wordlists in JSON format to facilitate their integration with the BGRID system.

## 🗂️ Repository Structure

```
wordlist/
├── bip39-cs.json    # Czech
├── bip39-en.json    # English
├── bip39-es.json    # Spanish
├── bip39-fr.json    # French
├── bip39-it.json    # Italian
├── bip39-ja.json    # Japanese
├── bip39-ko.json    # Korean
├── bip39-pt.json    # Portuguese
└── bip39-zh.json    # Chinese
```

## 🌍 Supported Languages

| Code | Language | File | Words |
|--------|--------|---------|----------|
| `cs` | Czech | `bip39-cs.json` | 2048 |
| `en` | English | `bip39-en.json` | 2048 |
| `es` | Spanish | `bip39-es.json` | 2048 |
| `fr` | French | `bip39-fr.json` | 2048 |
| `it` | Italian | `bip39-it.json` | 2048 |
| `ja` | Japanese | `bip39-ja.json` | 2048 |
| `ko` | Korean | `bip39-ko.json` | 2048 |
| `pt` | Portuguese | `bip39-pt.json` | 2048 |
| `zh` | Chinese | `bip39-zh.json` | 2048 |

## 📄 Formato de Datos

Each file contains a JSON array with exactly 2048 unique words:

```json
[
    "abandon",
    "ability",
    "able",
    "about",
    "above",
    ...
]
```

## 🚀 Usage in BGRID

These wordlists are used by the BGRID system for:

- Generation of mnemonic coordinates
- Encoding of geographic locations
- Spatial data mapping
- Word-based navigation systems

### Loading Example

```javascript
// Load English wordlist
const englishWords = require('./wordlist/bip39-en.json');

// Load Spanish wordlist
const spanishWords = require('./wordlist/bip39-es.json');

// Get word by index
const wordAtIndex = englishWords[42]; // "achieve"
```

## 🔧 Technical Specifications

- **Standard**: [BIP39](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki)
- **Format**: JSON Array
- **Encoding**: UTF-8
- **Words per language**: 2048
- **Indices**: 0-2047

## ✅ Validation

Each wordlist meets the following criteria:

- ✅ Exactly 2048 unique words
- ✅ Alphabetically sorted according to the language
- ✅ No problematic special characters
- ✅ Compatible with the official BIP39 standard

## 🔗 Related Links

- [BIP39 Specification](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki)
- [BGRID Documentation](https://github.com/kudelink/bgrid)
- [Mnemonic Code Converter](https://iancoleman.io/bip39/)

## 📝 License

This repository contains data from the BIP39 standard which is in the public domain. The code and repository structure are available under the MIT license.

## 🤝 Contributions

To report issues or suggest improvements:

1. Check that the issue hasn't been reported previously
2. Create an issue describing the problem or improvement
3. If it's a correction, ensure it complies with the BIP39 standard
