FROM registry.access.redhat.com/ubi8/ubi-minimal:8.3

ARG TARGETARCH

LABEL name="MinIO" \
      vendor="MinIO Inc <dev@min.io>" \
      maintainer="MinIO Inc <dev@min.io>" \
      version="v4.0.0" \
      release="v4.0.0" \
      summary="MinIO Operator brings native support for MinIO, Console, and Encryption to Kubernetes." \
      description="MinIO object storage is fundamentally different. Designed for performance and the S3 API, it is 100% open-source. MinIO is ideal for large, private cloud environments with stringent security requirements and delivers mission-critical availability across a diverse range of workloads."

COPY CREDITS /licenses/CREDITS
COPY LICENSE /licenses/LICENSE

COPY logsearchapi_${TARGETARCH} /logsearchapi

CMD ["/logsearchapi"]
