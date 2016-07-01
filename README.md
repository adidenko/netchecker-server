netchecker-agent
================

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
