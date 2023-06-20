build/setup_packer_configs.sh 1-26 raw ubuntu s3://projectbuildpipeline-857-pipelineoutputartifactsb-10ajmk30khe3f /home/image-builder/eks-anywhere-build-tooling/projects/kubernetes-sigs/image-builder/_output/tar/1-26/raw/ubuntu 1-26 latest image-builder/images/capi
PACKER_FLAGS="-force"
PACKER_LOG=1
PACKER_LOG_PATH=/home/image-builder/eks-anywhere-build-tooling/projects/kubernetes-sigs/image-builder/_output/tar/1-26/raw/ubuntu/packer.log
PACKER_VAR_FILES="/home/image-builder/eks-anywhere-build-tooling/projects/kubernetes-sigs/image-builder/_output/1-26/raw/ubuntu/config/kubernetes.json /home/image-builder/eks-anywhere-build-tooling/projects/kubernetes-sigs/image-builder/_output/1-26/raw/ubuntu/config/common.json /home/image-builder/eks-anywhere-build-tooling/projects/kubernetes-sigs/image-builder/_output/1-26/raw/ubuntu/config/cni.json /home/image-builder/eks-anywhere-build-tooling/projects/kubernetes-sigs/image-builder/_output/1-26/raw/ubuntu/config/additional_components.json"
make -C image-builder/images/capi build-raw-ubuntu-2204-efi
