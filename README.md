# lnmp-docker
Simple Nginx+PHP+MySQL docker template

Nginx config located in site.conf.tpl. Copy it to site.conf in the root of the repo to be used by containers.
Change something if needed.

Install docker-ce and docker-compose if haven't done it yet (use the latest version from the official repos)

PHP application should be located in application/ folder. By default, server root is application/ root, change it in site.conf if needed.

Execute the following to startup the application
```
docker-compose up
```

Add lnmp.local to hosts file being linked to docker local ip.
Visit http://lnmp.local in browser.
