# docker-haveged

Docker image for [haveged](http://www.issihosts.com/haveged/), an entropy daemon for Linux. It uses CPU flutter
to provide additional entropy for the `/dev/random` and `/dev/urandom` devices.

When the container is run with `--privileged`, it provides entropy for the host's random devices, which is then
available to other containers.