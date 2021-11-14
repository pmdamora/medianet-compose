# Media Net Configuration
This `docker-compose.yml` file contains the basic configuration for setting up a NZBGet/Transmission/Sonarr/Radarr/Jellyfin media server. This is intended for use on a Synology NAS.

## Quickstart
- Create the needed directories:
`sudo mkdir -p ${HOST}/data/{torrents/{tv,movies},{usenet/{tv,movies},media/{tv,movies}}`
`sudo mkdir -p ${HOST}/docker/appdata/{ONE FOR EACH DOCKER SERVICE}`

- Setup portainer
Follow the steps in Portainer's [documentation](https://docs.portainer.io/v/ce-2.9/start/install/server/docker/linux#deployment).

- Deploy stack in portainer
Open portainer and deploy the medianet stack using the `docker-compose.yml` file in this repository.

- Configure applications
Configure all of the application settings, referencing the examples in this [guide](https://trash-guides.info/Hardlinks/Examples/) to get hardlinking and atomic moves working.
