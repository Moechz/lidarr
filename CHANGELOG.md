# Changelog

All notable user-visible changes to the Lidarr TOS application package.

## 3.1.6-1 — 2026-11-08

### Added
- First release. Lidarr (`linuxserver/lidarr:3.1.6.5079-ls47`, Docker Hub official image, unmodified)
  packaged as a TOS 7 Docker application, published on port 8018 and running
  as a non-root user (1000:1000).
- Persistent data is kept under `/Volume1/DockerAppData/lidarrdocker/`.

### Architectures
- Dual-architecture release: `lidarrdocker_x86_64.tar.gz` (4052 B, `c87481496ecabb9ead67c7ab834827b00994ecb70f629ca84c894c4ade29c424`) and
  `lidarrdocker_aarch64.tar.gz` (4054 B, `33238662f42a8b62276fea3203156cc25a047c837e87230576ea6ae6c914b51f`), built by `scripts/build-dual.sh`.
  x86_64 has the full on-device E2E; aarch64 passes the official check and the
  platform validation (no ARM host available for a container E2E).
