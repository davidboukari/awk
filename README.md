# awk

## Print line 2 and field 2
```
k get ingress -A
NAMESPACE       NAME                           CLASS   HOSTS                         ADDRESS          PORTS     AGE
myappdemo-tst   myappdemo-tst-myappdemo-helm   nginx   myappdemo-tst.myhawksys.com   xxxx   80, 443   36m

k get ingress -A|awk 'NR==2 {print $2}'
myappdemo-tst-myappdemo-helm

```
