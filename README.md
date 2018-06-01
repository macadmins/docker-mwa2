# MWA2 Docker Container

This container is currently only built for testing purposes.
See the [sal](https://github.com/salopensource/sal) and [sal-ldap](https://github.com/macadmins/sal-ldap) containers for how to rebuild this container to add gunicorn and ldap support.


# Usage

```
docker run -d --name="munkiwebadmin" \
  -p 80:8000 \
  -v /path/to/munki_repo:/munki_repo \
  -e ADMIN_PASS=password \
  macadmins/mwa2:latest
```


