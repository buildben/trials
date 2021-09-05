# Requirements

 Helm 3+

# Installation

## Dependencies download

1. helm repo add bitnami https://charts.bitnami.com/bitnami

2. helm dep up

## Buildben installation

1. helm upgrade --install -n buildben-helm-test buildben -f values.yaml . \
    --set values.imageCredentials.registry=docker.pkg.github.com \
    --set values.imageCredentials.username=mehdzor \
    --set values.imageCredentials.password=3820f23038657582d2edefcca3af5369f0968595
