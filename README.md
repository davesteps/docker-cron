# docker-cron
- `sudo docker build -t nickel/cron .`

Build with ARGS
`docker build -t ais-to-s3 . --build-arg proj_dir=/ais --no-cache`

Shared with host 
- `docker run --name ais-to-s3 -v ~/ais/:/ais ais-to-s3`
Shared docker volume
- `docker run -it --name test2 -v data:/data nickel/cron bash`

Start container
`docker start ais-to-s3-1`

`chmod 400 key.pem`
`sudo crontab -e`

# SWAP!
https://www.digitalocean.com/community/tutorials/how-to-add-swap-space-on-ubuntu-16-04
https://stackoverflow.com/questions/46721871/how-to-ssh-into-amazon-lightsail-without-putty

## Resources
ENV vars
https://vsupalov.com/docker-env-vars/
