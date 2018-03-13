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
# cd geeqie-1.3.tar.xz
# make
# make install
```
