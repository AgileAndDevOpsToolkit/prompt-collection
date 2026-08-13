Pour créer et héberger une image Docker dans GHCR :

```
crée un Dockerfile et le workflow Github Action afin de mettre l'image dans GHCR
```

Les commandes pour tester l'image une fois qu'elle est créée et déposée dans GHCR par le workflow GitHub Action :

```
docker pull ghcr.io/agileanddevopstoolkit/categorix:6824550

docker run -d --name categorix -p 8083:80 ghcr.io/agileanddevopstoolkit/categorix:6824550
```