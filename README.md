# lvm2
repo for the lvm2 spec and rpm build files for centos6/el6 

## steps to build this projekt

First we need the development packages:

```
yum install libselinux-devel libsepol-devel ncurses-devel readline-devel corosynclib-devel openaislib-devel clusterlib-devel python2-devel libudev-devel
```

download this repo and go into
```
git clone git@github.com:afdata/lvm2.git
cd lvm2
```

Build the project
```
rpmbuild --define "_sourcedir $PWD" -ba *.spec
```

