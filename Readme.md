# Kubernetes Notes

This is repo is to save all notes and commonly commands about kubernetes.

## Notes

### ReplicaSet vs Deployment

The function of replicaset is manage all pods with the X Label that you configure. Check if all is fine, start or stop some containers to have the exactly replicas. 

About Deployment is a point of view more high which also review is the version of the image in the containers are correct.

> For this we always tries to create a Deployment which automatically will create a replicaset inside. 

## Commands

This command will execute a temporally command into a pod inside the k8s cluster:
```
kubectl run --rm -it --tty <deployment_name> --image=<image_name> <command>
```
