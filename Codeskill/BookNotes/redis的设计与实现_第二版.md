
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
* 链表
  * 链表和链表节点的实现
  * 链表和链表节点的API
* 字典
  * 字典的实现
    * 哈希表
    * 哈希表节点
    * 字典
  * 哈希算法
  * 解决键冲突
  * rehash
  * 渐进式 rehash
  * 字典API
* 跳跃表
  * 跳跃表的实现
    * 跳跃表节点
      * 层
      * 前进指针
      * 跨度
      * 后退指针
      * 分值和成员
    * 跳跃表
  * 跳跃表的API
* 整数集合
  * 整数集合的实现
  * 升级
  * 升级的好处
  * 降级
  * 整数集合API
* 压缩列表
  * 压缩列表的构成
  * 压缩列表节点的构成
    * pervious_entry_length
    * encoding
    * content
  * 连锁更新
  * 压缩列表API
* 对象
  * 对象的类型和编码
    * 类型
    * 编码和底层实现
  * 字符串对象
    * 编码的转换
    * 字符串命令的实现
  * 列表对象
    * 编码转换
    * 列表命令的实现
  * 哈希对象
    * 编码转换
    * 哈希命令的实现
  * 集合对象
    * 编码的转换
    * 集合命令的实现
  * 有序集合对象
    * 编码的转换
    * 有序集合命令的实现
  * 类型检查与命令多态
    * 类型检查的实现
    * 多态命令的实现
  * 内存回收
  * 对象共享
  * 对象的空转时长
## 单机数据库的实现
## 多机数据库的实现
## 独立功能的实现
