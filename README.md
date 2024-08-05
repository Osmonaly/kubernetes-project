# Project Overview: Awesome Cats Deployment

## For the Next Project, the Following Steps Were Required:

1. **Create a Database Instance**:
   - Set up an RDS or CloudSQL instance.
   - Connect to your database and create tables inside the PostgreSQL database.

2. **Create a Secret**:
   - Store your hostname, username, password, and database name in a secret.

3. **Clone Repositories**:
   - Clone the backend and frontend repositories:
     - [Backend Repository](https://github.com/AntTechLabs/awesome_cats_backend.git)
     - [Frontend Repository](https://github.com/AntTechLabs/awesome_cats_frontend.git)

4. **Write Dockerfiles**:
   - Create Dockerfiles for both frontend and backend images.
   - Push the images to private repositories in ECR or GCR.

5. **Write Deployment YAML Files**:
   - Develop YAML files for backend and frontend deployments with 2 replicas.
   - Configure database credentials as environment variables.

6. **Create ClusterIP Services**:
   - Set up ClusterIP services for your deployments.

7. **Install NGINX Controller**:
   - Install an NGINX controller and create an ingress to access your application with a load balancer.

8. **Configure Domain Name**:
   - Set up your domain name with Cloud DNS or Route53 and ExternalDNS.
   - Access the Awesome Cats application from a web browser using your domain name.

9. **Obtain SSL Certificate**:
   - Get a certificate for your domain name using cert-manager.

10. **Repository Limitations**:
    - Since external repositories could not be added, only my own YAML files were used for the successful completion of this project.

## Steps in Detail

### 1. Creating a Database
- I chose Google Cloud to deploy everything as all my Kubernetes projects were hosted there.
![Create Database](https://github.com/user-attachments/assets/5598a056-cd21-479d-aa42-00b995a3f0de)

### 2. Connecting to the Database
![Database Connection](https://github.com/user-attachments/assets/532abfe8-dd7e-4d33-9b29-912536435bf0)

### 3. Creating Secrets
- Created a `secret.yaml` to store and manage sensitive data such as username, password, and database name.
![Secrets Configuration](https://github.com/user-attachments/assets/7f74c8e5-1b76-476d-b66a-c0f137b98ab5)

### 4. Cloning Repositories
- Cloned the necessary backend and frontend repositories:
  - [Backend Repository](https://github.com/AntTechLabs/awesome_cats_backend.git)
    
  - [Frontend Repository](https://github.com/AntTechLabs/awesome_cats_frontend.git)

### 5. Writing Dockerfiles
- Created Dockerfiles for both backend and frontend images and pushed them to Google Cloud repositories.
![Dockerfile](https://github.com/user-attachments/assets/34df36e7-eb3c-4805-82a8-71126868f12c)

![Push to GCR](https://github.com/user-attachments/assets/de88f7d0-e97c-4abe-9bd7-f6bd0ede19b2)

![GCR Push](https://github.com/user-attachments/assets/dfd0192b-cf79-48db-a5af-5e3fc6788619)

### 6. Writing Deployment YAML Files
- Developed YAML files for frontend and backend deployments with detailed descriptions.
![Deployment YAML](https://github.com/user-attachments/assets/300f3585-ca4f-4172-a446-bae87bcea24b)

### 7. Creating ClusterIP Services
- Created ClusterIP services for the deployments.
![ClusterIP Services](https://github.com/user-attachments/assets/9158aa41-add2-4633-984e-13c3f84515fd)

### 8. Installing NGINX Controller
- Installed the NGINX controller with Load Balancer type.
![NGINX Controller](https://github.com/user-attachments/assets/a054d9fa-3eca-45ef-b284-8c346934d5c7)

![Load Balancer](https://github.com/user-attachments/assets/3e726223-92f4-4e83-8003-16e6e5d9e2e5)

### 9. Accessing the Site
- Opened the site using the pre-purchased DNS name.
![Access Site](https://github.com/user-attachments/assets/d3fb4f6d-8e74-44f1-967b-62d0d894a27e)

### 10. Final Steps
- Viewed the connection to the database and successful registration and login to the game.
![image](https://github.com/user-attachments/assets/0da81002-d32c-4088-a1da-56937b750ba7)

![Game Login](https://github.com/user-attachments/assets/d7009df7-247e-4fbb-bef2-5c2f7d00a4ef)

![Multiple Characters](https://github.com/user-attachments/assets/124ca5a5-287d-4bb9-9987-189c0c45c8db)


### Obtaining SSL Certificate
- Obtained a certificate using `ClusterIssuer.yaml` and `Certificate.yaml`.
![SSL Certificate](https://github.com/user-attachments/assets/4605565e-80e2-4943-852e-618e257550d7)

## Project Duration

- The project took three full days to complete. The time was extended due to the need for proper setup of backend and frontend components. This project reinforced my knowledge of Kubernetes, Docker, and other tools.

I hope you find this project and its details informative!














