# To Verify a Hash of a file

Windows cmd
```
CertUtil -hashfile "your_file" SHA256
```
OhMy_more_letters11243242025.zip: SHA256
8d63ed49e34a22f9835d776032ad908ecbccf2d04b436b1079b5544594a54720

more_letters1212202412.zip: SHA256
6c59a4f786623fcb1bbd6cea9f3d7e714cf33873e5e43c2770728ff1da8ac79c

Songs-20241212T211044Z-001.zip: SHA256
a07cd59cf075623187de227bcae3042796e22761b6111b45dfb01f9c49a674e2

whatloveis_060820251240.zip: SHA384
b91f01e08be47613cce50816bd7d1d2d11a41f3552127ac5fd8107265c8d6ecb589d7623979a59bb1dbea3dae2340fbb

more_letters092220241343_a prophet of their own_reduced.zip: SHA384
732cb18adc230d21760fa477d2c7096e7f1e07654afb3618e236d1e455b91eb0a773ca7ba183be0e64893a2a96ac2aa6
  The reduced version of a prophet of their own

#12ff25_0728202516455.zip: SHA384
0b1df86455e7da0a41ec9b6c1c55634c84d8bac1a593d6bc53ede3acc294440e15bc84d795504502360a36c36f1126b6

#### songs/:

more_songs06082025.txt: SHA256
594a373b4f3ce727b46c7aa281cb845b3e71903566b5c6257e1ea376cef92c37

more_songs072820251703.txt: SHA256
09e45aee9fa1d6593398f423d5ac6a3aa09890a5b5630780af0df4fc0a4cb6c8




## L5// CertUtil -hashfile 'your_file' SHA256

When you have a file on your computer, it’s like having a digital document or a picture. Sometimes, you want to make sure that this file hasn’t been changed or messed with. That’s where a "hash" comes in.

A hash is like a unique fingerprint for your file. It’s a long string of letters and numbers that represents the contents of that file. If even a tiny bit of the file changes, the hash will look completely different.

Now, the command "CertUtil -hashfile 'your_file' SHA256" is a way to check that fingerprint. Here’s what it means:

CertUtil: This is a tool on your computer that helps you work with certificates and files.
-hashfile: This tells the tool that you want to create a hash for a specific file.
'your_file': This is where you put the name of the file you want to check.
SHA256: This is a specific type of hash algorithm, which is just a fancy way of saying it’s a method to create that unique fingerprint.
So, when you run this command, your computer will create a hash for the file you specified. You can then compare this hash to a previous one you saved. If they match, your file is exactly the same as before. If they don’t match, something has changed, and you might want to investigate further!


## Same result using different commands in various shells

The command `CertUtil -hashfile "your_file" SHA256` is used in Windows to compute the SHA-256 hash of a specified file. While the exact command may not have a direct equivalent in all Unix-like shells, you can achieve the same result using different commands in various shells. Here are the commands for some common shells:

### 1. **Bash / Bourne Again Shell (bash)**
```bash
sha256sum your_file
```

### 2. **Bourne Shell (sh)**
```sh
sha256sum your_file
```
(Note: `sha256sum` is typically available in most Unix-like systems, including those using `sh`.)

### 3. **C Shell (csh)**
```csh
sha256 your_file
```
(Note: You may need to install additional tools or use `sh` syntax.)

### 4. **TENEX C Shell (tcsh)**
```tcsh
sha256 your_file
```
(Note: Similar to `csh`, you may need to install additional tools.)

### 5. **Korn Shell (ksh)**
```ksh
sha256sum your_file
```

### 6. **Z Shell (zsh)**
```zsh
sha256sum your_file
```

### 7. **Fish Shell (fish)**
```fish
sha256sum your_file
```

### 8. **Dash**
```sh
sha256sum your_file
```

### Additional Notes:
- The command `sha256sum` is commonly available on Linux distributions and macOS. If it's not available, you may need to install the `coreutils` package or use an alternative tool.
- On macOS, you can also use:
  ```bash
  shasum -a 256 your_file
  ```
- On some systems, you might find other tools like `openssl` that can also compute SHA-256 hashes:
  ```bash
  openssl dgst -sha256 your_file
  ```

Make sure to replace `your_file` with the actual path to the file you want to hash.


## More Info

Here are commands for different terminal environments to find the hash of a file using various hashing algorithms:

### Windows Command Prompt
For SHA256:
```bash
CertUtil -hashfile "your_file" SHA256
```

For MD5:
```bash
CertUtil -hashfile "your_file" MD5
```

For SHA1:
```bash
CertUtil -hashfile "your_file" SHA1
```

### macOS Terminal
For SHA256:
```bash
shasum -a 256 your_file
```

For MD5:
```bash
md5 your_file
```

For SHA1:
```bash
shasum your_file
```

### Linux Terminal
For SHA256:
```bash
sha256sum your_file
```

For MD5:
```bash
md5sum your_file
```

For SHA1:
```bash
sha1sum your_file
```

### Notes:
- Replace `"your_file"` with the actual path and name of the file you want to check.
- Make sure to use the correct quotes based on your terminal (double quotes for Windows and no quotes for Linux/macOS if there are no spaces in the file name). 

These commands will generate the hash for the specified file using the chosen algorithm!

Got it! Here are the commands specifically for Bash or Zsh (common shell environments on macOS and Linux):

## Even More Info

Here are the commands specifically for Bash or Zsh (common shell environments on macOS and Linux):

### For SHA256
```bash
shasum -a 256 your_file
```

### For MD5
```bash
md5 your_file
```

### For SHA1
```bash
shasum your_file
```

### For SHA512
```bash
shasum -a 512 your_file
```

### For BLAKE2
If you have the `b2sum` command available:
```bash
b2sum your_file
```

### Notes:
- Replace `your_file` with the actual path and name of the file you want to check.
- If the file name contains spaces, make sure to wrap it in quotes, like `"your file with spaces.txt"`.

These commands will generate the hash for the specified file using the chosen algorithm in a Bash or Zsh terminal!
