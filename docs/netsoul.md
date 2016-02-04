# Netsoul

Netsoul est, entre autre, un protocole d'authentification sur le réseau de l'école. Il est nécessaire pour aller sur internet depuis le réseau câblé (pas nécessaire sur Ionis Portal).

Il faut s'authentifier avec votre login et votre pass SOCKS (voir la rubrique [Mots de passe](passwords.md))

## Clients

Il existe de nombreux clients netsoul disponibles sur différentes plateformes :

 * BnetSoul (Windows)
 * jogsoul (Linux, Windows, etc.)
 * QNetSoul (Linux)
 * etc.

## Diskless / Rack - Archlinux

Jogsoul est présent  avec un wrapper supplémentaire afin d'aider à entrer les identifiants.

Ce wrapper lance une fenêtre graphique si le login/password n'ont jamais été renseignés. Sinon il lance directement jogsoul.

En cas d'erreur lors de la saisie des identifiants, il faut supprimer le fichier _".jogsoul.conf"_  (et non jogsoul.conf) puis relancer `jogsoul`.

## Racks - Windows

BnetSoul est déjà installé sur le windows présent sur les racks. Il suffit d'y entrer son login/password.
