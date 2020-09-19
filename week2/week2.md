# Week2

## WEEK 02

 \[TOC\] \#\# Topic1: Introduction to ER Modelling \#\#\# Basic ER Modelling concepts \[wiki\]\(https://en.wikipedia.org/wiki/Entity–relationship\_model "Entity–relationship model 实体关系模型"\) 1. Entities and relationships to 企业 &gt;理解运用即可, 不需要记住定义 \*\*Entity\*\*: Real-world object distinguishable from other objects, using a set of attributes in DB.  
 "\*\*实体\*\*: 可与其他对象区分开的真实对象. 使用一组属性来描述实体\(in DB\)" \*\*Entity Set\*\*: A collection of entities of the same type "同一个类型的集合, 比如所有的同学" - All entities in an entity set have the same set of attributes. "实体集中的所有实体具有\*\*相同的属性集\*\*" - Each entity has a key \(underlined\). "每个实体都有一个键\(带下划线\) 这个意义在于identify\(key\)ER Modeling里面要用下划线表示" 在图片里, 从'Employee'连出去的每一根单独的线都表示一个attribute"属性", 其中在这个Entity Set里相同的属性叫做\*\*'KEY'\*\*, 就是每一个Entity里那个含有下划线的arribute

```text
 HInt: 平时DB中经常叫的'**Set**'就是这里的‘**Entity Set**’
```

  
 2. 这两点有关的信息有哪些**应该**被储存在database里   
  
 3. 数据库完整性约束"Integrity Constraints"有一些什么

## Topic2: Relational Model

### Relational Model -- relation & tablke

> Data Model -- 可以把信息以一种形式储存在电脑里的模型 例: **Relational**, ER, O-O, Network, Hierarchical, etc.
>
> **Relational Model**这个课程学的 Rows & Columns\(Tuples/records & /Attributes/fields\) -- _Primary Keys_ & _Foreign Keys_ to link Relations -- Foreign Keys: 指向另外一个表格

**Relational database**: a set of Relations _\[Relation: 这种关系由两个部分组成\]_

* **Schema**: specifies name of _relation_, plus name and type of each column \(attribute\).

  // e.g. Students\(sid: string, name: string, login: string, age: integer, gpa: real\)

* **Instance**: a _table_, with rows and columns.

  -&gt; rows = cardinality -&gt; fields = degree \(or arity\) -&gt; Example: [\[Instance of Students Relation\]](week2.md) \[如果说有**完全相同**的两row, 就不能说成是relation\]

**ER to Relational Model**:     \[\[Logical Design\]\]

* In **logical design** entity set becomes a relation. 
* Attributes become attributes of the relation .

  ⚠️[\[The Entire Cycle\]](week2.md)

1. _Conceptual Design_
2. _Logical Design_
3. _Physical Design_
4. Implementation -- 用SQL制表
5. Create Instance -- 内部联系

   \(@\_@\)

   > Example: Creating the Students relation.
   >
   > > CREATE TABLE Students \(sidCHAR\(20\), name CHAR\(20\), login CHAR\(10\), age INTEGER, gpaFLOAT\) \[SQL制作表格的例子, 可以看见中间都是用逗号链接\]

### Keys & Integrity Constraints

_\[内在的联系, 也可以看作是整个database的核心comment（interconnections\)\]_ _\[Keys are a way to associate tuples in different relations, 同时是 \[\[integrity constraint\]\] \(IC\) 的一种\]_

**Key**: 可以直接代表这个table里面的所有和这个relation有关的records _\[e.g.student\_id,email\_addrss\]_ _\[不一定是一个column,可以由多个columns组成\]_ **Primary Keys**: every record 都一定是unique的 _\[仍然可以是多个组成\]_ **Candidate keys**: 表示的是除了\[primary key\]之外的所有keys //NOTE **Super Keys**: \[No Subset 的 Keys\]

**Foriengn key**: _\[这个就看作是另一个表里的conlumns和其他表的index可以在用一定义下/有联系\]_ \[如果所有的Foriengn keys都有连接,就算是 \[\[Achieved referential integrity\]\] - 参照的完整性\] \(@\_@\)

> e.g. 只有在Primary Key表有的rows/records才可以:在SQL的表达
>
> > CREATE TABLE Enrolled \(sid CHAR\(20\), cid CHAR\(20\), grade CHAR\(2\), PRIMARY KEY \(sid,cid\), FOREIGN KEY \(sid\) REFERENCES Students **Enforcing Referential Integrity**: 表示的是如果要删除records需要满足的限制条件

**Integrity Constraints \(ICs\)** -- 限制条件/表格格式\(e.g. 字数\)

  IC: condition that must be true for any instance of the database;

* ICs are specified when schema is defined. 「表格建立的时候定义格式」
* ICs are checked when relations are modified. 「在建立关系的时候就要考虑这个限制条件」

   **A legal instance**: a instance/tabke of a relation satisfies all specified ICs. 「在关系中满足所有限制条件的表格-&gt;合法的表格」

* DBMS should not allow illegal instances. 「想要把instance放进DBMS必须满足所有的ICs」

### **Translating** ER to Logical and Physical Model

{Recall: Logical Design   -&gt; In **logical design** entity set becomes a relation.   -&gt; Attributes become attributes of the relation .} **Multi-valued attributes in logical design**

**Composite attributes in logical design**

**ER to Logical Design: Many to Many**

**Logical to Physical Design**

**Implementation \(Create table\)**

**ER to Logical Design: Ternary relationship**

**ER to Logical to Implementation: Ternary relationship**

{Recall: Key Constraints in ER} **Logical design: Key Constraints**

**Key Constraints in SQL** **Logical Design: Key Constraints Rule**

{Recall: Participation Constraints} Participation Constraints in SQL

{Rexall: Weak Entities} Translating Weak Entities

Relational Model: Summary •A tabular representation of data. •Simple and intuitive, currently the most widely used. •Integrity constraints can be specified based on application semantics. DBMS checks for violations.  
–Two important ICs: primary and foreign keys –In addition, we alwayshave domain constraints. •Rules to translate ER to logical design \(relational model\)

\[\[Examinable\]\] -&gt; Translate conceptual \(ER\) into logical & physical design -&gt; Understand integrity constraints -&gt; Use DDL of SQL to create tables with constraints

## Tutorial Week02

\[toc\]

Difference between conceptional design and logical design

CD: 关联性的处理 ---ER Modelling

​

LD: 我们选择 DB system --- type of application 的选择

​

Physical design: SQL / "notation chose"

Easy to go 所以分开更好 如果你的 entity 不能 interrupt others 那你很有可能就错了

帮助generate

buss 是一种Relastion &gt; 没有什么用

