# Multimedia-Security-using-Encryption
A project that implements encryption techniques to secure multimedia files and prevent unauthorized access.
# Multimedia Security using Encryption

## Overview

This project demonstrates a secure multimedia protection approach by combining **AES encryption** and **LSB steganography**. A secret text message is encrypted using AES and then hidden inside an image using Least Significant Bit (LSB) embedding. The project also evaluates image quality after embedding using PSNR, MSE, and SSIM metrics.

## Problem Statement

With the increasing exchange of digital multimedia data, protecting sensitive information from unauthorized access is critical. Traditional encryption secures data but does not conceal its existence. This project addresses the need for both **data confidentiality** and **data invisibility**.

## Objectives

* To encrypt sensitive text data using AES encryption
* To hide encrypted data inside an image using LSB steganography
* To extract and decrypt the hidden message accurately
* To evaluate image quality after data embedding

## Technologies Used

* Python
* OpenCV (cv2)
* NumPy
* PyCryptodome (AES, SHA256)
* PIL (Python Imaging Library)
* Matplotlib
* SSIM-PIL

## Methodology

1. Load and resize the input image
2. Encrypt the secret message using AES with a SHA-256 generated key
3. Convert encrypted data into hexadecimal format
4. Embed encrypted data into the image using LSB technique
5. Extract the hidden data from the image
6. Decrypt the extracted data to retrieve the original message
7. Evaluate image quality using PSNR, MSE, and SSIM

## Encryption Technique

AES (Advanced Encryption Standard) is used to encrypt the secret message. A SHA-256 hash function generates a secure encryption key. The encrypted message ensures confidentiality even if the hidden data is detected.

## Steganography Technique

Least Significant Bit (LSB) steganography embeds encrypted data into the least significant bits of image pixels. This method ensures minimal visual distortion while securely hiding information.

## Performance Metrics

* **MSE (Mean Squared Error):** Measures pixel-level differences between original and stego image
* **PSNR (Peak Signal-to-Noise Ratio):** Evaluates image quality after embedding
* **SSIM (Structural Similarity Index):** Measures structural similarity between original and stego image

## Results

The encrypted data is successfully embedded and extracted without noticeable visual changes. High PSNR and SSIM values indicate good image quality and effective data hiding.

## Applications

* Secure image-based communication
* Digital watermarking
* Multimedia data protection
* Cyber security and forensics

## Limitations

* Limited data embedding capacity
* Uses ECB mode which is less secure for large data
* Designed for educational and demonstration purposes

## Future Enhancements

* Implement CBC or GCM mode for stronger encryption
* Extend support to audio and video files
* Improve embedding capacity and robustness
* Develop a GUI-based application

## Conclusion

This project successfully integrates encryption and steganography to provide enhanced multimedia security. By combining AES encryption with LSB image embedding, the system ensures both data confidentiality and invisibility while maintaining image quality.
