homebrew.mxcl.samba
===================

A simple property list (plist) file for use in `launchd`/`launchctl` on systems with samba installed via Homebrew.

Assumes that `smbd` is installed to */usr/local/sbin/smbd* and that `smb.conf` is installed to */usr/local/etc/smb.conf*.

## Installation
- Copy the *homebrew.mxcl.samba.plist* file into your preferred *LaunchAgents* or *LaunchDaemons* folder. This is usually */Library/LaunchDaemons/* or */System/Library/LaunchDaemons/*.
- Make sure that the file is owned by root, as samba requires root privileges.
- Load the plist with `sudo launchctl load /path/to/file`. 

## License
Public domain. 