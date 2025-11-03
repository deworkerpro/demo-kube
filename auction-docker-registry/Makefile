deploy:
	kubectl -n auction \
		create secret docker-registry docker-registry \
		--save-config \
		--dry-run=client \
		--docker-server="${REGISTRY}" \
		--docker-username="${USERNAME}" \
		--docker-password="${PASSWORD}" \
		-o yaml | kubectl apply -f -
