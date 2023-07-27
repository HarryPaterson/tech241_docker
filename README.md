<h1 style="text-align: center;">Docker</h1>

### Contents
* Installation
* Architechture
* Create Image

### Docker Installation
![](https://i.imgur.com/H8jc6XA.png)
1. Download at https://docs.docker.com/desktop/install/windows-install/
2. Follow instructions to install
3. Verify installation with 
```
docker --version
```
4. Update windows subsystem with
```
wsl --update
```
### Hyper V
1. Through control panel navigate to Programs -> Programs and Features
2. Turn Windows Features on or off
3. Check Hyper-V
4. Restart system to take effect

### API 
![](https://geekflare.com/wp-content/uploads/2019/09/docker-architecture-609x270.png)

### Create Docker Image
1. docker run -d -p 80:80 nginx
2. alias docker="winpty docker"
3. docker exec -it 12bf4fe17ca2 sh
4. cd /usr/share/nginx/html
5. apt update + apt upgrade
6. apt install nano
7. nano index.html
8. Make changes and save + exit
9. exit
10. docker commit 12bf4fe17ca2 harrypaterson/nginx-tech241
11. docker push harrypaterson/nginx-tech241
12. docker run -d -p 100:80 harrypaterson/nginx-tech241

