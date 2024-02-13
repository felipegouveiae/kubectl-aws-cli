<!-- ABOUT THE PROJECT -->
# About The Project

This is a simple image that contains the latest kubernetes cli installed and aws-cli v2 installed over a Ubuntu 22.04.
I found this awesome <a href="https://linuxhandbook.com/auto-update-aws-ecr-token-kubernetes/" target=blank>article</a> about a cron job to renewal AWS ECR tokens and after running on my local environment (Macbook Pro M1 over Microk8s + Multipass) I was getting an error related to invalid platform.

The original one can be found <a href="https://hub.docker.com/r/omarxs/awskctl" target="blank">here</a>: omarxs/awskctl:v1.0

AWS CLI installs according to the platform (amd64/arm64) so I decided to create this repo in order to share the code and also provide a open-source docker image to run this cron on Kubernetes.

The image can be downloaded here: https://hub.docker.com/repository/docker/felipegouveiae/kubectl-aws-cli/general

## Build instructions

`
$ sh build.sh
`