# Cluster Pod Status Controller

## Prerequisite

1. k8s Cluster



## Quick Installation Guide
 
 1. Apply
 ```
 bash ./deployment/apply.sh
 ```

 2. CleanUp or Destroy

 ```
 bash ./deployment/destroy.sh
 ```


## Installation Guide

1. Create Service account 
```
Kubectl apply -f ./deployment/service-account.yml
```
2. Create Cluster Role 
```
Kubectl apply -f ./deployment/cluster-role.yml
```
3. Create Cluster Role Binding 
```
Kubectl apply -f ./deployment/cluster-role-binding.yml
```
2. Apply Deployment 
```
Kubectl apply -f ./deployment/deployment.yml
```

## Run 
```
go mod tidy
go run main.go
```
## Build 
```
go build -o main .
./main
```