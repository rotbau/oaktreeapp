# oaktreeapp

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
