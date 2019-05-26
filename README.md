# nginx
nginx notes

NGINX web server can be used for a handful of operations in addition to serving just as a static web server.

Nginx has one main config file by name nginx.config at /etc/nginx/(for redhat distro). This file needs to be configured for any of the usages mentioned below. There is one additional optional config directory/file at /etc/nginx/conf.d/ where config files for multiple applications can be placed if you want nginx to serve multiple sites.

Note: All the config files that I have shown here use just the main config file, nginx.config. you can also use combination of both nginx.config file and additional config file(creating dedicated files for every application) by representing just the server block in additional config file.

1) As Reverse Proxy:
Re-directing incoming requests on default nginx port 80 to other application servers' port and sending back the response appropriately.

2) https connection:
Serving traffic on https port 443 with SSL certificates

3) Load balancing:
Default load balancing scheme is Round Robin.

4) Serve multiple applications with just one domain.
