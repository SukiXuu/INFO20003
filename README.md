# INFO20003 Database Systems

\[toc\]

## Overview

#### Intended learning outcomes

Demonstrate proficiency in solving practical data-modelling tasks Use SQL to interact with a relational database Understand the internal mechanisms and policies behind database systems Understand the need for database transactions, and use them Profile and tune business analytics queries, and administer database systems. Through the combination of lectures, workshops and assignments, students will gain considerable hands-on experience in: 1ºmodelling a number of diverse informational situations, useful to both organisations and individuals, 2º writing efficient SQL queries to analyse data

## Assignments 🧨

[Quizzes](https://github.com/SukiXuu/websetting/tree/0aadb01b81fe627c447b9ad1e936219cc6e1a8cd/courses/INFO20003/Ass/quiz.md)10% & [Ass](https://github.com/SukiXuu/websetting/tree/0aadb01b81fe627c447b9ad1e936219cc6e1a8cd/courses/INFO20003/Ass/proj.md) & [Final](https://github.com/SukiXuu/websetting/tree/0aadb01b81fe627c447b9ad1e936219cc6e1a8cd/courses/INFO20003/Ass/final.md)60%

| Week | Lecture 1 | Lecture 2 | Readings \(optional\) | Tutorial | Lab | Assessments |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| W01 3-Aug | 1. Introduction to the Subject and Database Systems | 2. The Database Development Process | Chapter 1, Ramakrishnan and Gehrke, Database Management Systems | MySQL Overview/Installation | / | / |
| W02 10-Aug | 3. Introduction to ER Modelling | 4. Relational Model | Chapters 2 and 3,  Ramakrishnan and Gehrke | Tutorial: Introduction to Database Development | Lab: ER modelling with MySQL Workbench | / |
| W03 17-Aug | 5. ER Example with MySQL Workbench | 6. Hands-on Modelling | / | Tutorial: Conceptual and Logical Modelling \(ER\) | Lab: ER modelling with MySQL Workbench continued | 🧨 [A01](https://github.com/SukiXuu/websetting/tree/0aadb01b81fe627c447b9ad1e936219cc6e1a8cd/courses/INFO20003/Ass/proj.md) ER post |
| W04 24-Aug | 7. Relational Algebra | 8. SQL | Chapters 4 and 5,  Ramakrishnan and Gehrke | Tutorial: ER modelling case study | Lab: ER modelling case study | / |
| W05 31-Aug | 9. SQL Summary | 10. Storage and Indexing | Chapter 8,  Ramakrishnan and Gehrke | Tutorial: Relational Algebra and translation to SQL | Lab: SQL Skills | 🧨 [A01](https://github.com/SukiXuu/websetting/tree/0aadb01b81fe627c447b9ad1e936219cc6e1a8cd/courses/INFO20003/Ass/proj.md) ER DUE Friday |
| W06 7-Sept | 11. Query Processing-Part 1 \(Selection & Projection\) | 12. Query Processing-Part 2 \(Joins\) | Chapters 12 and 14,  Ramakrishnan and Gehrke | Tutorial: Indexing and Storage | Lab: More SQL Skills | 🧨 A02 SQL post |
| W07 14-Sept | 13. Query Optimization-Part 1 | 14. Query Optimization-Part 2 | Chapters 12 and 15,  Ramakrishnan and Gehrke | Tutorial: Query Processing | Lab: Even More SQL Skills | / |
| W08 21-Sept | 15. Normalization | 16. Normalization \(hands-on\) | / | Tutorial: Query Optimization | Lab: Query Optimization using Execution Plan | 🧨 A02 SQL  DUE Friday |
| W09 28-Sept | 17.  Transactions | 18. Database Administration | Chapters 16 and 17,  Ramakrishnan and Gehrke | Tutorial: Normalization | Tutorial: Normalization | / |
| Mid Semester Break |  |  |  |  |  |  |
| W10 12-Oct | 19. Data Warehousing | 20. Distributed Databases | / | Tutorial: Database Administration and Transactions | Lab: Transaction exercise using MySQL Workbench | / |
| W11 19-Oct | 21. Introduction to NoSQL | 22. Adaptive databases for the future \(nonexaminable: introducing database research avenues\) | / | Tutorial: Data Warehousing | Lab:  Database Admin: Backup and Recovery | 🧨 A03 QP/QO Quiz |
| W12 26-Oct | 23. Review 1 | 24. Wrap up and Review 2 | / | Tutorial: NoSQL | Tutorial: Exam FAQs | / |

## Course Question list

### Week\_01

**L01-Introduction**

  
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

**L02-DatabaseDevelopment**

-&gt; Can you discuss \[\[DBMS&lifecycle\]\] of DB?  
 -&gt; What is done at each [Stage of Design](https://github.com/SukiXuu/websetting/tree/0aadb01b81fe627c447b9ad1e936219cc6e1a8cd/courses/INFO20003/Stage%20of%20Design.md)?

### Week\_02

**L03- \[\[Data Model\]\]**

_\[Need to be able to draw conceptual diagrams on your own\]_

-&gt; Given a problem, determine entities, attributes, relationships  
 -&gt; What is key constraint and participation constraint, weak entity?   
 -&gt; Determine constraints for the given entities & their relationships

**L04- Relational Model**

-&gt; Translate conceptual \(ER\) into logical & physical design -&gt; Understand integrity constraints -&gt; Use DDL of SQL to create tables with constraints

### Week\_03

**L05**

**L06**

## Reference && More Details

