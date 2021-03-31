# oaktreeapp

Sample Web Frontend and Backend application for Oaktree

## Deployment

### Create Namespaces
```
kubectl create ns product-store
kubectl create ns product-api
```

### Deploy Application
```
cd oaktreeapp
kubectl apply -f product-api/
kubectl apply -f product-store/
