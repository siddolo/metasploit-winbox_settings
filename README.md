# Metasploit - winbox_settings

Post module for Metasploit to extracts Mikrotik Winbox credentials saved in the "settings.cfg.viw" file when the "Keep Password" option is selected in Winbox.

This repository is obsolete. The module is now part of [metasploit](https://github.com/rapid7/metasploit-framework)!

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

## Author

[Pasquale 'sid' Fiorillo](https://www.pasqualefiorillo.it/)

Thanks to [ISGroup](https://www.isgroup.biz/) :heart:

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/F1F3SGS48)
