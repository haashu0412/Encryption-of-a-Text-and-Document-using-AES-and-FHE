Working

  Encryption:
    Encrypts both TXT & PDF files using AES-256
    Combines the AES-encrypted outputs into a single file
    Encrypts AES-encrypted TXT & PDF data using Fully Homomorphic Encryption (FHE)

  Decryption:
    This loads the FHE context (which includes the secret key) and decrypts the encrypted chunks
    Then load the AES-256 encryption key and decrypt the Base64 data
    Split the decrypted AES Base64 data into two parts (one for TXT, one for PDF)
    Decrypt each part using AES-256
    Save the restored data as a TXT file and a PDF file


