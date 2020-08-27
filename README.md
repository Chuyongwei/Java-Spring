## 导入准备

### 目录结构

```powershell
.
|-- README.md
|-- axis.log
|-- document
|   |-- Mybatis第二天讲义.pdf
|   |-- Mybatis第三天讲义.pdf
|   |-- Mybatis第四天讲义.pdf
|   |-- Mybatis第一天讲义.pdf
|   |-- jdbcConfig.properties
|   |-- log4j.properties
|   |-- mybatisdb.sql
|   `-- 截图
|-- mybatis_day01
|   |-- day01_eesy_01mybatis
|   |-- day01_eesy_02mybatis_annotation
|   |-- day01_eesy_03mybatis_dao
|   `-- day01_eesy_04mybatis_design
|-- mybatis_day02
|   |-- day02_eesy_01mybatisCRUD
|   `-- day02_eesy_02mybatsiDAO
|-- mybatis_day03
|   |-- day03_eesy_01datasourceAndTx
|   |-- day03_eesy_02dynamicSQL
|   |-- day03_eesy_03one2many
|   |-- day03_eesy_04many2many
|   `-- day03_eesy_05jndi
|-- mybatis_day04
|   |-- day04_eesy_01lazy
|   |-- day04_eesy_02cache
|   |-- day04_eesy_03annotation_mybatis
|   `-- day04_eesy_04annoOne2Many
`-- tree.txt
```



### 针对mysql8的修改

1. 导入doucment中的mybatisdb.sql

    1. 创建数据库eesy_Mybaties
    
    2. 将mysql-connect版本改成8.0.20
    
2. 修改资源中的bean包的数据库
   
    + `com.sql.jdbc.Driver`改成`com.mysql.cj.jdbc.Driver`
    
    + `url`中`properties`要添加`?useUnicode=true&characterEncoding=utf-8&useSSL=false&serverTimezone = GMT`
    
      在`xml`中`?useUnicode=true&amp;characterEncoding=utf-8&amp;useSSL=false&amp;serverTimezone = GMT`
    
    + `password`修改密码
    
### 问题

day02_eesy_01的xml导properties文件使用绝对路径 

day03_05的sqlMapConfig错误