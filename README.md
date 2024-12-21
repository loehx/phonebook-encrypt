# Phonebook Encrypt

A simple text encryption tool that disguises encrypted data as a phonebook entry list.

## Demo

Try it live at: https://loehx.github.io/phonebook-encrypt

## How it Works

The encryption process:
1. Takes input text and an encryption key
2. Converts text to ASCII codes and applies a hash based on the key
3. Chunks the encrypted data into phone number-sized pieces
4. Generates random names and area codes
5. Formats output to look like phonebook entries:
   ```
   Name: +XX XXXX-XXXX
   ```

The decryption process:
1. Detects encrypted format based on structure
2. Extracts the encrypted chunks
3. Uses the key to reverse the encryption
4. Validates using embedded checksum
5. Returns original text if successful

## Usage

1. Enter text in the left textarea to encrypt
2. Enter an encryption key
3. Encrypted output appears on the right
4. To decrypt, paste encrypted text and enter the same key

## Features

- Simple text encryption/decryption
- Disguised output format
- Built-in checksum validation
- Copy/paste friendly format
- Mobile responsive design

## License

MIT License - Created by Alexander Löhn
