### Docker-nginx-reverse-proxy

Two sample web services inside Docker containers and a Nginx reverse proxy for those services.

Corrected example from [phoenixnap tutorial](https://phoenixnap.com/kb/docker-nginx-reverse-proxy) including SSL certs.


Build and run the sample web services from ```example1``` and ```example2``` directories.

```
docker-compose build
```

```
docker-compose up -d
```

Run the Nginx proxy from the ```proxy``` directory.

```
docker-compose build
```

```
docker-compose up -d
```


Make sure to add your host IP in ```/etc/hosts``` file:

```
192.168.2.11 example1.test
192.168.2.11 example2.test
```

Test the web services using
```
curl example1.test
```
```
curl example2.test
```