# linux-sys
---------------update bash---------------
[root@mail ~]# /bin/bash -version

GNU bash, version 3.2.25(1)-release (x86_64-redhat-linux-gnu)

Copyright (C) 2005 Free Software Foundation, Inc.

安装升级bash

wget http://ftp.gnu.org/gnu/bash/bash-5.1.tar.gz

tar zxvf bash-5.1.tar.gz

cd bash-5.1

./configure

make

make install

因为bash默认是安装在/usr/local/bin/目录下，所以需要创建一个链接到 /bin/目录下，安装完毕后需要重启生效！

mv /bin/bash /bin/bash.bak; ln -s /usr/local/bin/bash /bin/bash

[root@mail ~]# /bin/bash -version

GNU bash, version 4.2.0(1)-release (x86_64-unknown-linux-gnu)

Copyright (C) 2011 Free Software Foundation, Inc.

License GPLv3+: GNU GPL version 3 or later

This is free software; you are free to change and redistribute it.

There is NO WARRANTY, to the extent permitted by law.
