## kubectl ssh

ssh into a pod's node

[![asciicast](https://asciinema.org/a/lNy3cRCPFGwDM26UBQYmfNKYT.svg)](https://asciinema.org/a/lNy3cRCPFGwDM26UBQYmfNKYT)


### Installing


** Important: kubectl 1.15 or greater is required **


```
curl -fsS -o /usr/local/bin/kubectl-ssh \
    https://raw.githubusercontent.com/IuryAlves/kubectl-ssh/master/kubectl-ssh && \
        chmod +x /usr/local/bin/kubectl-ssh
```

**make sure that `/usr/local/bin` is in your path.**
