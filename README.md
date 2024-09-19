
## Install
```
git clone https://github.com/enghwa/eks-dify-chart
cd eks-dify-chart/charts/dify

# no need to run this, the dep. are in this git.
# helm dependency build

helm install dify .
```

Get public NLB endpoint:
```
kubectl get --namespace default svc -w dify
```
then:
```
http://<xxxxxxx.xxxx.ap-xxx-1.elb.amazonaws.com>/install

```

You will see a page that says "Setting up an admin account", setup an admin acct using any email address and username/password.
Next, you can login to dify!

## Uninstall

```
helm uninstall  dify
```
manually delete all the PVC.
