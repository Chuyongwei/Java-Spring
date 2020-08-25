## 导入准备

### 针对mysql8的修改

1. 导入doucment中的mybatisdb.sql

    1. 创建数据库eesy_Mybaties
    
    2. 将mysql-connect版本改成8.0.20
    
2. 修改资源中的bean包的数据库
    
    + `com.sql.jdbc.Driver`改成`com.mysql.cj.jdbc.Driver`
    
    + `url`中`properties`要添加`?useUnicode=true&characterEncoding=utf-8&useSSL=false&serverTimezone = GMT`
    
      在`xml`中`?useUnicode=true&amp;characterEncoding=utf-8&amp;useSSL=false&amp;serverTimezone = GMT`
    
    + `password`修改密码
    
day02_eesy_01的xml导properties文件使用绝对路径 