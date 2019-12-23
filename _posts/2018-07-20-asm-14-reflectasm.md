---
layout: post
title:  ASM-14-reflectASM 性能更高的反射框架
date:  2018-07-20 13:43:31 +0800
categories: [Java]
tags: [java, asm, annotation, sh]
published: true
---

# reflectasm

[reflectasm](https://github.com/EsotericSoftware/reflectasm) is a very small Java library that provides high performance reflection by using code generation. 

An access class is generated to set/get fields, call methods, or create a new instance. 

The access class uses bytecode rather than Java's reflection, so it is much faster. 

It can also access primitive fields via bytecode to avoid boxing.

# 使用例子

## Maven 引入

```xml
<dependency>
    <groupId>com.esotericsoftware</groupId>
    <artifactId>reflectasm</artifactId>
    <version>1.11.9</version>
</dependency>
```

## 测试代码

### 对象定义

```java
public class UserService {

    private String name;

    public UserService() {
        this("default");
    }

    public UserService(String name) {
        this.name = name;
    }

    public void showName() {
        System.out.println("Name is: " + name);
    }

}
```

### 方法验证

```java
UserService someObject = new UserService("ryo");
MethodAccess access = MethodAccess.get(UserService.class);
access.invoke(someObject, "showName");
```

### 构造器验证

发现不支持有参构造器，这点我们可以进行提升。

```java
ConstructorAccess<UserService> access = ConstructorAccess.get(UserService.class);
UserService someObject = access.newInstance();
someObject.showName();
```

### 字段构造器

字段默认也无法反射私有变量，这也非常的麻烦。

```java
UserService someObject = new UserService();
FieldAccess access = FieldAccess.get(UserService.class);

for(int i = 0; i < access.getFieldCount(); i++) {
    System.out.println(access.get(someObject, i));
}
```

# 思考

ReflectASM 的思想非常好，通过 asm 创建一个集成类。然后所有的实现都是直接通过调用，性能是优于反射的。

## 缺点

如上面所述，功能还是过于简单。

当然，我们也可以根据这种思想，结合 asm 处理所有的字段信息。

构建一个依赖于 asm 强大的工具包。

# 拓展阅读

更多技术文章，生活趣事，尽在【老马啸西风】。

![老马啸西风](https://user-images.githubusercontent.com/18375710/71305502-3d9d0a00-2410-11ea-8cb1-da60a584785b.jpg)

# 参考文档

[https://asm.ow2.io/asm4-guide.pdf](https://asm.ow2.io/asm4-guide.pdf)

[reflectasm](https://github.com/EsotericSoftware/reflectasm)

* any list
{:toc}