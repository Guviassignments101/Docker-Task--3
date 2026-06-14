# Docker-Task--3
Task Description:  Create a custom docker image for nginx and deploy it using docker compose, where the volume bind mount should be at /var/opt/nginx location. Push the created custom docker image to your docker-hub.  Techstacks needs to be used :   AWS EC2 Docker Docker Compose

Step 1 : Launch EC2 and install docker 
<img width="1907" height="852" alt="image" src="https://github.com/user-attachments/assets/aefe2b35-9cbb-4845-ba30-ef095282702b" />

Step 2 : Buid Docker image
<img width="1898" height="605" alt="image" src="https://github.com/user-attachments/assets/68253d40-e547-4503-a742-42ecd499eb1e" />
<img width="1900" height="158" alt="image" src="https://github.com/user-attachments/assets/5f4430cb-cdda-42b7-89c4-04789e4883d0" />

Step 3 : Create Host Volume Directory and verify
sudo mkdir -p /var/opt/nginx
sudo cp index.html /var/opt/nginx/
ls /var/opt/nginx
<img width="1888" height="122" alt="image" src="https://github.com/user-attachments/assets/0440866a-4a18-4281-9573-858c92a4ded7" />

Step 4: Create docker-compose.yml
<img width="1908" height="673" alt="image" src="https://github.com/user-attachments/assets/aaa89fb5-20dc-4e1a-9ac1-85dcfeb796da" />

Step 5: Deploy using Docker Compose
<img width="1907" height="371" alt="image" src="https://github.com/user-attachments/assets/d7cf28cb-e23f-428b-b319-f0fb95c3a65d" />
<img width="1913" height="917" alt="image" src="https://github.com/user-attachments/assets/3fd751a7-559f-4995-af5f-6e72db669db3" />

Step 6: Push Image to Docker Hub
<img width="1882" height="412" alt="image" src="https://github.com/user-attachments/assets/83900219-3b0c-466f-a81c-0955fb78c2da" />
<img width="1911" height="560" alt="image" src="https://github.com/user-attachments/assets/1f6000aa-3578-460c-9ecd-b38733cbf929" />
<img width="1891" height="903" alt="image" src="https://github.com/user-attachments/assets/e5965a59-5569-4b8d-a8ff-21244e14b948" />

check volume mount 
docker inspect nginx-server
<img width="1901" height="478" alt="image" src="https://github.com/user-attachments/assets/a4f263e3-bbfe-4b10-979e-e5cb2afc94a6" />




