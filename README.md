personal
========

vinnyScripts

``` Shell 
[hrtvxb@biopvm201 kakapo]$ docker build -t kakapotestlee - < Dockerfile
Sending build context to Docker daemon  2.56 kB
Sending build context to Docker daemon
Step 0 : FROM nimmis/apache-php5
 ---> e48d1888bc73
Step 1 : MAINTAINER Kiwifruit Data Gurus <kiwifruit-data-science@plantandfood.co.nz>
 ---> Using cache
 ---> 2dcba960191b
Step 2 : WORKDIR /var/www/html
 ---> Using cache
 ---> 922a5cf70065
Step 3 : ENV GITHUB_OWNER leeogrady
 ---> Using cache
 ---> 601d20679cda
Step 4 : ENV GITHUB_REPO kakapo
 ---> Using cache
 ---> 5da12a30f6db
Step 5 : ENV GITHUB_TOKEN 4ba02d5eff0aa10d144d45658e1499a023aaafd1
 ---> Using cache
 ---> ac7c9957b4ae
Step 6 : ENV GITHUB_BRANCH master
 ---> Using cache
 ---> 04b10bd8d193
Step 7 : ENV HTTPS_PROXY http://proxy.pfr.co.nz:8080
 ---> Using cache
 ---> 975e012e49dd
Step 8 : RUN apt-get -y update
 ---> Running in 086bd3f19b40
Err http://archive.ubuntu.com trusty InRelease

Err http://archive.ubuntu.com trusty-updates InRelease

Err http://archive.ubuntu.com trusty-security InRelease

Err http://archive.ubuntu.com trusty Release.gpg
  Cannot initiate the connection to archive.ubuntu.com:80 (2001:67c:1360:8c01::18). - connect (101: Network is unreachable) [IP: 2001:67c:1360:8c01::18 80]
Err http://archive.ubuntu.com trusty-updates Release.gpg
  Cannot initiate the connection to archive.ubuntu.com:80 (2001:67c:1360:8c01::18). - connect (101: Network is unreachable) [IP: 2001:67c:1360:8c01::18 80]
Err http://archive.ubuntu.com trusty-security Release.gpg
  Cannot initiate the connection to archive.ubuntu.com:80 (2001:67c:1360:8c01::18). - connect (101: Network is unreachable) [IP: 2001:67c:1360:8c01::18 80]
Reading package lists...
W: Failed to fetch http://archive.ubuntu.com/ubuntu/dists/trusty/InRelease

W: Failed to fetch http://archive.ubuntu.com/ubuntu/dists/trusty-updates/InRelease

W: Failed to fetch http://archive.ubuntu.com/ubuntu/dists/trusty-security/InRelease

W: Failed to fetch http://archive.ubuntu.com/ubuntu/dists/trusty/Release.gpg  Cannot initiate the connection to archive.ubuntu.com:80 (2001:67c:1360:8c01::18). - connect (101: Network is unreachable) [IP: 2001:67c:1360:8c01::18 80]

W: Failed to fetch http://archive.ubuntu.com/ubuntu/dists/trusty-updates/Release.gpg  Cannot initiate the connection to archive.ubuntu.com:80 (2001:67c:1360:8c01::18). - connect (101: Network is unreachable) [IP: 2001:67c:1360:8c01::18 80]

W: Failed to fetch http://archive.ubuntu.com/ubuntu/dists/trusty-security/Release.gpg  Cannot initiate the connection to archive.ubuntu.com:80 (2001:67c:1360:8c01::18). - connect (101: Network is unreachable) [IP: 2001:67c:1360:8c01::18 80]

W: Some index files failed to download. They have been ignored, or old ones used instead.
 ---> 19b502bcbc0e
Removing intermediate container 086bd3f19b40
Step 9 : RUN apt-get --assume-yes install php5-ldap
 ---> Running in b29fb51baa40
Reading package lists...
Building dependency tree...
Reading state information...
E: Unable to locate package php5-ldap
The command '/bin/sh -c apt-get --assume-yes install php5-ldap' returned a non-zero code: 100
```
