# E-R\_Model

## E-R Model

\[TOC\]

### Entity

Definition: **实体**是数据的对象或组成部分\[单独的一个例子\] ER: 在ER图中表示为矩形

#### Weak Entity

Definition: **弱实体**是不能通过自身属性唯一标识并且依赖于与其他实体的关系的实体   
\[每个弱实体有且只有一个强实体要依赖\(关键约束\)弱实体集必须完全参与此关系集,这种关系称为识别,并表示为“粗体”\] ER: **弱实体**由矩形加粗表示 ![avator](https://github.com/SukiXuu/websetting/tree/0aadb01b81fe627c447b9ad1e936219cc6e1a8cd/courses/INFO20003/notes/ppt/截屏2020-08-16%20下午3.36.40.png) // NOTE Weak entities have only a “partial key” \(dashed underline\) and they are identified uniquely only when considering the primary key of the owner entity = weak entity\(key要用虚线\)没有足够的属性来构建主键

#### Entity Set

All entities in an entity set have the same set of attributes. "实体集中的所有实体具有相同的属性集", A collection of entities of the same type 「同一个类型的集合, 比如所有的同学」

_\[平时DB中经常叫的'Set'就是这里的‘Entity Set’\]_

### Attribute

Definition: An attribute 描述了an entity的属性\(property-单复同形\) ER: 椭圆

#### 1. Primary Key Attribute

Definition: "Primary Key",在这个Entity Set里相同的属性,每个实体都有一个key ER: arribute with 下划线

#### 2. Composite attribute

Definition: 由其他属性组合而成的属性称为复合属性 ![avatar](https://github.com/SukiXuu/websetting/tree/0aadb01b81fe627c447b9ad1e936219cc6e1a8cd/courses/INFO20003/notes/ppt/截屏2020-08-16%20下午2.40.17.png)

#### 3. Multivalued attribute

Definition: 可以包含多个值的属性称为多值属性在 ER: 双层椭圆形 e.g. 一个人可以有多个电话号码，因此电话号码属性是多值的

#### 4. Derived attribute

Definition: 派生属性是其值是动态的并且从另一个属性派生的属性 ER: 虚线椭圆 e.g. 年龄是随时间变化的派生属性，可以从另一个属性（出生日期）派生 ![avatar](https://github.com/SukiXuu/websetting/tree/0aadb01b81fe627c447b9ad1e936219cc6e1a8cd/courses/INFO20003/notes/ppt/截屏2020-08-16%20下午2.47.12.png)

### Key Constraints

Definition: 两个entity set之间在某一些限制条件下形成 ER: 菱形

#### 1. Many to Many

#### 2. One to Many / Many to One

—ER: 有箭头

#### 3. One to One

#### Participation Constraints

探索one entity set中的all entities是否都有参与relationship total participation: 都参与 \[e.g.每个员工都必须在一个部门工作\] —ER: 线条加粗 partial participation: 有的没有参与或者说并不是强制参与 —ER: 正常连线

### Relationship

#### binary

#### n-ary/ternary

