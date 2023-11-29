# Kubernetes kubectl Commands Cheat Sheet

## List Pods

```bash
kubectl get pods
```

## List Services

```bash
kubectl get services
```

## Describe a Pod

```bash
kubectl describe pod pod-name
```

## Describe a Service

```bash
kubectl describe service service-name
```

## Execute a Command in a Running Pod

```bash
kubectl exec -it pod-name -- command
```

## Delete a Resource

```bash
kubectl delete resource resource-name
```

## Get Cluster Info
```bash
kubectl cluster-info
```
