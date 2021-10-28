
#!/bin/bash
yum install httpd -y
systemctl enable httpd
mkdir /var/www/html/application1/
echo "<h1>This is a testing page for app1</h1>" > /var/www/html/application1/index.html
systemctl start httpd
