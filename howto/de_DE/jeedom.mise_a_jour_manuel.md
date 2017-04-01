Wir werden hier sehen, wie man Jeedom manuell aktualisiert.

Voraussetzungen
===============

-   Sie wissen, wie Sie sich mit SSH in Jeedom einloggen können

-   das SSH Passwort kennen (siehe Installationsdokumentation)

-   Sie haben Internet auf der Jeedombox

> **Important**
>
> Denken Sie daran, vor jeder manuellen Aktualisierung ein Backup zum wiederherstellen zu machen.

Herunterladen und Entpacken
===========================

En SSH, faites :

    sudo su -
    cd /root
    wget https://github.com/jeedom/core/archive/stable.zip
    unzip stable.zip
    cp -R core-stable/* /var/www/html

Update Durchführung
===================

Toujours en SSH:

    sudo su -
    php /var/www/html/install/install.php mode=force
    chmod 775 -R /var/www/html
    chown www-data:www-data -R /var/www/html

> **Important**
>
> Wenn Ihre Jeedom Installation etwas älter ist, ersetzen Sie alle /var/www/html Verzeichnis durch /usr/share/nginx/www/jeedom
