# TestBlueGreenDeployment

建立node api
```sh
kubectl apply -f nodejs/node-deployment.yaml
kubectl apply -f nodejs/node-service.yaml
```

建立nginx
```sh
kubectl apply -f nginx/nginx-deployment.yaml
kubectl apply -f nginx/nginx-service.yaml
```

使用瀏覽器打開頁面
```sh
http://localhost:32000
```

可以用下面指令更新api的版本觀察pod更新的狀態
```sh
kubectl apply -f node-deployment-1.0.1.yaml
```
