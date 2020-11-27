1. 
```
cd ./images
docker build -t jervis/tomcat-app:v1 .
```

1. 
```
kubectl create -f mysql-rc.yaml
```

2. 
```
kubectl create -f mysql-svc.yaml
```

3. 
```
kubectl create -f myweb-rc.yaml
```

4. 
```
kubectl create -f myweb-svc.yaml
```

5. 
```
docker ps | grep my
```

6. 
```
kubectl get services
```

7. 
```
http://172.28.124.194:30001/demo/
```