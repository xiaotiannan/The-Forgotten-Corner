
##	数据结构与对象
* 简单动态字符串 simple dynamic string
  * SDS的定义
    * sdshdr-> free / len/buf(字节数组)
  * SDS与C字符串的区别
    * 常数复杂度获取字符串长度 len 字段记录
    * 杜绝缓冲区溢出
    * 减少修改字符串时带来的内存重分配次数
      * 空间预分配
        * len+len+1 = buf
        * 如果sds大于1m将最高分配1m
      * 惰性空间释放
    * 二进制安全 binary-safe
      * 使用len 属性来判断字符串是否结束
    * 兼容部分C字符串函数
  * SDS --API ---P17
    * sdsnew``创建一个包含C字符串的SDS``
    * sdsempty
    * sdsfree
    * sdslen
    * sdsavail
    * sdsdup
    * sdsclear
    * sdscat
    * sdscatsds
    * sdscpy
    * sdsgrowzero
    * sdsrange
    * sdstrim
    * sdscmp
