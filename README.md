# Image-Based Steganography

## Overview
This project implements a simple steganography technique to hide a secret message inside an image by modifying its pixel values. The message can be retrieved later using the correct passcode.

## Requirements
- Python 3.x
- OpenCV (`cv2`)

## Installation
1. Install Python 3 if not already installed.
2. Install OpenCV using pip:
   ```sh
   pip install opencv-python
   ```

## Usage

### Encryption
1. Place an image in the specified path.
2. Run the script and enter a secret message when prompted.
3. Provide a passcode for encryption.
4. The script modifies the image pixels to store the message.
5. An encrypted image named `encryptedImage.jpg` is created and opened automatically.

### Decryption
1. Run the script again.
2. Enter the correct passcode for decryption.
3. If the passcode matches, the secret message is extracted and displayed.

## Code Explanation
- The image is read using OpenCV.
- The message characters are converted into their ASCII values and embedded into pixel values.
- The modified image is saved as `encryptedImage.jpg`.
- The same process is used to extract the message if the correct passcode is entered.

## Notes
- The message length should be within the limit of available pixels.
- Image modifications may slightly alter its visual appearance.
- This is a basic implementation and does not provide high-level security.

## License
This project is open-source and can be modified as needed.

