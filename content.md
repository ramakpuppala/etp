### Emerging Technologies
-Presented on 22 May, 2018 to CGI team at Massachusetts Department of Unemployment Insurance <!-- .element: style="font-size:x-small;" -->


### What is an Emerging Technology ?
> Emerging technologies are technologies that are perceived as capable of changing the status quo  
> -- Wikipedia

### Why Change Status Quo?
* Cost 
* Efficiency 
* Survival 
* Competitive Advantage 
* Faster time to market 
* Agility 
* Scalability 

### Caveats
* Support
* Feature Complete
* Bugs
* Immature


### ETP - NEBU,CGI
- Cloud 
- Agile 
- DevOps 
- Security  
- BlockChain 
- Robotic Process Automation 



### DUA
- DevOps 
  - Docker 
  - Orchestration (Portainer) 
- Cloud 
 - Monitoring & Alerting (Prometheus, Grafana, Mattermost) 
 - Database driver upgrade (No Client or Tns files) 
- Agile 
 - TFS, Git & CICD 
 - Communication (mattermost) 
 


### Docker
- What is Docker?
  - Docker is an ecosystem of tools that help IT orgranizations to help package and run applications infrastructure agnostic.
  - Docker is a virtulization technology which relies on the host operating system capabilities
    to create as many sub systems (containers) only bounded by the physical resources on the host.
  - Docker runs natively on linux, mac and windows. Previously Mac and Windows ran with the help of Docker Toolbox which created a linux vm.

- How ?
  - Images
  - Containers
  - Registries

### Docker File
```
FROM microsoft/dotnet-framework:4.6.2
WORKDIR /app
COPY bin/Debug/ .
RUN sc create ListenerService binPath= "C:\\app\\uFACTS.BatchProcess.Listener.exe"
ENTRYPOINT sc start ListenerService \
&& PowerShell Get-Content C:\\uFACTS\\logs\\uFACTS.BatchProcess.Listener\\*.uLOG -Wait
```

### Images
 A Docker image is built up from a series of layers. Each layer represents an instruction in the image's Dockerfile.
 ![alt text](https://docs.docker.com/v17.09/engine/userguide/storagedriver/images/container-layers.jpg)(https://docs.docker.com/v17.09/engine/userguide/storagedriver/images) 


### Containers


### Registries



### Orchestration
- Compose
- Swarm
- Kubernetes
- Mesos DC/OS
- OpenShift
- ECS, EKS, AKS & Many more ...

### Kinds of Orchestration
- Single Node
- Cluster

### DUA
- Portainer
  - Single Node orchetrator


### Demo


### Thank You
### &
### Questions
