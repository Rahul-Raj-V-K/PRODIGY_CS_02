# PIXEL MANIPULATION FOR IMAGE ENCRYPTION
# Introduction to Pixel Manipulation for Image Encryption Using Python
Pixel manipulation for image encryption is a technique where the pixel values of an image are altered to transform the image into an encrypted form. This encrypted image should look significantly different from the original, making it difficult to interpret without the decryption key. The primary goal is to protect the image from unauthorized access by making the content unreadable without decryption.

# Basic Concept
In digital images, each pixel's color is represented by values of red, green, and blue (RGB). By modifying these pixel values based on a certain key, we can encrypt the image. The same key can be used in reverse to decrypt the image, restoring it to its original form.

# Encrypt Function:
Opens an image and converts it to RGB format.
Converts the image to a numpy array for easy pixel value manipulation.
Adds the encryption key to each pixel value (with modulo 256 to handle overflow).
Saves the modified image as the encrypted image.
# Decrypt Function:
Opens the encrypted image and converts it to RGB format.
Converts the image to a numpy array.
Subtracts the encryption key from each pixel value (with modulo 256 to handle underflow).
Saves the restored image as the decrypted image.
