# solita/ubuntu-systemd-ssh

[`solita/ubuntu-systemd`](https://hub.docker.com/r/solita/ubuntu-systemd/) + an SSH server.

## Supported tags

* `latest`, `16.04`

## Running

You need to add a couple of flags to the `docker run` command to make `systemd` play nice with Docker:

    docker run --stop-signal=SIGRTMIN+3 --tmpfs /run --tmpfs /run/lock -v /sys/fs/cgroup:/sys/fs/cgroup:ro YOUR_IMAGE

## License

Copyright © 2016 [Solita](http://www.solita.fi). Licensed under [the MIT license](LICENSE).
