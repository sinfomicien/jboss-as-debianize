jboss-as-debianize
==================

JBoss AS 7 debianize scripts by me :)

First you have to clone this repo:
git clone git@github.com:sinfomicien/jboss-as-debianize.git

Then download the jboss-as tar.gz file from:
http://download.jboss.org/jbossas/7.1/jboss-as-7.1.1.Final/jboss-as-7.1.1.Final.tar.gz

Then you rename it:
```
mv jboss-as-7.1.1.Final.tar.gz jboss-as_7.1.1.Final.orig.tar.gz
```

The you untar it:
```
tar -zxvf jboss-as-7.1.1.Final.tar.gz
```

Go into the new extracted directory:
```
cd jboss-as-7.1.1.Final
```

Copy the debian directory from this repository
```
cp ../jboss-as-debianize/debian .
```

Launch the build:
```
debuild -us -uc
```

Enjoy!!
