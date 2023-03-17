---
title: "单例模式：Singleton Pattern"
date: "2022-11-16"
---

# 单例模式

1. 类只有唯一实例
2. 自行创建这个实例

```java
class TaskManager {
  private static TaskManager tm = null;
  private TaskManager() {...}
  public static TaskManager getInstance() {
    if (tm == null) {
      tm = new TaskManager();
    }
    return tm;
  }
}
```

