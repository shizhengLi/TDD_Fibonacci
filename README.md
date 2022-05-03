

# Fibonacci using Test-Driven Development



## Contents



这个repo记录Fibonacci函数的4种实现方式：命令式，函数式，普通递归，记忆化递归。其中，记忆化递归需要复用普通递归的代码，并且测试记忆化递归比普通递归执行速度快。



设计要求：好的代码质量，轻量化设计，最少的代码，自动测试，代码覆盖，持续集成，尽可能地复用代码。



编程语言：Java 和 Junit5单元测试



使用技术：测试驱动开发(TDD), 自动化测试(CT)，持续集成(CI)，敏捷开发(Agile)，使用Jacoco查看代码coverage，使用pmd进行静态代码检查等。



使用的设计原则：单一职责原则(SRP), 别重复原则(DRY), 开闭原则(OCP), 依赖倒置原则(DIP)等。



## Requirement

```
windows子系统wsl2: ubuntu 18
Java 8 及以上: 需要支持lambda表达式
Junit5: Unit test
gradle: 4.4.1 及以上
```



## Run



```
cd TDD_Fibonacci
./gradlew
```

查看code coverage在：`/TDD_Fibonacci/build/reports/jacoco/test/html/index.html` （先run之后才能查看）
