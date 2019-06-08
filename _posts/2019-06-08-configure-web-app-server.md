---
layout: "post"
title: "configure web application server"
date: 2019-06-08 21:07:00 -0700
---

## install apache2
```
sudo apt-get install apache2
```

## install mod_wsgi
```
sudo apt-get install libapache2-mod-wsgi
```

## configure Apache to handle requests using the WSGI module

edit the file `/etc/apache2/sites-enabled/000-default.conf`

add the following line at the end of the `<VirtualHost *:80>` block, right before the closing `</VirtualHost>` line: `WSGIScriptAlias / /var/www/html/myapp.wsgi`

## restart Apache 

```
sudo apache2ctl restart
```

## create the first wsgi application

```
sudo nano /var/www/html/myapp.wsgi
```