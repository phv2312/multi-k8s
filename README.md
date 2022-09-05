# Updates
1. Change dependency in *./server/package.json*, **pg** to **8.7.1**
2. Mount storage for server deployment to get log.
3. Specify version for image instead of using the latest one.

# Start Docker

```bash
docker-compose -f docker-compose.yml up --build --remove-orphans
```

Then, access the UI via

```
http://localhost:3050/
```

# Start k8s

```bash
kubectl apply -f k8s/
```

Then, access the UI via:

```
http://<your_minikube_ip>
```

