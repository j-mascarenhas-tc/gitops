# https://github.com/sedflix/multi-cluster-istio-kind
The following dependencies must be installed before running the script:

kubectl
kind
docker
Usage:

   ./setupkind.sh --cluster-name cluster1 --k8s-release 1.21.1 --ip-octet 255

Where:
   -n|--cluster-name - name of the k8s cluster to be created, cluster1 will be used if not given
   -r|--k8s-release  - the release of the k8s to setup, latest available if not given
   -s|--ip-octet     - the 3rd octet for public ip addresses, 255 if not given, valid range: 100-255
   -h|--help         - print the usage of this script