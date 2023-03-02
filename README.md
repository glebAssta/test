# This playbook was written to install nginx, haproxy, keepalived on server #

## What tasks are used: ##

### Install nginx ###

1. install nginx
2. start nginx
3. download index.HTML
 > to download html file on server
4. download templates
 > to download nginx templates on servers
5. update default conf
 > to download nginx.conf on servers
6. handlers to reload nginx
```
  - name: Reload nginx
    service:
      name: nginx
      state: reloaded
```

### Install Ha-proxy ###
1. Configure Load balancer
2. download haproxy.cfg
3. and handler reload haproxy

### Install keepalived ###
1. Configure Load balancer
2. download haproxy.cfg
3. and handler reload haproxy
