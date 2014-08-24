homebrew.mxcl.smbd
===================

**UPDATE**: A version of this plist is now available directly within the `samba` formula on homebrew. For installation instructions, follow `brew info samba`.

A simple property list (plist) file for use in `launchd`/`launchctl` on systems with samba installed via Homebrew.

Assumes that `smbd` is installed to */usr/local/sbin/smbd* and that `smb.conf` is installed to */usr/local/etc/smb.conf*.

## Installation
- Copy the *homebrew.mxcl.smbd.plist* file into your preferred *LaunchAgents* or *LaunchDaemons* folder. This is usually */Library/LaunchDaemons/* or */System/Library/LaunchDaemons/*.
- Make sure that the file is owned by root, as samba requires root privileges.
- Load the plist with `sudo launchctl load /path/to/file`. 

## License
Public domain. 
