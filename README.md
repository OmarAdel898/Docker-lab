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