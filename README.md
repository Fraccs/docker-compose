# docker-compose `main-server`

> 🐋 docker-compose deployments on `main-server`.

| Container Name | Container Image | Host Port | Internal Port |
|----------------|-----------------|-----------|---------------|
| authelia | [authelia/authelia:latest](https://hub.docker.com/r/authelia/authelia) | 10000 | 9091 |
| barsempione49 | [httpd:2.4-bullseye](https://hub.docker.com/_/httpd) | 10010 | 80 |
| grafana | [grafana/grafana-oss:latest](https://hub.docker.com/r/grafana/grafana-oss) | 10060 | 3000 |
| homeassistant  | [lscr.io/linuxserver/homeassistant:latest](https://hub.docker.com/r/linuxserver/homeassistant) | 10070 | 8123 |
| homepage | [ghcr.io/benphelps/homepage:latest](https://github.com/benphelps/homepage/pkgs/container/homepage) | 10071 | 3000 |
| jellyfin | [jellyfin/jellyfin:latest](https://hub.docker.com/r/jellyfin/jellyfin) | 10090 | 8096 |
| kavita | [linuxserver/kavita:latest](https://hub.docker.com/r/linuxserver/kavita) | 10100 | 5000 |
| lidarr | [linuxserver/lidarr:latest](https://hub.docker.com/r/linuxserver/lidarr) | 10110 | 8686 |
| muse | [codetheweb/muse:latest](https://hub.docker.com/r/codetheweb/muse) | / | / |
| nextcloud | [nextcloud:latest](https://hub.docker.com/_/nextcloud/) | 10130 | 80 |
| nextcloud-mariadb | [mariadb:latest](https://hub.docker.com/_/mariadb) | / | 3306 |
| nginx-proxy-manager | [jc21:nginx-proxy-manager:latest](https://hub.docker.com/r/jc21/nginx-proxy-manager) | 10131,10132,10133 | 80,81,443 |
| onlyoffice-documentserver | [onlyoffice/documentserver:latest](https://hub.docker.com/r/onlyoffice/documentserver) | 10140 | 80 |
| pihole | [pihole/pihole:latest](https://hub.docker.com/r/pihole/pihole) | 53,10150 | 53,80 |
| portainer | [portainer/portainer-ce:latest](https://hub.docker.com/r/portainer/portainer-ce) | 10151 | 9443 |
| portfolio | [ghcr.io/fraccs/portfolio:latest](https://github.com/Fraccs/portfolio/pkgs/container/portfolio) | 10152 | 80 |
| prometheus | [prom/prometheus:latest](https://hub.docker.com/r/prom/prometheus) | 10153 | 9090 |
| prometheus-node-exporter | [prom/node-exporter:latest](https://hub.docker.com/r/prom/node-exporter) | / | 9100 |
| prowlarr | [linuxserver/prowlarr:latest](https://hub.docker.com/r/linuxserver/prowlarr) | 10154 | 9696 |
| qbittorrent | [linuxserver/qbittorrent:latest](https://hub.docker.com/r/linuxserver/qbittorrent) | 10160,10161/tcp,10161/udp | 10160,6881/tcp,6881/udp |
| radarr | [linuxserver/radarr:latest](https://hub.docker.com/r/linuxserver/radarr) | 10170 | 7878 |
| readarr | [linuxserver/readarr:latest](https://hub.docker.com/r/linuxserver/readarr) | 10171 | 8787 |
| sonarr | [linuxserver/sonarr:latest](https://hub.docker.com/r/linuxserver/sonarr) | 10180 | 8989 |
| syncthing | [lscr.io/linuxserver/syncthing:latest](https://hub.docker.com/r/linuxserver/syncthing) | 10181,10182/udp,10183/tcp,10183/udp | 8384,21027/udp,22000/tcp,22000/udp |
| uptime-kuma | [louislam/uptime-kuma:latest](https://hub.docker.com/r/louislam/uptime-kuma) | 10200 | 3001 |
| watchtower | [containrrr/watchtower:latest](https://hub.docker.com/r/containrrr/watchtower/tags) | 10220 | 8080 |
