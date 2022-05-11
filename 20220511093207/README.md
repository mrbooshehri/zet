# Use encrypt password in bash script

1. Install ```openssl``
1. Encrypt on the command line
```bash
echo 'MY_STRONG_PASSWORD' | openssl enc -aes-256-cbc -md sha512 -a -pbkdf2 -iter 100000 -salt -pass pass:'DIFFERENT_VISIBLE_PASSWORD' > .secret.vault.txt
```
- **enc -aes-256-cbc:** The encoding type. We’re using the Advanced Encryption Standard 256-bit key cipher with cipher-block chaining.
- **md sha512:** The message digest (hash) type. We’re using the SHA512 cryptographic algorithm.
- **a:** This tells openssl to apply base-64 encoding after the encryption phase and before the decryption phase.
- **pbkdf2:** Using Password-Based Key Derivation Function 2 (PBKDF2) makes it much more difficult for a brute force attack to succeed in guessing your password. PBKDF2 requires many computations to perform the encryption. An attacker would need to replicate all of those computations.
- **iter 100000:** Sets the number of computations that PBKDF2 will use.
- salt: Using a randomly applied salt value makes the encrypted output different every time, even if the plain text is the same.
- **pass pass:** ’DIFFERENT_VISIBLE_PASSWORD’: The password we’ll need to use to decrypt the encrypted remote password. Substitute DIFFERENT_VISIBLE_PASSWORD with a robust password of your choosing.

## Make the file accessible just for the user
```bash
chmod 600 secret.value.txt
```

## Decrypt where ever you want
```bash
cat .secret_vault.txt | openssl enc -aes-256-cbc -md sha512 -a -d -pbkdf2 -iter 100000 -salt -pass pass:'DIFFERENT_VISIBLE_PASSWORD'
```

Tags:
```
#script #safe_scripting 
```

Related:
```
* https://www.skafeed.com/how-to-use-encrypted-passwords-in-bash-scripts/
```
