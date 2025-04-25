# Nginx Container Run Port 9000

* Container Name: my-nginx-9000
* run background
* show background log
* stop
* delete

```shell
# option delete publish name
docker run --rm -d -p 9000:80 --name my-nginx-9000 nginx:1.27.4
# stop
docker stop my-nginx-9000
```