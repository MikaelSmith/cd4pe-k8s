A Docker compose and K8s config for deploying CD4PE with containerized postgres.

Start with
```
docker stack deploy cd4pe --orchestrator kubernetes -c docker-compose.yml
```
or
```
kubectl apply -f postgres.yaml -f cd4pe.yaml
```

TODO: remove hard-coded `PFI_SECRET_KEY`.
