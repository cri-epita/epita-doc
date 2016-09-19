# Netsoul

Netsoul is, among many thingss, an authentication protocol on the school's network. Netsoul is necessary to go on the internet from network-wired computers.

One has to identify with his login and SOCKS [password](password_anglais.md).

## Clients

Multiple client exist on different platforms :

. BnetSoul (Windows)
. jogsoul (Linux, Windows, etc...)
. QNetSoul (Linux)

And more...

## Diskless / rack - Arch Linux

Jogsoul is present with an additional wrapper to help enter identifiers.

This wrapper launches a graphic interface if login/password have never been inquired. Else, it starts jogsoul directly.

In case of error while typing identifiers, deleting _".jogsoul.conf"_ file (NOT jogsoul.conf !) will allow you to restart `jogsoul`.

## Racks - Windows

BnetSoul is already installed on windows. One simply has to enter login and password.
