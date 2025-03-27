# Kubernetes

## Nodes

- Virtual or physical machine
- Typically, several nodes make up a cluster

## Containers

### Images

- For containers
- Stored in a registry (Artifactory, GitLab)

## Workloads

### Pods (Example: instance of a Feature Generator or a Server, ...)

- Smallest deployable units of computing in Kubernetes
- Created using a Deployment (or Job or StatefulSet)
- Provide Networking and Storage for the container(s)
- Usually contains one container
- Can be evicted for lack of resources on a Node
- Restarts on crashes
- Can mount (persistent) Volumes
- Can have liveness and readiness probes

### Deployments (Example: Server, FG, Ingestion Service, ...)

- Manages a set of pods to run a stateless application
- Choose a desired state
  - image to run for each pod
  - how many replicas to run
- Can rollback to a previous Deployment
- Can be autoscaled

### CronJobs (Example: Hourly Consolidation Service)

### HPA (Example: Ingestion Service, FGs)

## Storage

### secret (Example: GCP key)

### persistent volumnes (Example: FG models)

### ephemeral storage

## Services

### Service (Example: Server)

- Helps you expose groups of Pods over a Network

- Pods have their own IP 
- Pods run and die, how does a frontend know which IP to hit? --> Come in Services
- Usually cluster internal (use Ingress to expose to the outside world)

## Configs

### configMap (Example: number of threads to use, any application configs)

- Do not need to redeploy Deployment, only update configMap and restart Deployment

### Liveness and Readiness Probes (Example: Server http check)

### Requests and Limits (Example: FGs, Ingestion, Server, ...)

cpu, memory
