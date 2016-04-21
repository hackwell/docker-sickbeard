# docker sickbeard
This is a Dockerfile to set up "Sickbeard" - (http://sickbeard.com/)
Build from docker file
```
git clone https://github.com/hackwell/docker-sickbeard.git
cd docker-sickbeard
docker build -t sickbeard .
```
```
docker run -d \
  -h *your_host_name* \
  -v /*your_config_location*:/config \
  -v /*your_videos_location*:/data \
  -p 8081:8081 \
  --restart=always sickbeard
```
