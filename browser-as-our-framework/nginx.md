```bash
server {
    listen       80;
    server_name  localhost;
    root         /srv/www/;
    index        index.html;

    location / {
        try_files $uri $uri/index.html /2017/index.html;
    }
}
```
