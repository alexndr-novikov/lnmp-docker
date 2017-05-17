server
{
    listen   80;
    server_name lnmp.local;

    root /var/www/html/site;
    index index.php;

    location /
    {
        try_files $uri $uri/ /index.php =404;
    }

    location ~ \.php$ {
        fastcgi_pass   test-php:9000;
        fastcgi_index  index.php;
        fastcgi_param  SCRIPT_FILENAME  $document_root$fastcgi_script_name;
        include        fastcgi_params;
    }
}