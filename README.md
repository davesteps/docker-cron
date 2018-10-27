# docker-cron
- `sudo docker build -t nickel/cron .`
Shared with host 
- `docker run --name test2 -v ~/gitClones/docker-cron/data/:/ais nickel/cron`
Shared docker volume
- `docker run -it --name test2 -v data:/data nickel/cron bash`

Build with ARGS
`docker build -t nickel/cron . --build-arg proj_dir=/ais`

Start container
`docker start test4`


## Resources
ENV vars
https://vsupalov.com/docker-env-vars/
