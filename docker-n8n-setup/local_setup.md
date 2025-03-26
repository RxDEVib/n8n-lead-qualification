# Setting Up n8n Locally Using Docker

To install docker on your machine, Please visit: <a href = "https://docs.docker.com/get-started/get-docker/">Docker Installation</a>

Follow these steps to set up n8n locally using Docker:

Open Terminal on your machine:<br>
If you have <b>Linux</b>: To open Terminal on your machine, press `Ctrl + Alt + T`.<br>
If you have <b>MacOs</b>: To open Terminal on your machine, press `Cmd + Space` and type `Terminal`.<br>
If you have <b>Windows</b>: To open Command Prompt, press `Win + R`, type `cmd`, and press `Enter`.

## Step 1: Create a Volume in Docker to Persist Data
Create a volume to store n8n data, ensuring it is retained across container restarts.
```bash
docker volume create n8n_data
```

## Step 2: Confirm That the Volume Has Been Created
Verify the volume's existence using the following command:
```bash
docker volume list
```
You should see `n8n_data` listed.

## Step 3: Create a Docker Container
Run the following command to create and start an n8n container:
```bash
docker run --name n8n -p 5678:5678 -v n8n_data:/home/node/.n8n docker.n8n.io/n8nio/n8n
```
- `--name n8n` → Names the container `n8n`
- `-p 5678:5678` → Maps port 5678 on your host to port 5678 on the container
- `-v n8n_data:/home/node/.n8n` → Mounts the volume to store n8n data persistently

## Step 4: Verify the Container is Running
Check if the container is running using:
```bash
docker ps
```
You should see the `n8n` container in the list.

## Step 5: Access n8n Web Interface
Open your browser and navigate to:

http://localhost:5678

You can now create workflows and automate tasks using n8n.

---
Enjoy building your workflows with n8n! If you encounter any issues, check the container logs using:
```bash
docker logs n8n
```

## 6. Create Workflows

Create your first workflow in the n8n web interface
Explore available nodes and start automating!

### Additional Tips:

To stop the container: <code>docker stop n8n</code><br>
To start the container again: <code>docker start n8n</code><br>
To remove the container: <code>docker rm n8n</code><br>

### Persistent Data
Your workflows and settings will be saved in the n8n_data volume, ensuring data persistence between container restarts.

### Additional Resources
- **For Any Doubts:** Refer to the official n8n documentation on local setup: [Local Setup Guide](https://docs.n8n.io/hosting/installation/docker/)