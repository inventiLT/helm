# Helm Repo

### How To publish charts

```console
$ helm package charts/mychart -d docs/
$ helm repo index docs --url https://inventilt.github.io/helm
$ git add -i
$ git commit -av
$ git push origin master
```

From there, you can do a `helm repo add tscharts https://inventilt.github.io/helm`
