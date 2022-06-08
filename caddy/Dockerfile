FROM caddy:2.5.1-builder AS builder

RUN xcaddy build \
    --with github.com/caddy-dns/cloudflare \
    --with github.com/lucaslorentz/caddy-docker-proxy/v2@2.7.1

FROM caddy:2.5.1

COPY --from=builder /usr/bin/caddy /usr/bin/caddy