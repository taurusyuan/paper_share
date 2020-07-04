# data_quiz
## 关于大数据开发岗位面试的一些资料总结和经验

一. 关于数据结构
1. **大话数据结构（精华版总结）**：https://www.cnblogs.com/anliux/p/10802321.html
* 说明：刷题前必看，分章节对《大话数据结构》这本书的重点和精华部分的概括（对于来不及看书er超级有用）。
2. **数据结构**：https://github.com/Jack-Lee-Hiter/AlgorithmsByPython/blob/master/%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84.md
* 说明：刷完上面的每一章之后看这个链接里对应的内容，是一种更加精简概括，适合用来巩固和面试前复习。
3. **二叉树**的分支介绍和详细总结：https://blog.csdn.net/zhaoyun_zzz/article/details/88393380  &  https://zhuanlan.zhihu.com/p/27700617

二. 关于SQL
1. **group by时select后跟聚合函数与否的剖析**：https://blog.csdn.net/u014717572/article/details/80687042
2. **on和where的区别**：https://www.jianshu.com/p/d923cf8ae25f
* 概括说明：先执行 on，后执行 where；on 是建立关联关系(无论条件真假都会建表，不辨真伪)，where 是对关联关系的筛选（在建表后辨真伪完成筛选）。
3. **各种表连接的区别**：https://www.runoob.com/sql/sql-join.html
>外连接outer join：
>>* left join：联结结果保留左表的全部数据
>>* right join：联结结果保留右表的全部数据
>>* full join：联结结果保留左右表的全部数据

>内连接inner join：取两表的公共数据
>交叉连接cross join：返回被连接的两个表的笛卡尔积，返回结果的行数等于两个表行数的乘积(注意：select * from 表1，表2实现自身级联，和cross join一样也是笛卡尔积的结果)
>上下连接union：内部的每个select语句必须拥有相同数量的列，列也必须拥有相似的数据类型，同时每个select语句中的列的顺序必须相同。



三. 关于Python

0. **时间/空间复杂度分析**：https://blog.csdn.net/haha223545/article/details/93619874
1. **切片**：https://www.jianshu.com/p/15715d6f4dad
2. **复制/浅拷贝/深拷贝**：https://blog.csdn.net/bufengzj/article/details/90486991
* 说明：常用的是浅拷贝（".copy()"或者"[:]"），而不是深拷贝".deepcopy()"；深拷贝与浅拷贝唯一区别是除了外围元素，内层元素也做了复制，原数据变化后，复制的数据不会变化；浅拷贝只复制了外围元素，原数据外围元素变化时复制数据不变，但是原数据内层元素变化时复制数据跟着变化；复制（即"="）前后，原数据和复制数据的id相同，浅拷贝和深拷贝前后数据的id不同。
【备注：浅拷贝只复制指向某个对象的指针，而不复制对象本身，新旧对象还是共享同一块内存。但深拷贝会另外创造一个一模一样的对象，新对象跟原对象不共享内存，修改新对象不会改到原对象】
3. **continue 和 break 的区别**：https://www.cnblogs.com/NancyRM/p/7998088.html
4. **双边队列**https://www.cnblogs.com/lincappu/p/12890765.html



