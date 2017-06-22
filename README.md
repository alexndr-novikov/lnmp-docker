# lnmp-docker
Simple Nginx+PHP+MySQL+PostgreSQL docker template

Install docker-ce and docker-compose if haven't done it yet (use the latest version from the official repos)

PHP application should be located in www/* folders.

Nginx configs are located in /hosts folder.  Copy demo.dev config and change it to create new sites.
 

Execute the following to startup the application
```
docker-compose up -d
```


Execute the following to stop the application
```
docker-compose down
```

Execute the following to stop the application, deleting created data
```
docker-compose down --volumes
```


Add lnmp.local to hosts file being linked to docker local ip.
Visit http://demo.dev in browser , after you added in hosts

```
127.0.0.1   demo.dev
```
