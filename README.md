# Oaktree Test Application

Sample Web Frontend and Backend application for Oaktree

## Deployment

### Pull Github Repo
```
git clone https://github.com/rotbau/oaktreeapp.git
```
or Click on Code button and select download Zip

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

### Locate Service
```
kubectl -n product-store get svc
```

Look for the EXTERNAL-IP for the product-store service.  If EXTERNAL-IP is pending you may need to add a load balancer

NAME            TYPE           CLUSTER-IP      EXTERNAL-IP    PORT(S)        AGE
product-store   LoadBalancer   100.69.66.117   172.31.3.190   80:30373/TCP   13s
