deploy:
	kubectl apply -f kube/secret.yaml
	kubectl apply -f kube/service-account.yaml
	kubectl apply -f kube/cluster-role-binding.yaml

show-token:
	@echo
	@kubectl get secret/deploy -o go-template --template '{{index .data "token"}}' | base64 -d
	@echo
