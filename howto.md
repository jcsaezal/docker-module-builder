$ docker image build -t lin-alpine --build-arg KERNEL_REF=docker/for-desktop-kernel:5.15.49-13422a825f833d125942948cf8a8688cef721ead  --build-arg BUILD_REF=alpine:3.13 jc

$ docker container run -it --privileged --rm -v ${PWD}/module:/module lin-alpine bash