# DEVOPS-VIRTUALIZATION-AND-CONFIGURATION-MANAGEMENT
Daily Progress
### Basic Docker commands
* Docker -version
* docker info
* docker images or docker image ls
* docker run [image_name] echo "{message}"
* docker run --name {container_name} [image_name] echo "{message}"
* docker history https(image name)
* docker pull httpd(image name)
* docker run httpd echo "Hello World!"
* docker run -it ubuntu (open linux in terminal)
* docker run image
* docker run container_name
* docker rm container name
* docker stop container-name
* docker rm container1 container2(delete multi container)
* docker rm -f $(docker ps -aq)(for reset)
* docker ps(show run status)
* docker ps -a(show everything)
* docker run -it ubuntu(change into root directory of Linux)
* whoami(Linux command)
* `docker run -p 80:80 nginx`
* `docker run -e MY_VAR =value httpd env (set and check environment varibale)`
* `docker run -it -e MY_NAME=NAVNEET ubuntu bash`
* `check krne ke liye - echo $MY_NAME`
* Passing Environment variable from host system:
	1.  `$env:APP_PORT=8080` -> Powershell ; `export APP_PORT=8080` -> Ubuntu
	2. Check host variable -> `echo $env:APP_PORT`
	3. `docker run -e APP_PORT=$env:APP_PORT nginx env` 
	4. create a project and change the path to directory of that folder then run -> `docker run --env-file .env nginx env`
