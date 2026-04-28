# 基本查询
## 使用select语句查询多个字段
查询某一列：select 字段1,字段2,字段3 from 表名
查询所有：   select *from 表名;

## 设置别名、
select 字段1 as别名 from 表名;

# 条件查询

<img width="746" height="505" alt="Image" src="https://github.com/user-attachments/assets/442bfac2-d9c6-4ac2-be43-7d25606b8d00" />

# 聚合函数
格式 select 聚合函数(字段) from 表名 where 条件;
聚合函数有 max(最大值 ) min(最小值) avg(平均值) count(统计数量) sum(求和)

# 分组查询

select 字段名 from 表名 where 条件 group by 分组字段名 having 分组后过滤条件;
其中，where在分组前进行过滤，不满足where的不参与分组，having是分组后的过滤条件
在where中不能使用聚合函数






