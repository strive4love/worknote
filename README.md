** Windows监控端口使用情况的命令：netstat --ano | findstr "8080"   问：Linux怎么查？

** taskkill /PID 9060 /F  ##杀掉9060端口的进程

** 镜像与分光的区别？ https://blog.csdn.net/primeprime/article/details/78934784

**有人把SVN提交到错误的分支了，怎么办？
答：

** deligate to somebody to do something 委派某人做某事

========================================pengpeng operation===============================
[root@localhost createlog]# nohup ./createlog &
[1] 8547
[root@localhost createlog]# nohup: ignoring input and appending output to `nohup.out'

[root@localhost createlog]# 
[root@localhost createlog]# tailf nohup.out 
./createlog: error while loading shared libraries: libboost_regex.so.1.60.0: cannot open shared object file: No such file or directory
./createlog: error while loading shared libraries: libboost_regex.so.1.60.0: cannot open shared object file: No such file or directory
Open /opt/apm/probe/data/eth0//2017_08_28_00_18-25-2772.stream.temp failed.
./createlog: error while loading shared libraries: libboost_regex.so.1.60.0: cannot open shared object file: No such file or directory
Open /opt/apm/pAgent/flume/2017_12_05_14_24-46-0547.stream.temp failed.
^C

[root@localhost apm]# cd pAgent/flume/
[root@localhost flume]# ll
total 92
-rw-r--r--. 1 root root 81920 Jul 18 16:37 2018_07_18_08_37-10-6075.stream.temp
-rw-r--r--. 1 root root 12288 Jul 25 14:24 2018_07_25_06_24-41-8756.stream.temp


[root@localhost flume]# watch -d -n 1 'du -sh'
You have new mail in /var/spool/mail/root
=========================================
