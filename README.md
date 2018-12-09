### reverse ssh tunnel on docker alpine

env vars:

```
REMOTE_IP: same as gatewayports on ssh
REMOTE_PORT: port to bind to on remote server
LAN_IP: lan ip to tunnel
LAN_PORT: lan port to tunnel
SSH_USER: user to ssh with
SSH_HOST: ip/fqdn of ssh server
SSH_EXTRA_ARGS: extra args for ssh client, -oExitOnForwardFailure=yes, -v, etc.
```

volume mount for ssh key auth:

```
  -v '~/.ssh:/root/.ssh:ro'
```
