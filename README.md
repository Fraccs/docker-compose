# docker-compose `main-server`

> 🐋 docker-compose deployments on `main-server`.

## Useful information

### Interpolation of `docker-compose.yml` files

Some `docker-compose.yml` require interpolation. To achieve that, place the variables that have to be interpolated in a `.env` file.

### Environment variables

Each stack that uses environment variables contains a `.template.env` file (or `.template.<service>.env` in case of multiple services in the stack) with some configuration values set by default. Secrets are defaulted to a blank string. When deploying make sure to fill the empty secrets.

When cloning the repository for the first time, rename the `.template.*env` files to `*.env` with the following command:

```sh
find . -type f -name '.template.*env' -exec sh -c 'mv $1 "$(echo "$1" | sed 's/\.template//')"' _ "{}" \;
```

## Deployments

| Container Name | Container Image | Host Port | Internal Port |
|----------------|-----------------|-----------|---------------|
| authelia | [authelia/authelia:latest](https://hub.docker.com/r/authelia/authelia) | 10000 | 9091 |
| firefly | [fireflyiii/core:latest](https://hub.docker.com/r/fireflyiii/core) | 10050 | 8080 |
| grafana | [grafana/grafana-oss:latest](https://hub.docker.com/r/grafana/grafana-oss) | 10060 | 3000 |
| homeassistant  | [linuxserver/homeassistant:latest](https://hub.docker.com/r/linuxserver/homeassistant) | 10070 | 8123 |
| homepage | [ghcr.io/benphelps/homepage:latest](https://github.com/benphelps/homepage/pkgs/container/homepage) | 10071 | 3000 |
| jellyfin | [jellyfin/jellyfin:latest](https://hub.docker.com/r/jellyfin/jellyfin) | 10090 | 8096 |
| lidarr | [linuxserver/lidarr:latest](https://hub.docker.com/r/linuxserver/lidarr) | 10110 | 8686 |
| muse | [codetheweb/muse:latest](https://hub.docker.com/r/codetheweb/muse) | / | / |
| nextcloud | [nextcloud:latest](https://hub.docker.com/_/nextcloud/) | 10130 | 80 |
| nextcloud-mariadb | [mariadb:latest](https://hub.docker.com/_/mariadb) | / | 3306 |
| nginx-proxy-manager | [jc21:nginx-proxy-manager:latest](https://hub.docker.com/r/jc21/nginx-proxy-manager) | 10131,10132,10133 | 80,81,443 |
| photoprism | [photoprism/photoprism:latest](https://hub.docker.com/r/photoprism/photoprism) | 10157 | 2342 |
| pihole | [pihole/pihole:latest](https://hub.docker.com/r/pihole/pihole) | 53,10150 | 53,80 |
| portainer | [portainer/portainer-ce:latest](https://hub.docker.com/r/portainer/portainer-ce) | 10151 | 9443 |
| portfolio | [ghcr.io/fraccs/portfolio:latest](https://github.com/Fraccs/portfolio/pkgs/container/portfolio) | 10152 | 80 |
| portfolio-api | [ghcr.io/fraccs/portfolio-api:latest](https://github.com/Fraccs/portfolio-api/pkgs/container/portfolio-api) | 10153 | 5174 |
| prometheus | [prom/prometheus:latest](https://hub.docker.com/r/prom/prometheus) | 10154 | 9090 |
| prometheus-node-exporter | [prom/node-exporter:latest](https://hub.docker.com/r/prom/node-exporter) | / | 9100 |
| protonvpn | [linuxserver/wireguard:latest](https://hub.docker.com/r/linuxserver/wireguard) | / | / |
| prowlarr | [linuxserver/prowlarr:latest](https://hub.docker.com/r/linuxserver/prowlarr) | 10156 | 9696 |
| qbittorrent | [linuxserver/qbittorrent:latest](https://hub.docker.com/r/linuxserver/qbittorrent) | 10160,10161/tcp,10161/udp | 10160,6881/tcp,6881/udp |
| radarr | [linuxserver/radarr:latest](https://hub.docker.com/r/linuxserver/radarr) | 10170 | 7878 |
| readarr | [linuxserver/readarr:nightly](https://hub.docker.com/r/linuxserver/readarr) | 10171 | 8787 |
| romm | [zurdi15/romm:latest](https://hub.docker.com/r/zurdi15/romm) | 10172 | 8080 |
| romm-mariadb | [mariadb:latest](https://hub.docker.com/_/mariadb) | / | 3306 |
| samba | [dperson/samba:latest](https://hub.docker.com/r/dperson/samba) | 139,445 | 139,445 |
| sonarr | [linuxserver/sonarr:latest](https://hub.docker.com/r/linuxserver/sonarr) | 10180 | 8989 |
| syncthing | [linuxserver/syncthing:latest](https://hub.docker.com/r/linuxserver/syncthing) | 10181,10182/udp,10183/tcp,10183/udp | 8384,21027/udp,22000/tcp,22000/udp |
| watchtower | [containrrr/watchtower:latest](https://hub.docker.com/r/containrrr/watchtower/tags) | 10220 | 8080 |
