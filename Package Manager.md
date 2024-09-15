#package_manager
# compiler vs interpreter (المترجم)
compiler :
- after writing the source code of program you compile it → convert to binary file 
interpreter : 
- script languages like PHP, Bash, Python, Ruby , … 
# program : 
## compiled code that  stored on disk
# Application :
## compiled code that is running now in memory 
# package :
- البرنامج كاملا بكل ال dependencies بتاعته جاهز للتغشيل يمعلم  

---

1. بالنبسة ل Debian  عندك `dbkg`  بس لسة موجود مشكلة ال dependencies
2. لحل مشكلة ال dependencies + package  فال debian وكل مشتقاتها بقا عندك `apt`
# apt Package Manager :
- configration files are in /etc/apt/sources.list

- اولا اعمل update قبل كل شئ
```bash
$ apt update
```

- to install 
```bash
$ apt install اسم الباكدج 
```

- to check if package installed or no
```bash
$ apt list -a سم الباكدج
```

- to search for a package but you don’t remember the name 
```bash
$ apt search الاسم اللي انت فاكره | grep الاسم
ex : $ apt search vim | grep vim
```

- to delete package 
```bash
$ apt remove اسم الباكدج 
```

___

1. بالنبسة ل RedHat  عندك `rpm`  بس لسة موجود مشكلة ال dependencies
2. لحل مشكلة ال dependencies + package  ف RedHat وكل مشتقاتها بقا عندك `yum` or `dnf` 

> [!NOTE] rpm
> rpm \[option] \[path] package name  

- to check if package are installed or no
```bash
$ rmp -qi -p اسم الباكدج

#-p are used when package are not installed but exist on device

```

- to delete the package use this 
```bash
$ rmp -ev اسم الباكدج
```

