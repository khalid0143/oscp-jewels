# smb

## Samba v3.0.20 / 3.x

```
read https://0xdf.gitlab.io/2019/02/21/htb-legacy.html

https://www.exploit-db.com/exploits/16320
https://github.com/amriunix/CVE-2007-2447
https://gist.github.com/joenorton8014/19aaa00e0088738fc429cff2669b9851
```

## SambaCry

```
https://github.com/opsxcq/exploit-CVE-2017-7494
https://github.com/joxeankoret/CVE-2017-7494
(msf)linux/samba/is_known_pipename
set SMB::AlwaysEncrypt false
set SMB::ProtocolVersion 1
```

## srv2.sys SMB Code Execution MS09-050

```
Check MS09-050 in windows
[windows exploits](:/1cd2495e7c114135b2a16848042f6f30)
```

## SMB version

```
# server type: 0x9a03
# v 2.2.x
https://github.com/offensive-security/exploitdb/blob/master/exploits/linux/remote/7.pl

# server type: 0x809a03
# v 3.0.24
https://github.com/mikaelkall/HackingAllTheThings/tree/master/exploit/linux/remote/CVE-2010-0926_smb_symlink_traversal
$ gcc CVE-2010-0926.c -o exploit
$ ./exploit 10.11.1.136 "<SHARE>" /kashz /
Attempt to access / through symlink /kashz from Windows or smbclient.
```