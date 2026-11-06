FROM debian:bookworm-slim

RUN apt-get update && apt-get install -y --no-install-recommends \
      procps tree nano less file bc python3 \
    && rm -rf /var/lib/apt/lists/*

RUN useradd -m -u 1000 -s /bin/bash pixi

USER pixi
WORKDIR /home/pixi
CMD ["sleep", "infinity"]

