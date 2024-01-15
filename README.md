# FreeBSD Lighttpd OpenSSL
In this reopsitori, you will learn how to install and configure Lighttpd on a FreeBSD server. Not only that, to improve the security of the Lighttp web server, we have also added Openssl mode to the contents of this article.

## System specifications

OS: FreeBSD 13.2 Stable

Hostname: ns5

IP Address: 192.168.5.2

Domain: datainchi.com

Lighttpd version: lighttpd/1.4.67 (ssl) - a light and fast webserver

### Installation
As you know, on the FreeBSD server there are two ways to install each application, namely the port system and the PKG package. Especially for the Lighttp installation, we prefer to use the port system, because it can build all the libraries that Lighttpd needs.

Before we start the process of installing Lighttpd, you first install the Lighttpd dependencies, namely "Build dependencies" and "Library dependencies". Here's how to install these dependencies.
``` bash
root@ns5:~ # pkg install cmake-core ninja pkgconf
root@ns5:~ # pkg install pcre2 nettle lua54
root@ns5:~ # cd /usr/ports/www/lighttpd
root@ns5:/usr/ports/www/lighttpd # make config
root@ns5:/usr/ports/www/lighttpd # make install clean
```

## Support
https://www.unixwinbsd.site/2024/01/freebsd-lighttpd-installation-and.html
