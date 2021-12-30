# docker-ubuntu-systemd
## Description
Ubuntu with systemd in a Docker container - behaves (mostly) like a VM

## Example `docker-compose.yml`

```yaml
version: '3'
services:
  app:
    image: ghcr.io/sphr2k/ubuntu-systemd
    hostname: ubuntu
    volumes:
      - /sys/fs/cgroup:/sys/fs/cgroup:ro
    privileged: true
```
