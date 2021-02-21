# trino-k8s

* Create namespace for Trino
```
$ kubectl create namespace trino
```

* Update config files in config directory

* Create trino resource
```
$ kubectl create configmap trino-configs --from-file=trino-configs/ -n trino
$ kubectl create -f trino-tmp-data-pv.yaml -n trino
$ kubectl create -f trino.yaml -n trino
```
