# stuinfo_pyqt5

一个用pyqt5写的学生信息管理系统，能够访问本地sqlite数据库

1. 使用 python3，pyqt5 构建。

2. 由于连接的是本地的sqlite数据库，所以如果要修改连接数据库的方式以及某些参数的话，需要在data.py的init函数中进行修改。

3. 连接的数据库里面有两张表，分别叫做acount和stuinfo。其中acount主要储存的是用户的登陆账号和密码，有两个字段，分别是username和password，类型都是char(100) not null。stuinfo的表中主要储存的是学生的信息，有四个字段，分别是name，age，num和profession，分别储存学生的姓名，年龄，学号和专业，类型分别是char(10) not null，char(10) not null,char(20) not null,char(50) not null。

## 使用方法

gitclone代码库到本地之后，本地首先需要安装python（版本不一样应该也可以，但是一定要是3），之后进入代码目录执行pip install -r requirements.txt命令，最后在代码目录下使用python main.py命令启动程序即可。