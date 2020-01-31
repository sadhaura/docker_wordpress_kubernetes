                                  Wordpress App built with Docker Compose and kubernetes
For Docker:-

Enviroments:-
. Mysql5.7
. phpmyadmin
. wordpress

Installation:-
Clone this repository on your local computer. 


1. git clone https://github.com/sadhaura/docker_wordpress.git

2. cd docker_wordpress

3.Run the below command

docker-compose up -d

Your Wordpress App is now ready!! You can access it via http://localhost:8087.

You can access phpmyadmin via http://localhost:9006 with username root and password somewordpress

For Kubernetes:-

Requirements:-

You must have kubernetes cluster up and running.

1. Clone this repository on your kubernetes cluster

git clone https://github.com/sadhaura/docker_wordpress_kubernetes.git

2. cd docker_wordpress_kubernetes/kubernetes

3. Run the below command

kubectl create -f apache.yml,configmap.yml,secret.yml,mysql.yml,volume.yml

your kubernetes deployments,pods,service will be up and running with persistent volume for database.

You can check access your website with EXTERNAL IP of kubernetes service(my-wordpress-server).

 




