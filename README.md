



 >    大家好，我是小兵，在现在建筑的模式下，Autodesk公司退出了参数化编程可视化软件Dynamo。我们将对他进一步的研究，但是目前这个软件差不多不是很成熟，需要大家的努力才能使变得更加完善和稳定。在这儿为了让更多的英文不是太好的人了解这款软件，根据官方网站的指导文件，将进行中文的翻译，另外里边我还会加一些我个人对这个软件的理解，此文中有不当之处还请谅解。此资料不能用作商业用途，违版必究。谢谢大家(个人收集资料用，我愿意分享出来与大家一起探讨).


![](logo副本.jpg)


#  Dynamo指导教程
## Dynamo 教程版本号是0.9.X 

![Dynamo Logo](images/dynamo_logo_dark-trim.png)

> Dynamo是一个开源的可视化参数编程设计软件。
> 
> 这套教程我会根据官网的教程会做持续的更新，保证和官方的教程一样。

### Welcome
You have just opened the Dynamo Primer, a comprehensive guide to visual programming in Autodesk Dynamo Studio. This primer is an on-going project to share the fundamentals of programming. Topics include working with computational geometry, best practices for rules-based design, cross-disciplinary programming applications, and more with the Dynamo Platform.

The power of Dynamo can be found in a wide variety of design-related activities. Dynamo enables an expanding list of readily accessible ways for you to get started:
* **Explore** visual programming for the first time
* **Connect** workflows in various software
* **Engage** an active community of users, contributors, and developers
* **Develop** an open-source platform for continued improvement

In the midst of this activity and exciting opportunity for working with Dynamo, we need a document of the same caliber, the Dynamo Primer.

Version 1.0 of this Primer includes the first ten chapters developed by Mode Lab. These chapters focus on the essentials you will need to get up and running developing your own visual programs with Dynamo and key insights on how to take Dynamo further. Here's what you can expect to learn from the primer:

* **Context** - What exactly is "Visual Programming" and what are the concepts I need to understand to dive in to Dynamo?
* **Getting Started** - How do I get Dynamo and create my first program?
* **What's in a Program** - What are the functional parts of Dynamo and how do I use them?
* **Building Blocks** - What is "Data" and what are some fundamental types I can start using in my programs?
* **Geometry for Design** - How do I work with geometric elements in Dynamo?
* **Lists, Lists, Lists** - How to do I manage and coordinate my data structures?
* **Code in Nodes** - How can I start extending Dynamo with my own code?
* **Computational BIM** - How can I use Dynamo with a Revit model?
* **Custom Nodes** - How can I create my own nodes?
* **Packages** - How can I share my tools with the community?

This is an exciting time to be learning about, working with, and developing for Dynamo. Let's get started!

---

### Open Source
The Dynamo Primer project is open source! We're dedicated to providing quality content and appreciate any feedback you may have. If you would like to report an issue on anything at all, please post them on our git hub issue page: https://github.com/DynamoDS/DynamoPrimer/issues

If you would like to contribute a new section, edits, or anything else to this project, check out the github repo to get started: https://github.com/DynamoDS/DynamoPrimer.

---
### The Dynamo Primer Project
The Dynamo Primer is an open source project, initiated by Matt Jezyk and the Dynamo Development team at Autodesk.

**Mode Lab** was commissioned to write the First Edition of the primer. The team continues to work with Autodesk to provide updates in parallel with Dynamo's development.

