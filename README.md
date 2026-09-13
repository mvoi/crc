# CRC

## Installation
Download Archive from RedHat

    tar xvzf crc-linux-amd64.tar.xz
    cd crc-linux-2.63.0-amd64
    ./crc setup
    sudo apt-get install virtiofsd
    crc start

## Commands
    crc oc-env
    crc start
    crc console --credentials
    
## Tools
PATH="$HOME/.crc/bin/oc:$PATH"

## ArgoCD Helm Installation

    oc create namespace argocd
    helm install argocd argo/argo-cd -namespace argocd --values values-crc.yaml --timeout 10m
