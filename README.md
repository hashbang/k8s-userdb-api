# k8s-postgrest

## Usage

Add your own configuration (`base` by default looks for `config.txt`; though you can override with your own [kustomization](https://kubectl.docs.kubernetes.io/pages/app_customization/bases_and_variants.html)).

Apply with:

```
kubectl apply -k base
```

This repository assumes that an ingress controller is installed. A quick and dirty way to get one would be to `kubectl apply`:

  - https://raw.githubusercontent.com/kubernetes/ingress-nginx/nginx-0.26.1/deploy/static/mandatory.yaml
  - https://raw.githubusercontent.com/kubernetes/ingress-nginx/nginx-0.26.1/deploy/static/provider/cloud-generic.yaml

This repository assumes that a cert manager is installed. A quick and diry way to get one would be to `kubectl apply`:

  - https://github.com/jetstack/cert-manager/releases/download/v0.12.0/cert-manager.yaml
