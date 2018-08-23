
Docker  Installing  .


2.Install packages to allow apt to use a repository over HTTPS:

   $ sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    software-properties-common
 
 
3.Add Docker’s official GPG key:

  $ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
  
  
  $ sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
   
   
 1.Update the apt package index:

   $ sudo apt-get update
   
 2.Install the latest version of Docker CE, or go to the next step to install a specific version:
   
   $ sudo apt-get install docker-ce
   
   
  --> docker --version or docker -v  
   
________________________________________________________________________________________________________________________________________________

  
  
  Link  docker  engine  to  docker hub : 
  
   
   sudo -s 
   
  ---> docker  login  
  
  UserName :kiranreddyg2
  Password:kiran&123
   
   cat /etc/*se
   
   docker  run(docker pull +docker  start)
   
   docker  run centos
   
   docker  run -it  centos /bin/bash 
   exit
   
   cat /etc/*se
   
   docker  images 
   
   docker ps 
   
   docker  start CID(container  ID )
   
   docker attach CID
   
   docker  ps  -a  
   
   docker  run  -it  --name  web1 centos /bin/bash 
   
   docker ps 
   
   docker rm -f web1 or CID
   
   
   docker  run  -it  --name  web1 centos /bin/bash 
   
   docker ps 
   
   create   some  files 
   
   docker commit web1 kiranreddg2/web1:v1
   
   docker push kiranreddg2/web1
   
   docker  rm CID (to remove  container)
   
   docker  rmi -f centos ( to remove  images )
   
   docker  ps  -a  -q  or  -aq 
   
   docker rm -f $(docker  ps  -aq ) .....to  remove  all containers
   
   
   docker  run -it --name  web1 kiranreddyg2/web1:v1 /bin/bash
   
   
   
   
   docker commit web1 kiranreddg2/web1:v1
	
   docker tag kiranreddg2/web1:v1 kiranreddyg2/jyothinewrepo:jyothi
   
   docker push  kiranreddyg2/jyothinewrepo:jyothi
   
-----------------------------------------------------------------------------------------------------------------------
   
   docker  search  centos 
   
   docker pull  centos  
   
   hostnmae  
   
   docker  run  -itd  centos  --....(detach  mode)

   control+p+q ..........(container will come  out but container  up and  running )
   
________________________________________________________________________________________________________________
   
   
   docker  exec CID  touch  "file_name"
   
   docker  exec CID  mkdir  folder-name 
   
   docker  exec CID  touch  "folder-name/file_name"
   
   
   (C groups)....search for  this  in google .
   
   
   Docket  Network :
   ..................
   
   cat /etc/hosts
   
   docker  inspect  CID 
   
   docker network  ls  
   
   docker network inspect CID 
   
   docker run -d  kiranreddg2/web2 sleep 60
   
   docker  ps 
   
   docker run -it -p 81:80 ubuntu /bin/bash 
   
   
   
   Installing apache:
   -------------------------
   
   
   apt-get update  
   
 
   apt-get install  apache2
   
   service apache2 start 
   
   ip:81
   
   docker  commit cid  apache ..........from  root  
   
   docker run -it -p 82:80 apache   /bin/bash 
   
   service  apache2 start 
   
   ps  -aux | grep  apache2
   
   echo "<h1>container 1</h1>" > /var/www/html/index.html 
   
   
   
   docker run -d  -p 82:80 apache   apachectl -d  . -e info  -DFOREGROUND............
   
   docker run -d  -p 82:80 apache   apachectl -f  /etc/apache2/apache2.conf  -e info  -DFOREGROUND
   
   docker  cp index.html  CID:/var/www/html/index.html
   
   
   docker run -d  -P  apache   apachectl -f  /etc/apache2/apache2.conf  -e info  -DFOREGROUND ..............random  port
