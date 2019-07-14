# systemd_test
## Environment
```
[CPU]
processor       : 0
model name      : Intel(R) Atom(TM) CPU  C2750  @ 2.40GHz
processor       : 1
model name      : Intel(R) Atom(TM) CPU  C2750  @ 2.40GHz

[MEMORY]
MemTotal:        2049756 kB

[KERNEL]
Linux hostname 4.4.88-mainline-rev1 #1 SMP Wed Sep 13 23:49:03 UTC 2017 x86_64 x86_64 x86_64 GNU/Linux

[DISTRIBUTION]
Ubuntu 16.04.1 LTS \n \l

[LANGUAGES]
gcc (Ubuntu 5.4.0-6ubuntu1~16.04.10) 5.4.0 20160609
g++ (Ubuntu 5.4.0-6ubuntu1~16.04.10) 5.4.0 20160609
Python 2.7.12
Python 3.5.2
GNU Make 4.1
cmake version 3.5.1
Docker version 17.09.0-ce, build afdb6d4
```
## Requirement
* systemd running on host
## How To Use
```
$ docker-compose up -d
Creating network "systemdtest_default" with the default driver
Creating systemdtest_systemd_test_1 ... 
Creating systemdtest_systemd_test_1 ... done
$ docker exec -it systemdtest_systemd_test_1 /bin/bash
root@XXXXXXXXXXXX:/# systemctl status
● 052899b20ae4
    State: running
...
```
