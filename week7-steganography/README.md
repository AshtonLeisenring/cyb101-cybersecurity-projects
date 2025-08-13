# Week 7 – Steganography with steghide

Summary
Embedded and extracted a hidden text message from a JPEG and verified via steghide info and extract.

Tools used
steghide, nano, file utilities

Steps
- Prepared a carrier image and a message file
- Embedded the message with a passphrase
- Verified with steghide info
- Extracted the hidden file and validated contents

Commands (examples)
steghide embed -ef message.txt -cf image.jpg
steghide info image.jpg
steghide extract -sf image.jpg -xf extracted.txt

Screenshots
Place here: screenshots/info.png and screenshots/extract.png

Notes
- Use lossless workflows when possible to avoid corrupting embedded data
- Keep passphrases secret
