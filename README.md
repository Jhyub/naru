# Naru
Naru is my personal [unofficial arch repository](https://wiki.archlinux.org/title/Unofficial_user_repositories) that contains patches which seem to take forever to be applied.  

# Add to your pacman
server is not ready yet.

# Packages
* [sddm](#sddm) - +pamautounlock

## sddm
* Original package: [sddm](https://archlinux.org/packages/extra/x86_64/sddm/)
* Version: 0.19.0
* Patches
    * +pamautounlock - Automatically unlock the keyring with passphrase entered on LUKS decryption if autologin is enabled. Applies this [PR](https://github.com/sddm/sddm/pull/1550).
