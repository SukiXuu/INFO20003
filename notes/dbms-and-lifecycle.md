# DBMS&lifecycle

## Lecture 01 What are Database Systems?

### Difference between Data and Information

数据: known, available「已知的信息储备,可以直接使用」  
 信息: processed, more useful 「处理过,更有用」— 存在在DBMS里面的描述性文本

### Database Management system \(DBMS\)

#### -&gt; Difinition

A software system designed to store, manage, and facilitate access todatabases.   
「数据库系统基本上是为大量数据而开发的。当有大量的数据处理,有需要优化两两件事:[\[检索数据-retrieval\]](https://github.com/SukiXuu/websetting/tree/0aadb01b81fe627c447b9ad1e936219cc6e1a8cd/courses/INFO20003/notes/可以快速检索数据%3E在急需的时候/README.md)和[\[检索数据-retrieval\]](https://github.com/SukiXuu/websetting/tree/0aadb01b81fe627c447b9ad1e936219cc6e1a8cd/courses/INFO20003/notes/可以快速检索数据%3E在急需的时候/README.md)」  


#### -&gt; Advantages \[compare with File Processing Systems\]

-=&gt; 文件处理系统的坏处:   
  
\[Data redundancy\]数据冗杂也就是数据重复,  
\[Data inconsistency\]数据不一致&gt;一般是由于数据冗杂导致的&gt;e.g.两个人身份证号一摸一样,  
\[Data Isolation\]数据分散在各种文件里格式什么的不统一&gt;难以检索,  
\[Dependency on application programs\]对于应用程序的依赖,  
\[Atomicity issues\]执行的动作难以回滚,  
\[Data security\]应该设置权限

-=&gt; DBMS 的好处:   
  
\[几乎和上面是对应的\]  
\[No redundant dat\] by \[data normalization\],  
\[Data Consistency and Integrity\],  
\[Data Security\] ,  
\[Privacy\],  
\[Easy access to data \],  
\[Easy recovery\]易于恢复 数据库系统保留数据备份,  
\[Flexible\]

-=&gt; DBMS 的缺点:   
  
\[Expensive\]贵,  
\[Complexity\]数据库系统难以理解,\[Performance\]  
DBMS的通用使其适合于各种应用程序&gt;此功能会影响其在某些应用程序中的性能

## Lecture 02 Database Development Process

#### -&gt; Outline

{\[Database Planning\] &gt;&gt; Database Definition &gt;&gt; Requirements Definition and Analysis}  
  
 =&gt; {Conceptual Design &gt;&gt; Logical Design &gt;&gt; Physical Design}  
  
 =&gt; {Application Design}  
 =&gt; {Implementation}  
 =&gt; {Testing}  
 =&gt; {Operational Maintenance}  
 =&gt; {回到第一个}  
 \[Database Planning\]:   
Planning how to do the project; how Enterprise work & Enterprise data model   
\[Database Definition\]:   
Specifying scope and boundaries to users, application areas & How does the system interfere with other organisational systems知识水平是否可以维护,包括需要哪一个软件   
\[Requirements Definition and Analysis\]:   
Collection and analysis of requirements需要对于需求进行理解和解析,看作设身处地,  


