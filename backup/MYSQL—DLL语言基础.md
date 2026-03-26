 # 创建数据库
1，查询所有数据库
show databases;

<img width="246" height="235" alt="Image" src="https://github.com/user-attachments/assets/4555133b-e7d1-4249-96e1-d2093c497efe" />

2，创建数据库
<img width="1132" height="95" alt="Image" src="https://github.com/user-attachments/assets/f5a390cb-6093-4c5f-80b8-7393cdd4a44c" />

3，删除数据库
drop database {if exists} 数据库名称;

4,使用数据库，切换到输入的数据库中
use 数据库名称

5，select database();
查看当前所在的数据库

# 修改数据库

1，创建表
create table 表名(
名称1 数据类型 comment''注释
名称2 数据类型 comment''注释
名称3 数据类型 comment''注释
)comment'';

<img width="404" height="151" alt="Image" src="https://github.com/user-attachments/assets/4c2fc58d-bbd8-4eac-b063-c9862b2814c2" />

2，查询表内容desc+表名称;
<img width="597" height="176" alt="Image" src="https://github.com/user-attachments/assets/16c71d9e-9d07-4200-85b7-b3231793eb02" />

3，show tables
查看数据库中的所有表

4，向表中添加字段
alter table+表名 add+字段名+数据类型(长度)+comment'';

5，修改数据类型
alter table 表名 modify 字段名 数据类型(长度);

6，修改字段名与字段类型
alter table 表名 change 旧字段名 新字段名 数据类型(长度) comment'';

7，删除字段
alter table 表名 drop 旧字段

8，修改表名
alter table 旧表名 rename to 新表名；

9，删除表
drop table {if exists} 表名；


# 数据类型
1，数字的数据类型

<img width="1688" height="371" alt="Image" src="https://github.com/user-attachments/assets/c04b8c32-58c7-4814-bab3-db777d034acb" />
double使用中可标识长度（小数点前加小数点后加起来的长度）与小数位数（小数点后）如表示分数score 100.0 用
score double(4,1)

2，字符串数据类型
常用的有char与varchar
通常在使用中加入长度，如char(10)
varchar被称为变长字符串，会根据存储的内容计算存储空间，例如输入一个字符就占用一个字符的空间，性能较差；
char称为定长字符串，在char(10)中，输入占用的存储空间均为10，空缺会用空格补齐，性能好。

登陆界面的用户名一般使用varchar，用户名长度是变化的，可改变存储长度。


示例
create table employee(
id int comment'编号',
number_id varchar(10) comment'员工工号',
name varchar(10) comment'员工姓名',
gender varchar(1) comment'性别',
age tinyint unsigned comment'年龄',
idcard char(18) comment'身份证号',
employedtime date comment'入职日期'
) comment'员工表';

<img width="676" height="242" alt="Image" src="https://github.com/user-attachments/assets/cbba115a-fc6d-452f-a3b8-8d624fda96de" />

# 总结

<img width="878" height="745" alt="Image" src="https://github.com/user-attachments/assets/c213efba-3e71-4cad-b024-e6354fd82267" />
