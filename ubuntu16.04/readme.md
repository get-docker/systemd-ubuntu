# Ubuntu image with systemd enabled

You can use this image as a base container to run systemd services inside.

## Supported tags

* `latest`, `16.04`

## Usage

Run the container as a daemon

```shell
docker run -d \
--privileged \
--name systemd-ubuntu \
-v /sys/fs/cgroup:/sys/fs/cgroup:ro \
cnphpbb/systemd-ubuntu:16.04
```

Enter to the container

```shell
docker exec -it systemd-ubuntu bash
```
