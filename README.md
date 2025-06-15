# Simple Notes App for TWS Community
This is a simple notes app built with React and Django.

## Requirements
1. Python 3.9
2. Node.js
3. React

## Nginx

Install Nginx reverse proxy to make this application available

## MySQL
It is for Database

## Installation
1. Clone the repository
```
git clone https://github.com/infoguru19/django-notes-app.git
```

2. Build the app
```
docker build -t notes-app .
```

3. Run the Docker Compose
```
docker compose up --build
```

4. Check Containers.
```
root@master:~# docker ps
CONTAINER ID   IMAGE        COMMAND                  CREATED         STATUS                   PORTS                                         NAMES
5a840a6e6184   nginx        "/docker-entrypoint.…"   2 minutes ago   Up 2 minutes             0.0.0.0:80->80/tcp, [::]:80->80/tcp           nginx_cont
0c0a8dea23d7   django_app   "sh -c 'python manag…"   2 minutes ago   Up 2 minutes (healthy)   0.0.0.0:8000->8000/tcp, [::]:8000->8000/tcp   django_cont
d0fa8a81f1ce   mysql        "docker-entrypoint.s…"   2 minutes ago   Up 2 minutes (healthy)   3306/tcp, 33060/tcp                           db_cont
root@master:~#
```
5. Check Notes-App in Browser with ip
```
http://<IP>/
```
![image](https://github.com/user-attachments/assets/494dd81c-d355-486c-be43-bfb340d7be50)


