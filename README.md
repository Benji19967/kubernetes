# Kubernetes

## Containers

### Images

- For containers
- Stored in a registry (Artifactory, GitLab)

## Workloads

### Pods

- Usually contains one container
- Restarts on crashes

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
