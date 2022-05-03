

# Fibonacci using Test-Driven Development



## Contents



这个repo记录Java语言下使用测试驱动开发(Test-Driven Development, TDD) 来实现4种斐波那契函数。



**任务**

Fibonacci函数的4种实现方式：

- 命令式
- 函数式
- 普通递归
- 记忆化递归。

其中，记忆化递归需要复用普通递归的代码，并且测试记忆化递归比普通递归执行速度快。



**设计要求**

好的代码质量

轻量化设计

最少的代码

自动测试

代码覆盖

持续集成

尽可能地复用代码



## What you can learn



**可学习到的技术**

测试驱动开发(TDD), 自动化测试(CT)，持续集成(CI)，敏捷开发(Agile)，使用Jacoco查看代码coverage，使用pmd进行静态代码检查等。



**可学习到的设计原则**

单一职责原则(SRP), 别重复原则(DRY), 开闭原则(OCP), 依赖倒置原则(DIP)等。



## Structure

```bash
Fibonacci/
├── src
│   └── fibonacci
│       ├── Fibonacci.java
│       ├── FibonacciFunctional.java
│       ├── FibonacciImperative.java
│       ├── FibonacciMemoizedRecursion.java
│       └── FibonacciSimpleRecursion.java
└── test
    └── fibonacci
        ├── FibonacciFunctionalTest.java
        ├── FibonacciImperativeTest.java
        ├── FibonacciMemoizedRecursionTest.java
        ├── FibonacciSimpleRecursionTest.java
        ├── FibonacciSpeedTest.java
        └── FibonacciTest.java

conf/: pmd进行静态代码检查的规则

tests.txt: 各种要进行的测试

build.gradle.kts: gradle自动构建的脚本(kotlin)
```



## Requirement

```
windows子系统wsl2: ubuntu 18
Java 8 及以上: 需要支持lambda表达式
Junit5: Unit test
gradle: 4.4.1 及以上
```



## Run

clone这个repo

```bash
https://github.com/shizhengLi/TDD_Fibonacci.git
```

运行

```bash
cd TDD_Fibonacci/TDD_Fibonacci
./gradlew
```

查看code coverage在：`/TDD_Fibonacci/build/reports/jacoco/test/html/index.html` （注：先run之后才能出现build文件夹）
