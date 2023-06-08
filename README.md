# Deployment Scripts

This repository contains scripts for aiding in the deployment of [log-store](https://log-store.com). See the [docs](https://log-store.com/documentation.html?page=install) for more info.


## Kubernetes

#### License
Create a file named license.txt that has the license string inside
```
configMapGenerator:
- name: log-store-license
  files:
  - license.txt
  options:
    disableNameSuffixHash: true
```

#### Deployment
```
kubectl apply -k .
```
