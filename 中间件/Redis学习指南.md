# Redis学习指南
### 1.使用Homebrew安装、启动、重启、关闭Redis服务端
> 安装<br>
> brew install redis 

> 启动<br>
> brew services start redis

> 重启<br>
> brew services restart redis

> 关闭<br>
> brew services stop redis

### 2.Redis基础操作
> 设置链接密码（或直接修改redis.conf配置文件）<br>
> config set requirepass (密码)

> 链接Redis客户端<br>
> redis-cli

> 切换数据库 (所有操作使用13号库）<br>
> select (数据库编号0-15)

> 查看当前库下所有数据<br>
> keys *

### redis不同数据类型的存储结构以JSON格式表示如下:
>字符串(String)是最基本的类型,它的 value 就是字符串内容。<br>
 哈希(Hash)是字段-值(field-value)映射表,适合用于存储对象。<br>
 列表(List)是简单的字符串列表,按插入顺序排序。<br>
 集合(Set)是字符串的无序集合,元素不能重复。<br>
 有序集合(ZSet)是带分数的字符串元素集合,并按分数排序。<br>
```json
String:
  "key": "value"
Hash:
    "key": {
        "field1": "value1",
        "field2": "value2"
    }
List:
    "key": [
        "value1",
        "value2"
    ]
Set:
    "key": {
        "value1",
        "value2"
    }
ZSet:
    "key": [
        {"score": 0.1, "member": "value1"},
        {"score": 0.2, "member": "value2"}
    ]
```

### 常用命令50条
```
1. SET key value - 设置值
2. GET key - 获取值
3. DEL key - 删除键
4. EXISTS key - 检查键是否存在
5. EXPIRE key seconds - 设置键的过期时间
6. TTL key - 获取键的剩余过期时间
7. INCR key - 将键的整数值递增1
8. DECR key - 将键的整数值递减1
9. INCRBY key increment - 将键的整数值递增increment
10. DECRBY key decrement - 将键的整数值递减decrement
11. APPEND key value - 向键 appending 值
12. STRLEN key - 获取键值的长度
13. SETNX key value - 键不存在时,设置键值
14. MSET key value [key value ...] - 批量设置多个键值对
15. MGET key [key ...] - 批量获取多个键值
16. KEYS pattern - 查找匹配模式的键
17. TYPE key - 返回键的类型
18. FLUSHDB - 删除当前数据库所有键
19. FLUSHALL - 删除所有数据库键
20. RANDOMKEY - 随机返回一个键
21. RENAME key newkey - 重命名键
22. RENAMENX key newkey - 仅键不存在时重命名键
23. DBSIZE - 返回当前数据库键数量
24. EXPIREAT key timestamp - 设置键的过期unix时间戳
25. PTTL key - 以毫秒返回键的剩余过期时间
26. GETSET key value - 设置新值并获取旧值
27. GETRANGE key start end - 获取键值的范围子字符串
28. SETRANGE key offset value - 用值覆写键值的子字符串
29. SETBIT key offset value - 对键的二进制表示进行位操作
30. GETBIT key offset - 获取键的二进制表示位的值
31. BITCOUNT key - 统计键值被设置为1的比特数
32. BITOP operation destkey key - 对一个或多个键进行位操作
33. SADD key member - 向集合添加元素
34. SREM key member - 从集合移除元素
35. SPOP key - 随机移除并返回集合中的元素
36. SMEMBERS key - 返回集合中的所有元素
37. SUNION key [key ...] - 返回多个集合的并集
38. SUNIONSTORE destination key - 将集合并集保存到目标键
39. SINTER key [key ...] - 返回集合的交集
40. SDIFF key [key ...] - 返回集合的差集
41. SCARD key - 获取集合中的元素数量
42. SISMEMBER key member - 检查元素是否在集合中
43. SRANDMEMBER key - 随机返回集合中的元素
44. SSCAN key cursor - 迭代集合中的元素
45. ZADD key score member - 向有序集合添加元素
46. ZRANGE key start stop - 获取有序集合片段
47. ZREM key member - 从有序集合移除元素
48. ZCARD key - 获取有序集合中的元素数量
49. ZCOUNT key min max - 统计值在min和max之间的元素数
50. ZRANK key member - 获取元素的索引排名 
```



### 3.字符串String
> <br>
>

> <br>
>

> <br>
>

> <br>
>

> <br>

> <br>
>

> <br>
>

> <br>
>

> <br>
>

> <br>
>

> <br>
>

> <br>
>

> <br>
>

> <br>
>

> <br>
