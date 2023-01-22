docker run -d --rm -v mongo-data:/data/db -e MONGO_INITDB_ROOT_USERNAME=admin -e MONGO_INITDB_ROOT_PASSWORD=admin-passsword --name mongodb mongo
docker run -d --rm -v /app/node_modules -v logs:/app/logs -v /home/mrburnwal/Desktop/pythonTest/multi-container-deployment/backend:/app -e USERNAME=admin -e PASSWORD=admin-password -p 80:80 --name back-cont back-img
docker run --rm -it --name front-cont -p 3000:3000 --network goal-net -v /home/mrburnwal/Desktop/pythonTest/multi-01-starting-setup/frontend/src:/app/src front-img

