FROM jaegertracing/all-in-one@sha256:d035b283aad95248ff9afd3cfc49e4f25e622f4b06c97ced60e12229d5688418
HEALTHCHECK \
    --interval=1s \
    --timeout=1s \
    --start-period=1s \
    --retries=60 \
    CMD wget -q --header='Content-Type:application/json' -O - http://localhost:14269/health | grep "Server available"
