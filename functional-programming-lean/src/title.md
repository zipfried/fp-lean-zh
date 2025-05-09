<!--
# Functional Programming in Lean
-->

# Lean 函数式编程

*作者: David Thrane Christiansen*

*版权所有: Microsoft Corporation 2023 与 Lean FRO, LLC 2023-2025*



<!--
This is a free book on using Lean as a programming language. All code samples are tested with Lean release `{{#lean_version}}`.
-->

本书的主题是使用 Lean 进行函数式编程. 所有代码已在 Lean `{{#lean_version}}` 中进行测试.

## 发布历史

### April, 2025

<!--
The book has been extensively updated and now describes Lean version 4.18.
-->

本书已全面更新, 现基于 Lean `4.18` 版本编写.

### January, 2024

<!--
This is a minor bugfix release that fixes a regression in an example program.
-->

本次次要版本更新修复了示例程序中的回退问题.

### October, 2023

<!--
In this first maintenance release, a number of smaller issues were fixed and the text was brought up to date with the latest release of Lean.
-->

作为首个维护版本, 本次更新修复了若干细节问题, 并使内容与 Lean 最新版本保持同步.

### May, 2023

<!--
The book is now complete! Compared to the April pre-release, many small details have been improved and minor mistakes have been fixed.
-->

全书正式完成!
相较于 4 月的预发布版, 优化了大量细节并修正了细微错误.

### April, 2023

<!--
This release adds an interlude on writing proofs with tactics as well as a final chapter that combines discussion of performance and cost models with proofs of termination and program equivalence.
This is the last release prior to the final release.
-->

本次更新新增了关于策略式证明的插叙章节, 还增加了结合性能和成本模型, 停机证明与程序等价证明的终章.
这是最终版本前的最后一次更新.

### March, 2023

<!--
This release adds a chapter on programming with dependent types and indexed families.
-->

新增关于依赖类型与索引族编程的章节.

### January, 2023

<!--
This release adds a chapter on monad transformers that includes a description of the imperative features that are available in `do`-notation.
-->

新增单子变换器章节, 涵盖 `do` 记法中的命令式特性.

### December, 2022

<!--
This release adds a chapter on applicative functors that additionally describes structures and type classes in more detail.
This is accompanied with improvements to the description of monads.
The December 2022 release was delayed until January 2023 due to winter holidays.
-->

新增应用函子章节, 深入解析结构体与类型类.
优化了单子相关内容的阐述.
本次更新的发布因冬季假期而延期.

### November, 2022

<!--
This release adds a chapter on programming with monads. Additionally, the example of using JSON in the coercions section has been updated to include the complete code.
-->

新增单子编程章节, 并将类型转换章节中的 JSON 示例更新为完整代码.

### October, 2022

<!--
This release completes the chapter on type classes. In addition, a short interlude introducing propositions, proofs, and tactics has been added just before the chapter on type classes, because a small amount of familiarity with the concepts helps to understand some of the standard library type classes.
-->

完成类型类章节, 在该章节前介绍了命题, 证明与 tactics, 对它们的简单了解有助于理解标准库中的部分类型类.

### September, 2022

<!--
This release adds the first half of a chapter on type classes, which are Lean's mechanism for overloading operators and an important means of organizing code and structuring libraries. Additionally, the second chapter has been updated to account for changes in Lean's stream API.
-->

发布类型类章节的前半部分, 类型类是 Lean 运算符重载 与代码组织机制的核心.
更新了第二章, 以适配 Lean Stream API 的变更.

### August, 2022

<!--
This third public release adds a second chapter, which describes compiling and running programs along with Lean's model for side effects.
-->

第三次公开更新, 新增第二章, 描述了编译运行机制和 Lean 的副作用模型.

### July, 2022

<!--
The second public release completes the first chapter.
-->

第二次公开更新, 完成了第一章的全部内容.

### June, 2022

<!--
This was the first public release, consisting of an introduction and part of the first chapter.
-->

首次公开更新, 包含引言及第一章的部分内容.

## 关于作者

<!--
David Thrane Christiansen has been using functional languages for twenty years, and dependent types for ten.
Together with Daniel P. Friedman, he wrote [_The Little Typer_](https://thelittletyper.com/), an introduction to the key ideas of dependent type theory.
He has a Ph.D. from the IT University of Copenhagen.
During his studies, he was a major contributor to the first version of the Idris language.
Since leaving academia, he has worked as a software developer at Galois in Portland, Oregon and Deon Digital in Copenhagen, Denmark, and he was the Executive Director of the Haskell Foundation.
At the time of writing, he is employed at the [Lean Focused Research Organization](https://lean-fro.org) working full-time on Lean.
-->

David Thrane Christiansen 拥有二十年函数式语言与十年依值类型论的研究经验.
他曾与 Daniel P. Friedman 合著依值类型论入门经典《[The Little Typer](https://thelittletyper.com/)》.
他于哥本哈根 IT 获得大学博士学位, 在求学期间作为核心开发者为首版 Idris 语言做出了贡献.
离开学术界后, 他先后任职于俄勒冈州的 Galois 软件公司, 哥本哈根的 Deon Digital 公司, 并担任 Haskell 基金会执行董事.
David Thrane Christiansen 在撰写本文时全职供职于 [Lean Focused Research Organization](https://lean-fro.org), 从事 Lean 语言的研发工作.

## 授权许可

<!--
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
-->

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />本作品采用<a rel="license" href="http://creativecommons.org/licenses/by/4.0/">知识共享-署名 4.0 协议国际版</a>授权.

<!--
The original version of the book was written by David Thrane Christiansen on contract to Microsoft Corporation, who generously released it under a Creative Commons Attribution 4.0 International License.
The current version has been modified by the author from the original version to account for changes in newer versions of Lean.
A detailed account of the changes can be found in the book's [source code repository](https://github.com/leanprover/fp-lean/).
-->

本书原始版本由 David Thrane Christiansen 受微软公司委托撰写, 微软公司以知识共享-署名 4.0 协议国际版慷慨发布.
当前版本已由作者根据 Lean 新版本特性对原始内容进行修订, 具体变更内容详见本书[源代码仓库](https://github.com/leanprover/fp-lean/).
