netchecker-server
=================

Basic network checker service to check DNS and connectivity in kubernetes
cluster. Should be used together with [netchecker-agent]
(https://github.com/adidenko/netchecker-agent).

Service listens on 8081 port (31081 nodePort) and accepts updates from agents.
You can use simple `curl` to get status (see below).

How to
------
* Build and push container:

```bash
cd ./docker && cat README.md
```

* Run netchecker server pod:

```bash
kubectl create -f netchecker-server_pod.yaml
```

* Run service:

```bash
kubectl create -f netchecker-server_svc.yaml
```

* Check status:

```bash
curl -s localhost:31081/api/v1/agents/
```
