# Helm Repo

### How To publish charts

```console
$ helm package charts/mychart -d docs/
$ helm repo index docs --url https://inventi.github.io/helm
$ git add docs/
$ git commit -av
$ git push origin master
```

From there, you can do a `helm repo add inventi https://inventi.github.io/helm`
