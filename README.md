# GonnaCry Rasomware 
Original Repository of the GonnaCry Ransomware.

This project is OpenSource, feel free to use, study and/or send pull request.

GonnaCry is a linux ransomware that encrypt all user files with strong encryption scheme.

There is two versions of the Ransomware Code: <a href="https://github.com/tarcisio-marinho/GonnaCry/tree/master/C">C</a> and <a href="https://github.com/tarcisio-marinho/GonnaCry/tree/master/Python">Python</a>.
    
-------------

**How this ransomware works:**

https://0x00sec.org/t/how-ransomware-works-and-gonnacry-linux-ransomware/4594

https://medium.com/@tarcisioma/how-ransomware-works-and-gonnacry-linux-ransomware-17f77a549114

**How this ransomware encryption scheme works:**

https://medium.com/@tarcisioma/ransomware-encryption-techniques-696531d07bb9

**Mentions:**

https://www.sentinelone.com/blog/sentinelone-detects-prevents-wsl-abuse/

https://hackingvision.com/2017/07/18/gonnacry-linux-ransomware/

https://www.youtube.com/watch?v=gSfa2L158Uw



[![Travis branch](https://img.shields.io/travis/rust-lang/rust/master.svg)](https://github.com/tarcisio-marinho/GonnaCry)
[![Travis branch](https://img.shields.io/cran/l/devtools.svg)](https://github.com/tarcisio-marinho/GonnaCry/blob/master/LICENSE)
[![Travis branch](https://img.shields.io/badge/made%20with-%3C3-red.svg)](https://github.com/tarcisio-marinho/GonnaCry)
[![Travis branch](https://img.shields.io/github/stars/tarcisio-marinho/GonnaCry.svg)](https://github.com/tarcisio-marinho/GonnaCry/stargazers)
    
-------------

# Disclaimer
This Ransomware musn't be used to harm/threat/hurt other person's computer.

It's purpose is only to share knowledge and awareness about Malware/Cryptography/Operating Systems/Programming.

GonnaCry is a academic ransomware made for learning and awareness about security/cryptography.


**Be aware running C/bin/GonnaCry or Python/GonnaCry/main.py Python/GonnaCry/bin/gonnacry in your computer, it may harm.**

-------------

# What's a Ransomware?

A ransomware is a form of malware that prevent legitimate users from accessing
their device or data and asks for a payment in exchange for the stolen functionality.
They have been used for mass extortion in various forms, but the
most successful seem to be encrypting ransomware: most of the user data are
encrypted and the key can be retrieved with a payment to the attacker.
To be widely successful a ransomware must fulfill three properties:

**Property 1**: The hostile binary code must not contain any secret (e.g. deciphering
keys). At least not in an easily retrievable form, indeed white box cryptography
can be applied to ransomware.

**Property 2**: Only the author of the attack should be able to decrypt the
infected device.

**Property 3**: Decrypting one device can not provide any useful information
for other infected devices, in particular the key must not be shared among them.

-------------

# Objectives:

- [x] encrypt all user files with AES-256-CBC.
- [x] Random AES key and IV for each file.
- [x] Works even without internet connection.
- [x] Communication with the server to decrypt Client-private-key.
- [x] encrypt AES key with client-public-key RSA-2048.
- [x] encrypt client-private-key with RSA-2048 server-public-key.
- [x] Change computer wallpaper -> Gnome, LXDE, KDE, XFCE.
- [x] Decryptor that communicate to server to send keys.
- [x] python webserver
- [x] Daemon
- [ ] Dropper
- [ ] Kill databases


