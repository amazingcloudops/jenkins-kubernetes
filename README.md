# jenkins-kubernetes
Running Jenkins on a kubernetes cluster with the yaml files.
Jeknis is derived from Jenkins LTS official image, and docker, maven installed already.

Below modifications are required -

1. Update the pv_jeknins.yaml file to the IP of the NAS where NFS volume is used.
2. Update deployment_jenkins.yaml image file pointing to the path of your private docker registry where the jenkins image is hosted.
3. Update ingress_jenkins.yaml to point to correct hostname and the certificate secret file in your environment.

