# shamzaou-iot

GitOps source for Part 3 of Inception-of-Things. Argo CD deploys `manifests/` into the
`dev` namespace. To switch the app version, change the image tag and push:

```sh
sed -i 's/wil42\/playground:v1/wil42\/playground:v2/g' manifests/deployment.yaml
git commit -am "v2" && git push
```
