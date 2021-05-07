# Spring介绍



[toc]

## 文件目录

```powershell
.
|-- README.md
|-- spring_day01
|   |-- day01_eesy_01jdbc
|   |-- day01_eesy_02factory
|   |-- day01_eesy_03spring
|   |-- day01_eesy_04bean
|   `-- day01_eesy_05DI
|-- spring_day02
|   |-- day02_eesy_01anno_ioc
|   |-- day02_eesy_02account_xmlioc
|   |-- day02_eesy_03account_annoioc
|   `-- day02_eesy_04account_annoioc_withoutxml
|-- spring_day03
|   |-- day03_eesy_01account
|   |-- day03_eesy_02proxy
|   |-- day03_eesy_03springAOP
|   |-- day03_eesy_04adviceType
|   `-- day03_eesy_05annotationAOP
|-- spring_day04
|   |-- day04_eesy_01jdbctemplate
|   |-- day04_eesy_02account_aoptx_xml
|   |-- day04_eesy_03account_aoptx_anno
|   |-- day04_eesy_04tx
|   |-- day04_eesy_05tx_xml
|   |-- day04_eesy_06tx_anno
|   |-- day04_eesy_07anno_tx_withoutxml
|   |-- day04_eesy_08account_tx
|   `-- day04_eesy_09jdk8
`-- tree.txt
```

## 使用

### 针对mysql8的修改

1. 导入doucment中的account.sql

    1. 创建数据库eesy
    
    2. 将mysql-connect版本改成8.0.20
    
2. 修改资源中的bean包的数据库
    
    + `com.sql.jdbc.Driver`改成`com.mysql.cj.jdbc.Driver`
    
    + `url`要添加`?useUnicode=true&characterEncoding=utf-8&useSSL=false&serverTimezone = GMT`  或者`?useUnicode=true&amp;characterEncoding=utf-8&amp;useSSL=false&amp;serverTimezone = GMT`
    
    + `password`修改密码
    