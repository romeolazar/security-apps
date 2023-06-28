# Home Media Server

LANG=:us:

### Prerequisites.
- A public domain name. Buy one at [https://www.namecheap.com/](https://www.namecheap.com/)
- Use one for free at [https://duckdns.org](https://duckdns.org)
- Docker: [https://docs.docker.com/get-started/](https://docs.docker.com/get-started/)
- Docker Compose: [https://github.com/docker/compose/releases](https://github.com/docker/compose/releases)
- Server platform: [Rocky Linux 8](https://rockylinux.org/download)

# Applications
## security-apps
### [Nginx-Proxy-Manager](https://nginxproxymanager.com)
Proxy server that expose your services easily and securely. \
DockerHub: [jc21/nginx-proxy-manager](https://hub.docker.com/r/jc21/nginx-proxy-manager) \
GitHub: [jc21/nginx-proxy-manager](https://github.com/jc21/nginx-proxy-manager)

### [Vaultwarden](https://bitwarden.com/)
Offers the easiest and safest way for teams and individuals to store and share sensitive data from any device. \
DockerHub: [vvaultwarden/server](https://hub.docker.com/r/vaultwarden/server) \
GitHub: [bitwarden/server](https://github.com/bitwarden/server)

### [adGuardHome](https://adguard.com/en/welcome.html)
AdGuardHome is a network-wide software for blocking ads and tracking. After you set it up, it'll cover all your home devices, and you won't need any client-side software for that. \
DockerHub: [adguard/adguardhome](https://hub.docker.com/r/adguard/adguardhome) \
GitHub: [AdguardTeam/AdGuardHome](https://github.com/AdguardTeam/AdGuardHome/wiki/Docker)

## Info
Because all the services are setup with `docker-compose` they can all reach each other by their Docker Compose service name. So for example when connecting Sonarr with Jacket or qBittorrent, then Jackett would be available on `http://jackett/api....`, which makes everything a lot easier.

### Edit the .env file
All configuration to this setup, I've put in the `.env` file, so all you have to do is go through it and edit it to fit your needs.
