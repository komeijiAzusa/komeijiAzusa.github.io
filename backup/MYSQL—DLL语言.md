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


