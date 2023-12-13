# Kubernetes kubectl Commands Cheat Sheet

## List Pods

```bash
kubectl get pods
kubectl get pods -n namespace-name
```

## List Services

```bash
kubectl get services
```

## Describe a Pod

```bash
kubectl describe pod pod-name
kubectl describe pods -n namespace-name
```
## Check Logs

```bash
kubectl logs pod-name -n namespace-name
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
