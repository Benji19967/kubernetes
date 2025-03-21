# Kubernetes

## Containers

### Images

- For containers
- Stored in a registry (Artifactory, GitLab)

## Workloads

### Pods

- Smallest deployable units of computing in Kubernetes
- Created using a Deployment (or Job or StatefulSet)
- Provide Networking and Storage for the container(s)
- Usually contains one container
- Can be evicted for lack of resources on a Node
- Restarts on crashes
- Can mount (persistent) Volumes
- Can have liveness and readiness probes

### Deployments

- Manages a set of pods to run a stateless application
- Choose a desired state
  - image to run for each pod
  - how many replicas to run
- Can rollback to a previous Deployment
- Can be autoscaled

### CronJobs

### HPA

## Storage

### secret

### persistent volumnes

### ephemeral storage

## Services

### Service

## Configs

### configMap

### Liveness and Readiness Probes

### Requests and Limits

cpu, memory
