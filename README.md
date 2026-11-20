# Research and analysis of GOG Galaxy Service Local Privilege Escalation.

The issue is caused by insecure DLL loading combined with weak directory permissions. An attacker can abuse the DLL search order to make `GalaxyCommunication.exe` load a malicious `IPHLPAPI.DLL` from a directory writable by a low-privileged user.

**Impact:** A local attacker can execute code with SYSTEM privileges.

## Demo

<!-- Add your PoC demonstration GIF or screenshot here -->

![PoC Demo](images/demo.gif)

## Custom PoC

[View Custom PoC →](custom-poc.md)

## References

Original PoC: https://github.com/0xv1n/gog-lpe-poc
