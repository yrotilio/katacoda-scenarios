Démo Kubernetes App

1. Deploy, check, expose, scale

`launch.sh`{{execute T1}}

`kubectl run front-web --image nginx:stable-alpine`{{execute T1}}

`kubectl get all`{{execute T1}}

`docker ps | grep front-web`{{execute T2}}

`kubectl delete pod`{{execute T1}}

`cat front-web.yaml`{{execute T1}}

`kubectl create -f front-web.yaml`{{execute T1}}

`kubectl get deployment,svc,rc,pod`{{execute T1}}

`curl host01:30080`{{execute T1}}

`kubectl scale deploy/front-web --replicas=2`{{execute T1}}

`kubectl get deployment,svc,rc,pod`{{execute T1}}

2. Update, rollback

cat votingapp.yaml

kubectl create -f votingapp.yaml

Check web srv

kubectl scale deploy/vote --replicas=2

sed votingapp.yaml

kubectl rolling-update deploy/vote -f votingapp-v2.yaml

Check web srv

kubectl apply -f votingapp.yaml

3. Mesh

Service to v1/v2/v3