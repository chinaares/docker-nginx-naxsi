# Supported tags and respective `Dockerfile` links

-   [`1.13.0`, `1.13`, `mainline`, `latest` (*mainline/Dockerfile*)](https://github.com/dmgnx/docker-nginx-naxsi/blob/master/mainline/Dockerfile)
-   [`1.12.0`, `1.12`, `stable` (*stable/Dockerfile*)](https://github.com/dmgnx/docker-nginx-naxsi/blob/master/stable/Dockerfile)

# How to use this image

```console
$ docker run --name nginx-naxsi -p 80:80 \
    -v $(pwd):/usr/share/nginx/html -d dmgnx/nginx-naxsi
```

This will start a nginx service with default configuration, serving current working directory as you website.

# Volumes

-   /etc/nginx/conf.d : virtual hosts configuration
-   /etc/nginx/naxsi : your Naxsi rules
-   /etc/nginx/ssl : SSL certificates
-   /usr/share/nginx/html : web root directory
-   /var/log/nginx : log storage (default redirecting it to standard outputs)

