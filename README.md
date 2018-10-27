# docker-cron
- `sudo docker build -t nickel/cron .`

Build with ARGS
`docker build -t ais-to-s3 . --build-arg proj_dir=/ais --no-cache`

Shared with host 
- `docker run --name ais-to-s3 -v ~/ais/:/ais ais-to-s3`
Shared docker volume
- `docker run -it --name test2 -v data:/data nickel/cron bash`

Start container
`start ais-to-s3-1`

Export container:
`docker export <containername> | gzip > myapp.tgz`

`chmod 400 key.pem`
`scp -i "key.pem" aistos3.tgz ubuntu@35.178.87.3:~/ais`
`docker import myapp.tgz myapp`

https://stackoverflow.com/questions/46721871/how-to-ssh-into-amazon-lightsail-without-putty

## Resources
ENV vars
https://vsupalov.com/docker-env-vars/
