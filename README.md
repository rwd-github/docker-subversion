DEPRECATED moved to: https://gitlab.com/ytdocker/collection

docker-compose.yml

```
version: '2.2'
services:
 svn:
  image: rwd1/subversion
  container_name: svn
  ports:
    - "80"
  volumes:
    - /path/volumes/httpconfig:/etc/apache2/conf.d/httpconfig
    - /path/volumes/htpasswd:/etc/apache2/myhtpasswd
  restart: unless-stopped
```
