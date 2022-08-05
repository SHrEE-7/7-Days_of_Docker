# **Day-2**
### Web server configuration on container


Day 2 of learing Dcoker 🐋 was fully based on web server configuration on container, creating own image using commit command of configured container and pushing it on **hub.docker.com**. 


Three Steps to configure webserver
1. install httpd 
2. configure (put web pages) / Deploy
3. Start service
   
following commands will help to confihure webserver
```
[root@dockeruser ~]# yum install httpd -y 

[root@dockeruser ~]# cd /var/www/html (put webpages in this directory)

[root@dockeruser ~]# systemctl start httpd or /usr/sbin/httpd
```
To persist the configuration after reboot add the /usr/sbin/httpd or systemctl start httpd command in /root/.bashrc 

commands to be added in /root/.bashrc
``` 
rm -f /var/run/httpd/httpd.pid (removes pid of stoped service)
/usr/sbin/httpd
```

Create own image which has all the configuration setup ready
```docker commit <container name> <image name:tag/version>```
this command will creates new image.

To push your image on dockerhub, login to docker hub account and use the following syntax to push image.
```docker tag <created_image_name:version> dockerhub_id/<created_image_name:version>```
New image with name tag. name tag should be same as your docker hub id 

```docker push dockerhub_id/<created_image_name:version>``` (push image on dockerhub)

### Handwritten notes are also uploaded..have a look..!
### Contributions are always welcome. feel free to open full request.