## portainer step by step commmad 
  
   **Run the following command to create a named volume** 
  ```
  docker volume create portainervolume
  ```
  **Run Portainer with the Volume**
  ```
  docker run -d -p8000:8000 -p9000:9000 --name portainer -v /var/run/docker.sock:/var/run/docker.sock -v portainervolume:/data portainer/portainer-ce:latest
  ```
  **List Running Containers**
    ```
  docker ps
    ```
  **Stop the portainer**
    ```
  docker stop portainer
    ```
  **Remove the Container**
    ```
  docker rm portainer
    ```
    
  
