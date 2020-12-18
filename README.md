# kub

from https://kubernetes.io/docs/tasks/administer-cluster/dns-debugging-resolution/

Take a look inside the resolv.conf file
kubectl exec -ti dnsutils -- cat /etc/resolv.conf

kubectl exec -i -t dnsutils -- nslookup kubernetes.default

kubectl exec -ti dnsutils -- ping pod