[<img src="images/MODELAB_Logo.png">](http://modelab.is)

### Acknowledgments

A special thanks to Ian Keough for initiating and guiding the Dynamo project.

Thank you to Matt Jezyk, Ian Keough, Zach Kron, and Colin McCrone for enthusiastic collaboration and the opportunity to participate on a wide array of Dynamo projects.

### Software and Resources
**Dynamo** The current stable release of Dynamo is Version 0.9.

http://dynamobim.com/download/

**DynamoBIM** The best source for additional information, learning content, and forums is the DynamoBIM website.

http://dynamobim.org

**Dynamo GitHub** Dynamo is an open-source development project on Github. To contribute, check out DynamoDS.

https://github.com/DynamoDS/Dynamo

**Contact** Let us know about any issues with this document.

Dynamo@autodesk.com

### License
Copyright 2015 Autodesk

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.



#【Dyanamo 中文手册..】

![Dynamo Logo](images/dynamo_logo_dark-trim.png)

> Dynamo是一个开源的可视化参数编程设计软件。

### Welcome

你将打开的是dynamo教学手册第一版本。
一个编程指南由Autodesk Dynamo 指南
这篇文章是分享dynamo运作的基本原理。主要包括处理几何、规则图形的参数化,跨学科的编程应用程序,和更多的Dynamo平台。


Dynamo可以设计各种相关的行为。Dynamo可以不断扩大,有以下的方法：


* **探  索**   可视化编程的第一次
* **连  接** 工作流程里边的各种数据链接
* **社 区** 一个活跃的使用者、编著者和开发人员
* **开发** 一个开源平台持续改进

在这个过程中，实用Dynamo都会令人兴奋，我们需要一个文档[Dynamo 中文手册]


这个版本是在之前开发dynamo语言手册基础之上的的Dynamoprimer。这些章节重点是需要自己去学习的.这也是这本书的价值所在.


* **视觉编程** -“视觉编程”是什么概念我需要了解Dynamo吗?
* **入门指南** -我怎么得到Dynamo并创建我的第一个程序
* **这是什么程序** - 什么是Dynamo的节点件和如何使用它.
*  **搭建数据**什么是“数据”,有哪些基本类型可以使用
* **几何设计** - 怎么在工作中了解dynamo几何的基本原理.
*  **数列，数据列表** - 我怎么去做控制和管理我的数据结构.
* **节点代码** - 我怎么在Dynamo中扩展自己的代码.
* **BIM计算** -我如何在revit模型中使用Dynamo.
* **自定义节点** -我如何创建自己的节点?
* **程序包** -我怎么能与社区分享我的自定义节点?


一个激动人心的时学习刻即将来了,让我们一起开始Dynamo的学习吧！

---
###  dynamo指导项目


dynamo是个开源项目,由马特Jezyk和Autodesk的Dynamo的开发团队共开发.


* **实验室模式**  委托编写的第一版指导教材。http://modelab.is

![Mode Lab Logo](images/MODELAB_Logo.png)

### 特别感谢


特别感谢伊恩Keough启动和指导Dynamo项目.



感谢马特•Jezyk伊恩Keough扎克克隆亚麻,科林McCrone热情合作参与各种Dynamo各种研发.

### 软件和资源

参数化Dynamo当前稳定版本是0.9.0版。


http://dynamobim.com/download/

这个Dynamo的官方网站，这个网站必须要翻墙才能上去，下载软件也必须要翻墙出去，到时候我会下载下来，通过百度云盘的方式放在这上边，已提供给大家下载及学习.

DynamoBIM附加信息的最佳来源,学习内容,DynamoBIM网站和论坛。

http://dynamobim.org

Dynamo在GitHub GitHub Dynamo是一个开源开发项目。提供是DynamoDS伊恩Keough主持.

https://github.com/ikeough/Dynamo

dynamo在github中文翻译的提供地址为 https://github.comxiebinhqyh/dynamochina

这一部分正在翻译中，里边如有翻译不正确希望指出，大家一起来完善.

### 许可
  版权2015欧特克


在Apache许可下的2.0版本(“许可证”);你可能不使用这个文件符合许可除外。你可能会获得一份许可证

http://www.apache.org/licenses/LICENSE-2.0


除非适用法律要求或书面同意,在许可证下发布的软件是分布在一个“是”的基础上,没有任何形式的保证或条件,无论是明示或默示。看到许可下的特定语言管理权限和限制许可证。

谢谢！ Deattor 2015


