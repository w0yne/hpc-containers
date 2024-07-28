FROM public.ecr.aws/amazonlinux/amazonlinux:2

USER root

# Install necessary dependencies
RUN amazon-linux-extras install epel -y && \
    yum update -y && \
    yum install -y stress-ng

CMD ["stress-ng", "--matrix", "0", "-t", "5m", "--times"]