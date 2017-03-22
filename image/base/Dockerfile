FROM ubuntu:14.04.3
RUN apt-get update && \
    apt-get install -y qemu-kvm curl \
		       bridge-utils genisoimage curl jq
COPY startvm /var/lib/rancher/startvm
ENTRYPOINT ["/var/lib/rancher/startvm"]
VOLUME /image
EXPOSE 22
CMD []
