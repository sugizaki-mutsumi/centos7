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
