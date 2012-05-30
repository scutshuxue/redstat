redstat
=======

redis stat tools like iostat using python

使用方法如下：
[admin@vm-dw-174-101 redis-dump-load]$ ./redstat -h
Usage: redstat -H hostname -w password [ [ ] ]

Options:
-h, --help show this help message and exit
-H HOST, --host=HOST The redis server you want to connect to
-w PASSWD, --password=PASSWD
The password used to connect to the redis server
-p PORT, --port=PORT The port the redis server is using
-t TIMEOUT, --timeout=TIMEOUT
socket timeout to redis server
默认连接本地的redis，localhost:6379

$./redstat -H 10.20.174.140 -w redis 1 10
[2012-05-30 15:59:22] connects clients memory_used role commands memory_peak last_save_time
[2012-05-30 15:59:22] 159 1 1.71G master 1 3.78G 2012-05-04 13:48:40
[2012-05-30 15:59:23] 159 1 1.71G master 1 3.78G 2012-05-04 13:48:40
[2012-05-30 15:59:24] 159 1 1.71G master 1 3.78G 2012-05-04 13:48:40
[2012-05-30 15:59:25] 159 1 1.71G master 1 3.78G 2012-05-04 13:48:40
[2012-05-30 15:59:26] 159 1 1.71G master 1 3.78G 2012-05-04 13:48:40
[2012-05-30 15:59:27] 159 1 1.71G master 1 3.78G 2012-05-04 13:48:40
[2012-05-30 15:59:28] 159 1 1.71G master 1 3.78G 2012-05-04 13:48:40