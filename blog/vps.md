## 安装
[mysql 编译安装 博客园2013](http://www.cnblogs.com/xiongpq/p/3384681.html)--
[nginx pitfalls 陷阱](http://wiki.nginx.org/Pitfalls)--[nginx 配置](http://wiki.nginx.org/Configuration)

[creating-new-vhosts-on-Nginx](http://www.sebdangerfield.me.uk/2012/05/nginx-and-php-fpm-bash-script-for-creating-new-vhosts-under-separate-fpm-pools/)

[PHPFcgiExample](http://wiki.nginx.org/PHPFcgiExample)

             error_log  /var/log/nginx/error.log;
             /etc/php.ini
             /etc/nginx/conf.d/default.conf
             /etc/nginx/nginx.conf
             nginx -t -c /etc/nginx/nginx.conf
             
             cd sites-enabled
             sudo ln -s ../sites-available/foo.conf .
             ls -l

[rose 红玫瑰主机 joomla相关环境安装 ](http://www.rosehosting.com/blog/run-joomla-with-nginx-on-a-centos-vps/)


1. 更改php.ini
首先php.ini的配置中把
;cgi.fix_pathinfo=0   改为
cgi.fix_pathinfo=1


2. 在nginx/conf/nginx.conf   找到：
fastcgi_param  SCRIPT_FILENAME  /scripts$fastcgi_script_name;  改为：
fastcgi_param SCRIPT_FILENAME $document_root$fastcgi_script_name;
##### server com centos nginx 安装
[servermom nginx php 安装](http://www.servermom.org/how-to-build-working-centos-server-with-nginx-and-php/577/)--[binarytides](http://www.binarytides.com/)

[host1plus joomla 安装第一步失败](http://www.host1plus.com/tutorials/joomla/cannot-get-past-step-1-of-joomla-installation/)

## vhost相关

     文件位置       /usr/local/nginx/conf/vhost/
     80             /home/wwwroot/www.hadoopside.com
     8001           /home/wwwroot/hadoopside.com
     8002           /home/wwwroot/8002
     
     8011           /home/wwwroot/
     8021           /home/wwwroot/www.demo.com



### 优秀博客

[ccvita](http://www.ccvita.com/)--[nginx-php-fpm](http://www.if-not-true-then-false.com/2011/install-nginx-php-fpm-on-fedora-centos-red-hat-rhel/)
     service jenkins start 
     
#### tomcat http://www.hadoopside.com:8080/
#### jeksin http://www.hadoopside.com:9080/
#### 日志 http://hadoopside.com/log/
#### 控制台 https://199.231.87.194:4083/index.php?act=login
#### 账号管理 https://www.budgetvm.com/account
#### panel https://master.scalabledns.com:5656
#### ftp   http://hadoopside.com/ftp/
#### tomcat manager http://www.hadoopside.com:8080/manager/html
#### mysql http://www.hadoopside.com:8011


##### andriod manager http://hadoopside.com/ftpandriod/

     
     

## centos5.9 tomat install
1. [centos5.9](http://wavded.tumblr.com/post/258713913/installing-tomcat-6-on-centos-5)
2. [centos-unstall-openjdk--安装-jdk](http://hi.baidu.com/liangxiaoman/item/5f337804cbbde4edfe240d65)
3. hudson rpm安装完成后需要 rm registory.
4. 先装 lnmp 后装jdk-->tomcat6-->hudson(centos 自带)-->pureftpd(ftpuser)
5. [emacs](http://scc.ustc.edu.cn/zlsc/czxt/200910/W020100308601210472906.pdf)


## VPS控制台
1. [控制台](https://199.231.87.194:4083/index.php?act=login)
2. [hudson rpm install](http://wiki.hudson-ci.org/display/HUDSON/Installing+Hudson+using+RPM+repository) 注意装完后要 rm hudson.repo
3. [hudson 防火墙问题](http://www.cnblogs.com/haochuang/archive/2012/08/15/2640067.html)
4. [Running Hudson behind Nginx](http://wiki.hudson-ci.org/display/HUDSON/Running+Hudson+behind+Nginx)
5. [linux下常用 命令](http://www.vpser.net/build/linux-vps-ssh-command.html)
6. [centos 端口开放及关闭](http://www.cnblogs.com/winner/archive/2011/11/17/2252181.html)----依次执行三个命令
7. [如何对CentOS防火墙进行配置](http://blog.csdn.net/adparking/article/details/7612680)
8. [sftp--配置](http://linuxjcq.blog.51cto.com/3042600/717927)
9. [jdk--安装](http://zuoqiang.iteye.com/blog/1157422)
10. [linux 运维日志](http://www.centos.bz/about/)
11. [ldap centos](http://wiki.openiam.com/pages/viewpage.action?pageId=7635198)

## LNMP
1. [一键安装包----底部有配置文件位置](http://lnmp.org/install.html)
2. [hudson安装--后修改配置文件--端口9080--位置etc/sysconfig/hudson](http://blog.csdn.net/fbfsber008/article/details/7356323)
3. [hudson 防火墙问题](http://www.cnblogs.com/haochuang/archive/2012/08/15/2640067.html)
4. [hudson nginx设置](https://wiki.jenkins-ci.org/display/JENKINS/Running+Hudson+behind+Nginx)
5. [hudson--yum--install](http://wiki.eclipse.org/Hudson-ci/Installing_Hudson_RPM)
6. [pureftpd--教程](http://www.vpser.net/manage/lnmp-pureftpd-cp.html)
7. [php升级--5.3.10](http://www.vpser.net/manage/lnmp-upgrade-php-script.html)
8. [pureftpd--的权限控制](http://tech.it168.com/a2008/1226/261/000000261343.shtml)
9. [mysql innodb](http://www.hyh.me/blog/?p=20)

## yum install tomcat
1. [最简 yum install tomcat--/etc/tomcat6/tomcat-users.xml](http://www.unixmen.com/howto-install-tomcat-in-centos-fedora-the-easy-way/)
2. [tomcat user 设置](http://www.cnblogs.com/peter9/archive/2011/12/29/2362134.html)
3. [hudson tomcat 自动部署](http://www.avajava.com/tutorials/lessons/how-do-i-deploy-to-tomcat-using-ant.html)
4. [hudson-yum-安装后报错问题](http://naoboo.com/blog/2013/01/16/install-hudson/)
5. [tomcat6-安装文件-service tomcat6 start](http://wavded.tumblr.com/post/258713913/installing-tomcat-6-on-centos-5)


## 参考手册
1. [centos 参考手册](http://www.centos.bz/category/web-server/tomcat/)
2. nginx配置参数 nginx目录----/root/lnmp0.9-full/nginx1.0.15/conf/nginx.conf
3. [nginx 目录浏览功能](http://blog.licess.org/nginx-autoindex/)
4. [南京云维科技](http://kicklinux.com/service/)
5. [centos 运维](http://www.centos.bz/2011/03/windows-linux-transfer-data-tool-winscp/)
3. 
4. 

## 安全
1. [阻止扫描--DenyHosts--防 8080端口扫描](http://www.vpser.net/security/denyhosts.html)
2. [安全博客](http://www.lengmo.net/)
3. 

## budget主机新版配置安装
1. [LNMP一键安装包--底部有配置文件](http://lnmp.org/install.html)
2. [jenkins-安装](https://wiki.jenkins-ci.org/display/JENKINS/Installing+Jenkins+on+RedHat+distributions) 有配置和日志位置
3. [ant-jdk-安装](http://www.51testing.com/?uid-350678-action-viewspace-itemid-805565)

日志设置:
autoindex     on;
root  /var/log/;
1、vi /etc/profile
2、http://stackoverflow.com/questions/7532928/how-do-i-install-maven-with-yum
3、source /etc/profile 使环境变量生效

export M2_HOME=/usr/local/apache-maven/apache-maven-3.0.5

[inmotinghost教程](http://www.inmotionhosting.com/support/edu/joomla-3)
在ftp用户上传时更改权限 chown -R ftp1 /usr/local/ftphome

nginx日志设置
    location /log {
        autoindex on;
        root         /var/;
    }
    

