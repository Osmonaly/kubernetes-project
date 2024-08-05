#kub#

#For the next project, the following steps were required:


#Create an RDS or CloudSQL instance, connect to your database, and create tables inside the #PostgreSQL database.
#Create a secret with your hostname, username, password, and database name.
#Clone these repositories locally:
#https://github.com/AntTechLabs/awesome_cats_backend.git
#https://github.com/AntTechLabs/awesome_cats_frontend.git
#Write Dockerfiles for frontend and backend images.
#Push your images to private repositories in ECR or GCR.
#Write YAML files for backend and frontend deployments with 2 replicas, and show database #credentials as environment variables.
#Create ClusterIP services for your deployments.
#Install an NGINX controller and create an ingress to access your application with a load #balancer.
#Configure your domain name with Cloud DNS or Route53 and ExternalDNS, and access the Awesome #Cats application from a web browser using your domain name.
#Obtain a certificate for your domain name with cert-manager.
#Since I couldn't add external repositories, I was only able to add my own YAML files to my #repository for the successful completion of this final project.

#The first step was to create a database in AWS or GCE. I chose Google Cloud and decided to #deploy everything on this cloud server because all my Kubernetes projects were hosted here.
![image](https://github.com/user-attachments/assets/5598a056-cd21-479d-aa42-00b995a3f0de)

#Next, I needed to connect to the database:
![image](https://github.com/user-attachments/assets/532abfe8-dd7e-4d33-9b29-912536435bf0)

#The second step was to create secret.yaml to store and manage private data such as username, #password, and database name.
![image](https://github.com/user-attachments/assets/7f74c8e5-1b76-476d-b66a-c0f137b98ab5)

#The third step was to clone the corresponding backend and frontend repositories:
https://github.com/AntTechLabs/awesome_cats_backend.git
https://github.com/AntTechLabs/awesome_cats_frontend.git  

#The fourth step involved writing Dockerfiles for the backend and frontend images and storing #them in our prepared repository in Google Cloud:
 ![image](https://github.com/user-attachments/assets/34df36e7-eb3c-4805-82a8-71126868f12c)
#Push to private repos in GCR:
 ![image](https://github.com/user-attachments/assets/de88f7d0-e97c-4abe-9bd7-f6bd0ede19b2)
 ![image](https://github.com/user-attachments/assets/dfd0192b-cf79-48db-a5af-5e3fc6788619)

#The next steps involved writing YAML files for frontend and backend deployments:
![image](https://github.com/user-attachments/assets/300f3585-ca4f-4172-a446-bae87bcea24b)
#They can be seen in this repository with detailed descriptions.

#The seventh step was to create services for deployments using ClusterIP type. In the following #screenshot, you can see not only the primary services but also additional ones:
![image](https://github.com/user-attachments/assets/9158aa41-add2-4633-984e-13c3f84515fd)

#The eighth step was to install the NGINX controller, choosing the Load Balancer type:
![image](https://github.com/user-attachments/assets/a054d9fa-3eca-45ef-b284-8c346934d5c7)
![image](https://github.com/user-attachments/assets/3e726223-92f4-4e83-8003-16e6e5d9e2e5)
#After this step, you could open the site using the pre-purchased DNS name:
![image](https://github.com/user-attachments/assets/d3fb4f6d-8e74-44f1-967b-62d0d894a27e)


#The penultimate step was to open the site using the DNS name:

![image](https://github.com/user-attachments/assets/a9847184-6f14-4fba-8c0e-b967342337b7)
#In this screenshot, you can see the connection to the database that was created by me.

#Here, you can see successful registration and login to the game:

![image](https://github.com/user-attachments/assets/d7009df7-247e-4fbb-bef2-5c2f7d00a4ef)

#And try multiple characters for the game:
![image](https://github.com/user-attachments/assets/b0d03a65-03c4-48e4-ba64-0b6c460d0cb4)

#The final step was to obtain a certificate for my DNS, which I was able to get through steps #such as ClusterIssuer.yaml and Certificate.yaml, where using specific configurations I could #obtain a certified certificate for my site:
![image](https://github.com/user-attachments/assets/4605565e-80e2-4943-852e-618e257550d7)


#This project took me three full days to complete successfully. Since I already had experience #obtaining a certificate for my site, this time it took longer to correctly set up the backend #and frontend parts.
#While completing this project, I reinforced all my knowledge of Kubernetes, Docker, and #previously studied tools.

#I hope you understand my work!














