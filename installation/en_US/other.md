You will find here the documentation to install Jeedom on most linux systems (tested and approved on the Debian distribution)

> **Important**
>
> Debian 8 est la distribution officiellement supportée, l’utilisation d’une autre distribution est à proscrire au risque d’obtenir comme réponse du support de devoir restaurer votre Jeedom sur une image officielle. Si vous ne maitriser pas un minimum les environnements Linux, nous vous conseillons de partir sur une image officielle (OVF) ou l’utilisation d’une Mini+ ou Smart (disponible prochainement).

Connectez-vous en SSH à votre système et faites :

    wget https://raw.githubusercontent.com/jeedom/core/stable/install/install.sh
    chmod +x install.sh
    ./install.sh

Il vous suffit ensuite d’aller sur IP\_MACHINE\_JEEDOM

> **Note**
>
> Les identifiants par défaut sont admin/admin

> **Note**
>
> Les arguments suivants sont utilisables : -v = version jeedom désirer -w = dossier webserver -z = installation dependances z-wave -m = mot de passe root mysql désiré

    ./install.sh -v x.y.zz -w /var/www/html -z -m Jeedom

Ensuite vous pouvez suivre la documentation [Premier pas avec Jeedom](https://www.jeedom.fr/doc/documentation/premiers-pas/fr_FR/doc-premiers-pas.html)
