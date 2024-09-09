

```
git clone https://github.com/enghwa/eks-dify-chart
cd eks-dify-chart/charts/dify
helm dependency build
helm install dify .
```

do the port forwarding:
then:
```
http://localhost:8080/install

```