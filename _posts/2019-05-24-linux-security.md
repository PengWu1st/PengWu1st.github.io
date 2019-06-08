---
layout: "post"
title: "linux security"
date: 2019-05-24 23:04:00 -0700
---

## to check firewall status
```
sudo ufw status
```
## to block everthing incoming
```
sudo ufw default deny incoming
```
## to allow everthing outgoing

```
sudo ufw default allow outgoing
```

## allow ssh
```
sudo ufw allow ssh
```

## allow tcp on port 2222

```
sudo ufw allow 2222/tcp
```

## allow basic http server
```
sudo ufw allow www
```

## enable firewall

make sure you have allow ssh before you run this!!!
```
sudo ufw enable
```