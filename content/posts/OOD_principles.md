---
title: "Object Oriented Design Principles"
date: "2022-11-16"
---

# 面向对象设计原则

1. 单一职责原则：Single Responsibility Principle, SRP

   一个类只负责一个功能领域中的相应职责。或者可以定义为：就一个类而言，应该只有一个引起它变化的原因。

2. 开闭原则：Open-Closed Principle, OCP

   > 开闭原则是面向对象的可复用设计的第一块基石，它是最重要的面向对象设计原则

   一个软件实体应当对扩展开放，对修改关闭。即软件实体应尽量再不修改原有代码的情况下进行扩展。

3. 里氏代换原则：Liskov Substitution Principle, LSP

   所有引用父类的地方必须能透明的使用其子类的对象。

4. 依赖倒转原则：Dependence Inversion Principle, DIP

   抽象不应该依赖于细节，细节应当依赖于抽象。换言之，要针对接口编程，而不是针对实现编程。

5. 接口隔离原则：Interface Segregation Principle, ISP

   使用多个专门的接口，而不使用单一的总接口，即客户端不应该依赖那些它不需要的接口。

6. 合成复用原则：Composite Reuse Principle, CRP

   尽量使用对象组合，而不是继承来达到复用的目的。

7. 迪米特法则：Law of Demeter, LOD

   一个软件实体应该尽可能少地与其他实体发生相互作用。