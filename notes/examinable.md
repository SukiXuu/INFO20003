# INFO20003 Database

\[TOC\]

## Week01

### L01-Introduction

  
 -&gt; Difference between Data and Information   
   
   ♺ 数据: known,available「已知的信息储备,可以直接食用」  
      信息: processed,more useful 「处理过,更有用」— 存在

-&gt; Being able to discuss the advantages of Databases vs File Processing Systems

  ♺ 文件处理系统的坏处:   
\[Data redundancy\]数据冗杂也就是数据重复,  
\[Data inconsistency\]数据不一致&gt;一般是由于数据冗杂导致的&gt;e.g.两个人身份证号一摸一样,  
\[Data Isolation\]数据分散在各种文件里格式什么的不统一&gt;难以检索,  
\[Dependency on application programs\]对于应用程序的依赖,  
\[Atomicity issues\]执行的动作难以回滚,  
\[Data security\]应该设置权限

  ♺ DBMS 的好处: \[几乎和上面是对应的\]  
\[No redundant dat\] by \[data normalization\],  
\[Data Consistency and Integrity\],  
\[Data Security\] ,  
\[Privacy\],  
\[Easy access to data \],  
\[Easy recovery\]易于恢复 数据库系统保留数据备份,  
\[Flexible\]

  ♺ DBMS 的缺点:   
\[Expensive\]贵,  
\[Complexity\]数据库系统难以理解,\[Performance\]  
DBMS的通用使其适合于各种应用程序&gt;此功能会影响其在某些应用程序中的性能

### L02-DatabaseDevelopment

-&gt; Can you discuss \[\[DBMS&lifecycle\]\] of DB?  
 -&gt; What is done at each [Stage of Design](stage-of-design.md)?

## Week02

### L03- \[\[Data Model\]\]

_\[Need to be able to draw conceptual diagrams on your own\]_

-&gt; Given a problem, determine entities, attributes, relationships  
 -&gt; What is key constraint and participation constraint, weak entity?   
 -&gt; Determine constraints for the given entities & their relationships

### L04- Relational Model

-&gt; Translate conceptual \(ER\) into logical & physical design -&gt; Understand integrity constraints -&gt; Use DDL of SQL to create tables with constraints

