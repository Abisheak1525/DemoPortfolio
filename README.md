This only a demo website this isn't my main port folio

#!/bin/bash

yum update -y

yum install httpd -y

yum install git -y

git clone https://github.com/Abisheak1525/abi.git /tmp/mywebsite

cp -R /tmp/mywebsite/* /var/www/html/

systemctl enable httpd

systemctl start httpd
