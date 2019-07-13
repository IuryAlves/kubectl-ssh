## kubectl ssh

ssh into a pod's node

[![asciicast](https://asciinema.org/a/lNy3cRCPFGwDM26UBQYmfNKYT.svg)](https://asciinema.org/a/lNy3cRCPFGwDM26UBQYmfNKYT)


### Installing


**Important: kubectl 1.15 or greater is required**


```
curl -fsS -o /usr/local/bin/kubectl-ssh \
    https://raw.githubusercontent.com/IuryAlves/kubectl-ssh/master/kubectl-ssh && \
        chmod +x /usr/local/bin/kubectl-ssh
```

**make sure that `/usr/local/bin` is in your path.**


### Usage


* Basic usage:

```
kubectl ssh <pod_name>
```

* Ssh into node using specific ssh-user

```
kubectl ssh <pod_name> --user=root

```

This is equivalent to `ssh root@<ip>`


* Ssh into node using specific ssh-key

```
kubectl ssh <pod_name> -i /path/to/my/indetity-file
```

This is equivalent to: `ssh <ip> -i /path/to/my/indetity-file`


