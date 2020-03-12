A Docker compose and K8s config for deploying CD4PE with containerized postgres.

Start with
```
docker stack deploy cd4pe --orchestrator kubernetes -c docker-compose.yml
```
or
```
kubectl apply -f manifests/postgres.yaml -f manifests/cd4pe.yaml
```

> Note that manifests have been templated for deployment with kots.io and will need to have template substitution done before they can be applied.
