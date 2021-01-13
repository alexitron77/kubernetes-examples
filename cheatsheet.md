# Cheatsheet

## Kubernetes

### Useful commands

> kubectl rollout history deploy \<deployment name\> \
Get the rollout version history of a deployment

- kubectl rollout undo deploy/\<name\> --to-revision=1 \
Rollback the current version of the deployment to revision 1. The previous replicaset is used to recreate the pods

- kubectl proxy -p 8080 \
Expose kube api json schemas on localhost:8080

- kubectl api-ressources \
List all the resources from k8s

- kubectl explain <resource> \
Documentation on the resource + required fields for this resource

- kubectl scale deployment/<name> --replicas=10 \
Scale the current deployment replica

- kubectl set image deploy/<name> <container name>=<new image> --record \
Set a updated image in the container. The record paramater log this command into the current revision to trace what have been done


