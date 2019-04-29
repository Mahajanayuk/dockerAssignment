# dockerAssignment
Docker-PHP-nginx Project
The project has three components:
The PHP-FPM wordpress.
Database (MySQL) that will store your blog posts
A web server (NGINX) that will proxy requests on HTTP and HTTPS.


Steps: 
Clone the project.
cd to project directory
create keys as follows:

sudo openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout <project-dir>/nginx/certs/nginx-selfsigned.key -out <project-dir>/nginx /certs/selfsigned.crt

create dh param key as :

sudo openssl dhparam -out <project-dir>/nginx/certs/RSA2048.pem 2048
  

Run docker compose file as:

docker-compose up -d (-d for detatched mode)

see the running containers as:

docker ps



