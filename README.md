# Image Build


Rocky Linux 


https://user-images.githubusercontent.com/18540565/209907585-71324206-b900-47d9-bfe6-05a2dbaddf28.mp4

/home/image-builder/jma-image-build/

sudo build/setup_packer_configs.sh 1-24 raw rockylinux s3://projectbuildpipeline-857-pipelineoutputartifactsb-10ajmk30khe3f /home/image-builder/jma-image-build/eks-anywhere-build-tooling/projects/kubernetes-sigs/image-builder/_output/tar/1-24/raw/rockylinux/ 1-23 latest image-builder/images/capi


/home/image-builder/jma-image-build/

sudo PACKER_FLAGS="-force" PACKER_LOG=1 PACKER_LOG_PATH=/home/image-builder/jma-image-build/eks-anywhere-build-tooling/projects/kubernetes-sigs/image-builder/_output/tar/1-24/raw/rockylinux/packer.log PACKER_VAR_FILES="/home/image-builder/jma-image-build/eks-anywhere-build-tooling/projects/kubernetes-sigs/image-builder/_output/1-24/raw/rockylinux/config/kubernetes.json /home/image-builder/jma-image-build/eks-anywhere-build-tooling/projects/kubernetes-sigs/image-builder/_output/1-24/raw/rockylinux/config/common.json /home/image-builder/jma-image-build/eks-anywhere-build-tooling/projects/kubernetes-sigs/image-builder/_output/1-24/raw/rockylinux/config/cni.json /home/image-builder/jma-image-build/eks-anywhere-build-tooling/projects/kubernetes-sigs/image-builder/_output/1-24/raw/rockylinux/config/additional_components.json " make -C image-builder/images/capi build-raw-rockylinux-8













