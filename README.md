# ansible install k3s on ubuntu

this ansible playbook will install docker and k3s on the ubuntu, and make k3s use docker container.

## step1: install docker&k3s
```
ansible-playbook collectioin.yml --extra-vars "k3s_version=v0.10.0"
```

## step2: check k3s is running
```
$ sudo k3s kubectl get no
NAME       STATUS   ROLES    AGE   VERSION
k3s   Ready    master   47h   v1.15.4-k3s.1
```