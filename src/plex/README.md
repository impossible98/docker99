# Plex

## Usage

```bash
# https://github.com/plexinc/pms-docker/blob/master/README.md
# port 32400
docker run --detach \
    --device=/dev/dri:/dev/dri \
    --name plex \
    --network=host \
    --restart always \
    --volume $PWD/config/:/config/ \
    --volume $PWD/transcode/:/transcode/ \
    --volume <path>:/data/ \
    plexinc/pms-docker
```
