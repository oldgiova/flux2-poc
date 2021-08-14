# Flux2 PoC
PoC and experiments on Flux2

# Setup
```
flux bootstrap github --owner=rgiovanardi --repository=flux2-poc --branch=main --path=./clusters/my-cluster --personal
```

# Add podinfo repo to Flux
```
flux create source git podinfo \
  --url=https://github.com/rgiovanardi/flux2-poc \
  --branch=main \
  --interval=30s \
  --export > ./clusters/my-cluster/podinfo-source.yaml
```
