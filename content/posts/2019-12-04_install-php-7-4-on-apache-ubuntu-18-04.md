---
title: "Install PHP 7.4 on Apache Ubuntu 18.04"
date: 2019-12-04T10:59:14+02:00
tags: ["php", "apache"]
---

### Add PPA for PHP 7.4

Add the **ondrej/php** which has PHP 7.4 package and other required PHP extensions.

```bash
sudo apt install software-properties-common
sudo add-apt-repository ppa:ondrej/php
sudo apt update
```

Once you have added the PPA you can install PHP 7.4.

```bash
sudo apt install php7.4
```

### Verify PHP 7.4 is installed

```bash
php -v
```

### Install PHP 7.4 Extensions

Installing PHP extensions are simple with the following syntax.

```bash
sudo apt install php7.4-**extension_name**
```

Some common php extensions install command

```bash
sudo apt install php7.4-common php7.4-mysql php7.4-xml php7.4-xmlrpc php7.4-curl php7.4-gd php7.4-imagick php7.4-cli php7.4-dev php7.4-imap php7.4-mbstring php7.4-opcache php7.4-soap php7.4-zip php7.4-intl -y
```

### Configure PHP 7.4 Apache

```bash
sudo nano /etc/php/7.4/apache2/php.ini
```
