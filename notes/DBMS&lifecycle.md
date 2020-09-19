

# Lecture 01 What are Database Systems?

### Difference between Data and Information

<br>

数据: known, available「已知的信息储备,可以直接使用」<br>
信息: processed, more useful 「处理过,更有用」— 存在在DBMS里面的描述性文本

### Database Management system (DBMS)

#### -> Difinition

A software system designed to store, manage, and facilitate access todatabases. <br>「数据库系统基本上是为大量数据而开发的。当有大量的数据处理,有需要优化两两件事:[[检索数据-retrieval]]和[[检索数据-retrieval]]」<br>
[[数据存储-Storage]]: 占用更少的空间>因为冗余数据（重复数据）在存储前已被删除<br>
[[检索数据-retrieval]]:可以快速检索数据>在急需的时候

#### -> Advantages [compare with File Processing Systems]

-=> 文件处理系统的坏处: <br><br>[Data redundancy]数据冗杂也就是数据重复,<br>[Data inconsistency]数据不一致>一般是由于数据冗杂导致的>e.g.两个人身份证号一摸一样,<br>[Data Isolation]数据分散在各种文件里格式什么的不统一>难以检索,<br>[Dependency on application programs]对于应用程序的依赖,<br>[Atomicity issues]执行的动作难以回滚,<br>[Data security]应该设置权限

-=> DBMS 的好处: <br><br>[几乎和上面是对应的]<br>[No redundant dat] by [data normalization],<br>[Data Consistency and Integrity],<br>[Data Security] ,<br>[Privacy],<br>[Easy access to data ],<br>[Easy recovery]易于恢复 数据库系统保留数据备份,<br>[Flexible]

-=> DBMS 的缺点: <br><br>[Expensive]贵,<br>[Complexity]数据库系统难以理解,[Performance]<br>DBMS的通用使其适合于各种应用程序>此功能会影响其在某些应用程序中的性能

---
---
# Lecture 02 Database Development Process

### 
#### -> Outline

{[Database Planning] >> Database Definition >> Requirements Definition and Analysis}<br><br> => {Conceptual Design >> Logical Design >> Physical Design}<br><br> => {Application Design}<br> => {Implementation}<br> => {Testing}<br> => {Operational Maintenance}<br> => {回到第一个}<br>
[Database Planning]: <br>Planning how to do the project; how Enterprise work & Enterprise data model
<br>[Database Definition]: <br>Specifying scope and boundaries to users, application areas & How does the system interfere with other organisational systems知识水平是否可以维护,包括需要哪一个软件
<br>[Requirements Definition and Analysis]: <br>Collection and analysis of requirements需要对于需求进行理解和解析,看作设身处地,<br>



