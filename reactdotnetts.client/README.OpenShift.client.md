## OpenShift Client app

npm run dev  
  


docker build -f ./Dockerfile.OpenShift -t quay.io/dbrugger946/vite-weather-client:latest .  
docker run --name weather-client -p 3000:3000 quay.io/dbrugger946/vite-weather-client:latest  
docker push quay.io/dbrugger946/vite-weather-client:latest  

docker compose up
docker compose down
