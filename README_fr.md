# Misskey pour YunoHost

[![Niveau d'intégration](https://dash.yunohost.org/integration/misskey.svg)](https://dash.yunohost.org/appci/app/misskey) ![](https://ci-apps.yunohost.org/ci/badges/misskey.status.svg) ![](https://ci-apps.yunohost.org/ci/badges/misskey.maintain.svg)  
[![Installer Misskey avec YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=misskey)

*[Read this readme in english.](./README.md)*
*[Lire ce readme en français.](./README_fr.md)*

> *Ce package vous permet d'installer Misskey rapidement et simplement sur un serveur YunoHost.
Si vous n'avez pas YunoHost, regardez [ici](https://yunohost.org/#/install) pour savoir comment l'installer et en profiter.*

## Vue d'ensemble

Misskey est une plateforme de microblogging décentralisée. Puisqu'il existe au sein du Fediverse (un univers où diverses plateformes de médias sociaux sont organisées), il est mutuellement lié à d'autres plateformes de médias sociaux.

**Version incluse :** 12.110.1~ynh1



## Captures d'écran

![](./doc/screenshots/screenshot-desktop.png)

## Avertissements / informations importantes

### Points importants à lire avant l'installation

- *Misskey* nécessite un domaine racine dédié, par ex. `misskey.domain.tld`
- En raison de la dépendance de Cypress, *Misskey* ne fonctionne que sur les machines à processeur 64 bits.
- *Misskey* peut prendre un certain temps à installer (plus de 30 minutes). Alors prenez un peu de temps et prenez un café.
- Si l'installation à partir de la ligne de commande, l'utilisation de l'écran est réenregistrée pour éviter la déconnexion. Voir ci-dessous.
- Après l'installation, la première page peut prendre du temps à charger et peut afficher une erreur de délai d'attente. Donnez-lui le temps de se préparer pour vous. Actualiser la page après 2-3 minutes.
- Le premier compte créé sera un utilisateur administrateur et disposera de tous les droits d'administrateur.

Utiliser *screen* en cas de déconnexion

``` 
sudo apt-get install screen
screen
sudo yunohost app install https://github.com/YunoHost-Apps/misskey_ynh.git
```
Récupérer après déconnexion :
```
screen -d
screen -r
```

## Documentations et ressources

* Site officiel de l'app : https://misskey-hub.net/
* Dépôt de code officiel de l'app : https://github.com/misskey-dev/misskey
* Documentation YunoHost pour cette app : https://yunohost.org/app_misskey
* Signaler un bug : https://github.com/YunoHost-Apps/misskey_ynh/issues

## Informations pour les développeurs

Merci de faire vos pull request sur la [branche testing](https://github.com/YunoHost-Apps/misskey_ynh/tree/testing).

Pour essayer la branche testing, procédez comme suit.
```
sudo yunohost app install https://github.com/YunoHost-Apps/misskey_ynh/tree/testing --debug
ou
sudo yunohost app upgrade misskey -u https://github.com/YunoHost-Apps/misskey_ynh/tree/testing --debug
```

**Plus d'infos sur le packaging d'applications :** https://yunohost.org/packaging_apps