# MySql
Mysql常用工具

#常用的SQL语法

#1.SQL的模式匹配  以Hello开头，以o或者e结尾，中间全部是数字字母或者空格
SELECT * FROM dic_soft WHERE soft_name REGEXP '^Hello[a-zA-Z0-9 ]+[eo]$';

#2.转义字符使用，匹配'_'和'%'的方法  意思就是说/之后的_不作为通配符
SELECT * FROM dic_soft WHERE soft_name LIKE 'hello/_%' ESCAPE '/';
