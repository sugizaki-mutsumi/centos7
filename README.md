# centos7

## svn 1.9
```
# cat /etc/yum.repos.d/wandisco-svn.repo 
[WandiscoSVN]
name=Wandisco SVN Repo
baseurl=http://opensource.wandisco.com/centos/$releasever/svn-1.9/RPMS/$basearch/
enabled=1
gpgcheck=0

# yum remove subversion*
# yum clean all
# yum install subversion
# svn --version
```


## geeqie
```
# yum -y install intltool
# yum -y install doxygen
# yum -y install glib2-devel
# yum -y install gtk3-devel
# tar xvf geeqie-1.3.tar.xz
# cd geeqie-1.3
# ./autogen.sh
# make
# make install
```

### epel
```
# yum -y install yum-plugin-priorities 
# sed -i -e "s/\]$/\]\npriority=1/g" /etc/yum.repos.d/CentOS-Base.repo 

# yum -y install epel-release 
# sed -i -e "s/enabled=1/enabled=0/g" /etc/yum.repos.d/epel.repo 
# yum --enablerepo=epel install [package name]

### pip
# yum --enablerepo=epel install python2-pip
```
