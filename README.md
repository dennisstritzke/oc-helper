# OpenShift Reference by Example
This repository is a collection of OpenShift deployments that are common in day to day usage.
Oftentimes you need some kind of deployment, but are not sure what the exact syntax is, this repository is here to help.
It aims to be the place to go, if you quickly want to look up the usage of an OpenShift resource by examples.

Just use `oc new-project` and create the deployments below.

## Basic Deployments
- [Ubuntu Logger](ubuntu-logger.yaml)
  is printing 'Hello OpenShift!' every second to standard out.
  ```
  oc create -f https://raw.githubusercontent.com/dennisstritzke/oc-helper/master/ubuntu-logger.yaml
  ```
- [Ubuntu PVC](ubuntu-pvc.yaml) is writing continously writing files containing the current time to `/ubuntu-pvc`
  ```
  oc create -f https://raw.githubusercontent.com/dennisstritzke/oc-helper/master/ubuntu-pvc.yaml
  ```
- [Nginx with Service and Route](nginx.yaml) provides a basic deployment accessible via the network.
  ```
  oc create -f https://raw.githubusercontent.com/dennisstritzke/oc-helper/master/nginx.yaml
  ```
- Privileged Pod. Yet to come...
- DaemonSet. Yet to come...
- ScheduledJob. Yet to come...

## Utilities
- curl, telnet and dig Pod. Yet to come...

## Advanced Deployments
- Client Certificate authentication reverse proxy. Yet to come...