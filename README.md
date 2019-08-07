# kubernetes-ingress-info-helm

Helm chart for [kubernetes-ingress-info](https://github.com/bitsofinfo/kubernetes-ingress-info)

## Usage

Example using Traefik for the ingress controller

    helm install \
    --name kubernetes-ingress-info \
    --namespace my-namespace \
    . \
    --set rbac.create=true \
    --set loadConfigMode=cluster \
    --set databaseCache.enabled=true \
    --set ingress.enabled=true \
    --set ingress.labels."labelName"=value \
    --set ingress.annotations."ingress\.kubernetes\.io/protocol"=http \
    --set ingress.annotations."kubernetes\.io/ingress\.class"=traefik \
    --set ingress.annotations."anotherAnnotation"=value

## TODO: description of values
