# Naru
Naru is my personal [unofficial arch repository](https://wiki.archlinux.org/title/Unofficial_user_repositories) that contains patches which seem to take forever to be applied.  

## Add to your pacman
Import my gpg key to your pacman keyring:
```
pacman-key --keyserver keyserver.ubuntu.com --recv-keys 3C4D990D1EBA77F4
pacman-key --lsign-key 3C4D990D1EBA77F4
```

Then add this to the end of your `/etc/pacman.conf`:
```
[naru]
Server = https://naru.jhyub.dev/$repo
```

## Packages
* [sddm-naru](#sddm-naru) - +pamautounlock

### sddm-naru
* Original package: [sddm](https://archlinux.org/packages/extra/x86_64/sddm/)
* Version: 0.20.0
* Patches
    * +pamautounlock - Automatically unlock the keyring with passphrase entered on LUKS decryption if autologin is enabled. Applies this [PR](https://github.com/sddm/sddm/pull/1550).
