# For OpenShift Deployments

### Docker build
From solution directory
docker build  -f ./ReactDotNetTS.Server/Dockerfile.OpenShift -t quay.io/dbrugger946/noclient-weather-server:latest  .  
docker run -p 8888:8080 quay.io/dbrugger946/noclient-weather-server:latest  
docker push quay.io/dbrugger946/noclient-weather-server:latest

OR  
docker/podman build  -f ./ReactDotNetTS.Server/Dockerfile.OpenShift -t quay.io/dbrugger946/noclient-weather-server:latest --platform linux/amd64,linux/arm64 . 