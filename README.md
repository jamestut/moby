# Modified Dockerd

This is a forked version of dockerd with the following modifications:

- Allow dropping capabilities (`cap-drop`) on privileged containers.
- Reloads `config.v2.json` and `hostconfig.json` from a container every time that container is started, without having to restart the entire dockerd.