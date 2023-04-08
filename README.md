# api-version-test

```
> kubectl apply -f https://github.com/cert-manager/cert-manager/releases/download/v1.4.0/cert-manager.yaml

> k get --raw=/apis/cert-manager.io | jq
{
  "kind": "APIGroup",
  "apiVersion": "v1",
  "name": "cert-manager.io",
  "versions": [
    {
      "groupVersion": "cert-manager.io/v1",
      "version": "v1"
    },
    {
      "groupVersion": "cert-manager.io/v1beta1",
      "version": "v1beta1"
    },
    {
      "groupVersion": "cert-manager.io/v1alpha3",
      "version": "v1alpha3"
    },
    {
      "groupVersion": "cert-manager.io/v1alpha2",
      "version": "v1alpha2"
    }
  ],
  "preferredVersion": {
    "groupVersion": "cert-manager.io/v1",
    "version": "v1"
  }
}
```