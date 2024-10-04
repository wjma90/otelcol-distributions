FROM alpine:latest

ARG USER_UID=10001
USER ${USER_UID}

COPY otelcol-main /otelcol-main
COPY config.yaml /etc/otelcol-main/config.yaml
ENTRYPOINT ["/otelcol-main"]
CMD ["--config", "/etc/otelcol-main/config.yaml"]
EXPOSE 4317
