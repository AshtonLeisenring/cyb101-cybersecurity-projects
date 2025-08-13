# Week 2 – SSH keys, encryption, and commit signing

Summary
Describe the goal in your own words. Example: generate an SSH key pair, use it for auth, encrypt and decrypt a file with openssl, and sign a git commit using an SSH signing key.

Tools used
ssh-keygen, ssh, scp, openssl, git

What I did
1) Generated 4096 bit RSA key with a comment
   Command example: ssh-keygen -t rsa -b 4096 -C "Ubuntu key"
2) Used the key for authentication
   Example: ssh -i ~/.ssh/id_rsa user@host
3) Encrypted and decrypted a text file with openssl pkeyutl
   Example: openssl pkeyutl -encrypt ... and -decrypt ...
4) Signed a git commit and verified the signature
   Example: git commit --allow-empty -m "test" then git show --show-signature

Screenshots
Place here: screenshots/enc_dec.png and screenshots/git_signature.png

Notes and takeaways
- Private key stays private
- Commit signatures protect integrity
- Never expose private keys in screenshots
