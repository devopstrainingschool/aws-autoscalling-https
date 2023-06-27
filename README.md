# aws-autoscalling-https
### You can run this when creating ec2 via user data:
```
#!/bin/bash
/usr/bin/yum -y install httpd
/sbin/chkconfig httpd on
/sbin/service httpd start
/bin/echo “Welcome to my web server. My private IP is” > /var/www/html/index.html
curl http://checkip.amazonaws.com >> /var/www/html/index.html
```
