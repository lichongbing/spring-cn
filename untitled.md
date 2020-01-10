# 概述
**Spring 使创建 Java 企业应用程序变得更加容易。它提供了在企业环境中接受 Java 语言所需的一切,，并支持 Groovy 和 Kotlin 作为 JVM 上的替代语言，并可根据应用程序的需要灵活地创建多种体系结构。
从 Spring Framework 5.0 开始，Spring 需要 JDK 8(Java SE 8+)，并且已经为 JDK 9 提供了现成的支持。**

Spring支持各种应用场景， 在大型企业中, 应用程序通常需要运行很长时间，而且必须运行在 jdk 和应用服务器上，这种场景开发人员无法控制其升级周期。 其他可能作为一个单独的jar嵌入到服务器去运行，也有可能在云环境中。还有一些可能是不需要服务器的独立应用程序(如批处理或集成的工作任务)。

Spring 是开源的。它拥有一个庞大而且活跃的社区，提供不同范围的，真实用户的持续反馈。这也帮助Spring不断地改进,不断发展。

<a id="overview-spring"></a>

## 1、"Spring"是什么？

Spring在不同的背景下有这不同的含义。它可以指 Spring Framework项目本身，这也是创建他的初衷。随着时间的推移，其他的"Spring" 项目已经构建在Spring框架之上。大多数时候，当人们说 "Spring"，他们指的是整个项目家族。本参考文档主要侧重于Spring的基本：也就是Spring框架本身。

整个Spring框架被分成多个模块，应用程序可以选择需要的部分。core是核心容器的模块，包括模块配置和依赖注入机制 。Spring框架还为不同的应用程序体系结构提供了基础支持，包括消息传递，事务数据和持久化以及Web，还包括基于Servlet的Spring MVC Web框架 ，以及Spring WebFlux响应式Web框架。

关于模块的说明: Spring Framework 的jar包允许部署到JDK 9的模块路径("Jigsaw")。为了在支持Jigsaw的应用程序中使用， Spring Framework  5的jar带有 "Automatic-Module-Name" 清单条目，它定义了稳定的语言级模块名称(例如"spring.code","spring.context"等)独立于jar部件名称(jar遵循相同的命名模式使用"-"号代替"."， 例如"spring-core" 和 "spring-context")。当然，Spring Framework 的jar包在JDK 8和9的类路径上都能保持正常工作。

<a id="overview-history"></a>

## 2、Spring和Spring框架的历史

Spring 的初版发布在2003年，是为了克服早期 J2EE 规范的复杂性。虽然有些人认为 [J2EE](https://en.wikipedia.org/wiki/Java_Platform,_Enterprise_Edition) 和 Spring 是竞争的，但是Spring 实际上是对 Java EE 的补充。Spring编程模型不受 Java EE 的平台制约，相反 它与精心挑选的个别规范的java EE项 目结合：

- Servlet API ([JSR 340](https://jcp.org/en/jsr/detail?id=340))

- WebSocket API ([JSR 356](https://www.jcp.org/en/jsr/detail?id=356))

- Concurrency Utilities ([JSR 236](https://www.jcp.org/en/jsr/detail?id=236))
