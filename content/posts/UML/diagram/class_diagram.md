---
title: "Class Diagram"
date: "2022/11/16"
---



# Class Diagram

类由三部分组成：

![](/posts/UML/diagram/class_diagram/fig.png)

1. 类名

2. 属性
    ```code
    可见性 名称:类型 [ = 默认值]
    ```

    1. 可见性
       - public: +
       - private: -
       - protected: #

3. 方法
    ```code
    可见性 名称(参数列表) [: 返回类型]
    ```
    

## 类与类之间的关系

### 关联关系：Association

一个类的对象作为另一个类的成员变量

![](/posts/UML/diagram/class_diagram/association.png)

1. 双向关联

   ![](/posts/UML/diagram/class_diagram/bidir_asso.png)

2. 聚合关系：Arrgregation

   **拥有不同的生命周期**

   作为构造函数，Setter函数等的参数注

   ![](/posts/UML/diagram/class_diagram/aggregation.png)

3. 组合关系：Composition

   **相同的生命周期**

   在构造函数中初始化

   ![](/posts/UML/diagram/class_diagram/composition.png)

### 依赖关系：Dependency

某个类的方法使用另一个类的对象作为参数

![](/posts/UML/diagram/class_diagram/dependency.png)

### 泛化关系：Generalization

泛化关系就是继承关系

![](/posts/UML/diagram/class_diagram/generalization.png)

### 接口与实现关系

接口中，通常没有属性，且所有操作都是抽象的，只有声明没有实现

![](/posts/UML/diagram/class_diagram/interface.png)
