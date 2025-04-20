# Secure Two-Person Chat Application

## Overview

This project is a secure, encrypted chat application designed for two users to communicate privately. Messages are encrypted using a shared secret key, ensuring that only users with the key can decrypt and read the conversation. The application features a clean, user-friendly interface with options to save and load chat histories.

## Features

- **End-to-End Encryption**: Messages are encrypted using a shared secret key
- **Dual User Interface**: Separate input fields for User 1 and User 2
- **Message History**: View complete conversation history in the chat window
- **Data Persistence**:
  - Save entire chat history to a text file
  - Load previous conversations from saved files
- **Security Controls**:
  - Set/reset encryption key
  - Toggle between encrypted and decrypted views
- **Responsive Design**: Clean, modern interface that works on desktop browsers

## Technical Details

### Encryption Method
- Uses Base64 encoding combined with URI component encoding
- Requires a shared secret key for encryption/decryption
- Simple but effective obfuscation of message content

### User Interface
- Clear visual distinction between User 1 and User 2 messages
- Smooth animations for message display
- Intuitive controls for all functions

## Installation

This is a client-side web application that requires no server installation. To use:

1. Download the `index.html` file
2. Open it in any modern web browser (Chrome, Firefox, Edge, Safari)
3. No additional dependencies or installations needed

Alternatively, you can host this on any web server by simply uploading the HTML file.

## Usage Instructions

1. **Set Encryption Key**:
   - Enter a shared secret key in the "Enter shared secret key" field
   - Click "Set Key" to activate encryption

2. **Sending Messages**:
   - User 1 types in the top input field and clicks "Send as User 1"
   - User 2 types in the bottom input field and clicks "Send as User 2"

3. **Viewing Messages**:
   - Encrypted messages appear in the chat box
   - Click "Decrypt Chat" to view decrypted messages (requires correct key)

4. **Saving/Loading**:
   - Click "Save Chat" to download conversation history
   - Click "Load Chat" to upload a previously saved conversation
   - Click "Reset Chat" to clear the current conversation

## Security Considerations

- The encryption provided is basic and should not be considered military-grade
- For truly sensitive communications, consider more robust encryption methods
- Always share the secret key through a secure channel
- The application runs entirely client-side - no messages are sent to any server

## Screenshots

(Include screenshots showing:)
1. The interface with encrypted messages
2. The decrypted chat view
3. The save/load functionality in action

## Browser Compatibility

Tested and works on:
- Google Chrome (latest)
- Mozilla Firefox (latest)
- Microsoft Edge (latest)
- Safari (latest)

## Limitations

1. Encryption is not industrial-strength (uses Base64 + key combination)
2. No user authentication - anyone with access to the HTML file can use it
3. No network functionality - users must be on the same machine or share files
4. No message timestamps in the saved chat history

## Future Enhancements

- [ ] Implement more robust encryption (AES)
- [ ] Add network functionality for real-time communication
- [ ] Include message timestamps
- [ ] Add user authentication
- [ ] Implement message history search
- [ ] Add multi-language support
- [ ] Create mobile-friendly version

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for:
- Security improvements
- UI/UX enhancements
- New features
- Bug fixes

## License

[MIT License](LICENSE)

## Acknowledgments

- Base64 encoding/decoding functions using native browser APIs
- Modern CSS techniques for responsive design
- HTML5 File API for save/load functionality
