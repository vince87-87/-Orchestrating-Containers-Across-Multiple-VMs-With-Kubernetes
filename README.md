# Orchestrating-Containers-Across-Multiple-VMs-With-Kubernetes

# INSTALL CLIENT TOOLS

- awscli
- kubectl
- cfssl
- cfssljson

# Configure aws CLI

aws configure sso

<img width="841" alt="image" src="https://user-images.githubusercontent.com/49937302/183536918-d19063fe-a05b-49a3-891b-7c607a3633e5.png">

# Install kubectl

curl -o kubectl https://storage.googleapis.com/kubernetes-release/release/v1.21.0/bin/darwin/amd64/kubectl

chmod +x kubectl

sudo mv kubectl /usr/local/bin/

# Install CFSSL and CFSSLJSON

cfssl is an open source tool by Cloudflare used to setup a Public Key Infrastructure (PKI Infrastructure) for generating, signing and bundling TLS certificates. cfssl will be configured as a Certificate Authority which will issue the certificates required to spin up a Kubernetes cluster.

# MAC

curl -o cfssl https://storage.googleapis.com/kubernetes-the-hard-way/cfssl/1.4.1/darwin/cfssl

curl -o cfssljson https://storage.googleapis.com/kubernetes-the-hard-way/cfssl/1.4.1/darwin/cfssljson

chmod +x cfssl cfssljson

sudo mv cfssl cfssljson /usr/local/bin/

<img width="934" alt="image" src="https://user-images.githubusercontent.com/49937302/183536152-1822906c-f559-4379-9411-1a4829dd54bd.png">

cfssl version

cfssljson --version

<img width="571" alt="image" src="https://user-images.githubusercontent.com/49937302/183536770-50b1e9bc-780f-4230-bf93-5c53102062c0.png">

cfssljson --version
