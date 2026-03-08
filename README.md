# Docker Lab Tasks and Solutions

---

## Problem 1: Basic Container Operations (hello-world)

### Task
Work with the `hello-world` container to practice basic Docker operations.

### Steps

#### 1. Run the hello-world container
![Running hello-world container](image.png)

#### 2. Check the container status
![Container status check](image-1.png)

#### 3. Start the stopped container
![Starting the stopped container](image-2.png)

#### 4. Remove the container
![Removing the container](image-3.png)

#### 5. Remove the image
![Removing the image](image-4.png)
![Image removal confirmation](image-5.png)

---

## Problem 2: Interactive Container with CentOS/Ubuntu

### Task
- Run container CentOS or Ubuntu in an interactive mode
- Run the following command in the container: `echo docker`
- Open a bash shell in the container and touch a file named `hello-docker`
- Stop the container and remove it. Write your comment about the file `hello-docker`
- Remove all stopped containers

### Solution
![Interactive container operations](image-6.png)

### Comment
> **Note:** The hello-docker file is deleted with the container. Container filesystems are ephemeral by default.

---

## Problem 3: MySQL Database Deployment

### Task
Deploy a MySQL database called `app-database` with the following requirements:
- Use the `mysql` latest image
- Use the `-e` flag to set `MYSQL_ROOT_PASSWORD` to `P4sSw0rd0!`
- The container should run in the background

### Solution
![MySQL container deployment](image-7.png)

---

## Problem 4: Nginx Container with Static Files

### Task
- Run the Nginx image
- Add HTML static files to the container and make sure they are accessible
- Commit the container with image name `IMAGE_NAME`

### Solution

#### Running and configuring Nginx container
![Running Nginx container](image-8.png)
![Adding HTML files](image-9.png)
![Verification step 1](image-10.png)
![Verification step 2](image-11.png)
![Container configured](image-12.png)

---

## Problem 5: Python Application Containerization

### Task
- Create a Python simple app
- Create a Dockerfile to containerize the Python app
- Build the image and test it

### Solution

#### Python application and Dockerfile
![Python app and Dockerfile creation](image-13.png)

#### Building and testing the image
![Building the Docker image](image-14.png)
![Testing step 1](image-15.png)
![Testing step 2](image-16.png)

---
# lab2
## Problem 1: Docker Named Volumes

### Volumes Configuration
- **Volume1**: for containing static html file
- **Volume2**: for containing nginx configuration

![alt text](image-17.png)

![alt text](image-18.png)

## Steps

### 1. Edit the html content

![alt text](image-19.png)

### 2. Remove the container

![alt text](image-20.png)

### 3. Run a new 2 containers with the following:

- Attach the two volumes that were attached to the previous container using volume mount
- Map port 80 to port 8080 on your host machine

![alt text](image-21.png)

### 4. Access the html files from your browser

**Port 8080:**

![alt text](image-22.png)

**Port 8081:**

![alt text](image-23.png)


---

# Problem 2: Docker Bind Mounts

## Objective
Run a container Nginx with name nginx-bind-mount and attach 2 volumes using bind mount under any paths

![alt text](image-24.png)

## Steps

### 1. Remove the container

![alt text](image-25.png)

### 2. Run a new container with the following:

- Attach the two volumes that were attached to the previous container

![alt text](image-26.png)

- Check the old data in the new containers

![alt text](image-27.png)




## Task

### 1. Create the Networks

![Networks configuration](<Screenshot 2026-03-08 221128.png>)

### 2. Create the Nginx Container

![Nginx container creation](image-32.png)

### 3. Create the Flask App Container (The Bridge)

![Flask app container creation](image-34.png)

### 4. Create the MariaDB Container

![MariaDB container creation](image-33.png)

### 5. Verification (The Curl Test)

![Curl test result 1](image-38.png)

![Curl test result 2](image-39.png)