deploy:
	kubectl apply -f kube/sysctl.yaml

show:
	kubectl run busybox --image=busybox:latest --rm=true -it --privileged=true -- sysctl -a
