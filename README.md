# FDU CS自学指南

{% hint style="info" %}
【2025/02】 复旦大学泛计算机类课程和培养方案在近年里有了不少了变化与改革，比如新设立了AI大课与人工智能双学位等，如果有在校的学弟学妹有兴趣接力维护自学指南，欢迎与我们联系。联系方法请见 `联系我们` 栏目。
{% endhint %}



指南的写作动机与背景基本可以参照《CS自学指南》和《上海交大生存手册》，笔者就不再过多赘言，直接摘录如下：

> 各位同学们，在本书的开始，我不得不遗憾地告诉大家一个消息。国内绝大部分大学的本科教学，不是濒临崩溃，而是早已崩溃。在此，我无意争论是否复旦、中科大、或者清华、北大是否比我们崩溃的更少一些——这种争论是没有意义的。我只是看到了无数充满求知欲、激情、与年轻梦想的同学们，将要把自己的四年青春，充满希望与信任地交给大学来塑造。这使我心中非常不安。
>
> 在当今流水线式的教育体制下，我们就像廉价的零件一样被生产出来。因为数量巨大，没人会对每一个人的教学质量负责。
>
> ...... \
> 学不懂？那是因为你智力低，要么就是自己底下不用功。为什么跟你一个班上的某某某同学，人家就能懂？诚然，就算是老师上课说孟加拉语，一个班上也非常有可能冒出一两个翻翻书看看图就能学到八九不离十的同学（或者根本就是以前学过）。真正在课堂上口传心授的教学，其质量是不会有人过问的。教学评估会考察实验报告格式是否合格，出勤率是否够，但是绝对不会考察上百人的班上到底有几个听懂了的。\
> ......\
> 而对于具体课程，教学大纲的陈旧程度也令人叹为观止。当然，以“教学经验”的名义，十年用同一本教科书是可以理解的。甚至我们可以容忍教学大纲里有一些广受诟病的古典残留物（例如《线性代数》中的 Cramer 法解方程）。但我们无法容忍对于一门只有几十年历史的新兴学科，我们的教科书竟然可以只涉及到上个世纪八十年代的“新技术”！这样的课程，之所以能够存在并延续下去，从根本上讲是因人设课——开设相应课程是为了不让部分教师下岗。这也无怪国外有华裔学者实在看不下去了，拍案疾呼道：“中国大学，怎么那么盛产‘活化石’！”。

来源：[《上海交大生存手册》](https://survivesjtu.gitbook.io/survivesjtumanual)



> 大一入学时我是一个对计算机一无所知的小白，装了几十个 G 的 Visual Studio 天天和 OJ 你死我活。凭着高中的数学底子我数学课学得还不错，但在专业课上对竞赛大佬只有仰望。提到编程我只会打开那笨重的 IDE，新建一个我也不知道具体是干啥的命令行项目，然后就是 `cin`, `cout`, `for` 循环，然后 CE, RE, WA 循环。当时的我就处在一种拼命想学好但不知道怎么学，课上认真听讲但题还不会做，课后做作业完全是用时间和它硬耗的痛苦状态。我至今电脑里还存着自己大一上学期计算概论大作业的源代码 —— 一个 1200 行的 C++ 文件，没有头文件、没有类、没有封装、没有 unit test、没有 Makefile、没有 Git，唯一的优点是它确实能跑，缺点是“能跑”的补集。我一度怀疑我是不是不适合学计算机，因为童年对于极客的所有想象，已经被我第一个学期的体验彻底粉碎了。
>
> 这一切的转机发生在我大一的寒假，我心血来潮想学习 Python。无意间看到知乎有人推荐了 CS61A 这门课，说是 UC Berkeley 的大一入门课程，讲的就是 Python。我永远不会忘记那一天，打开 [CS61A](https://cs61a.org/) 课程网站的那个瞬间，就像哥伦布发现了新大陆一样，我开启了新世界的大门。
>
> 我一口气 3 个星期上完了这门课，它让我第一次感觉到原来 CS 可以学得如此充实而有趣，原来这世上竟有如此精华的课程。\
> ......\
> 这样的课程，你完全不需要任何计算机的基础，你只需要努力、认真、花时间就够了。此前那种有劲没处使的感觉，那种付出再多时间却得不到回报的感觉，从此烟消云散。这太适合我了，我从此爱上了自学。
>
> 试想如果有人能把艰深的知识点嚼碎嚼烂，用生动直白的方式呈现给你，还有那么多听起来就很 fancy，种类繁多的 project 来巩固你的理论知识，你会觉得他们真的是在倾尽全力想方设法地让你完全掌握这门课，你会觉得不学好它简直是对这些课程建设者的侮辱。
>
> 如果你觉得我在夸大其词，那么不妨从 [CS61A](https://cs61a.org/) 开始，因为它是我的梦开始的地方。
>
> .....
>
> 如果大家可以在三年不到的时间里就能建立起整座CS的基础大厦，能有相对扎实的数学功底和代码能力，经历过数十个千行代码量的 Project 的洗礼，掌握至少 C/C++/Java/JS/Python/Go/Rust 等主流语言，对算法、电路、体系、网络、操统、编译、人工智能、机器学习、计算机视觉、自然语言处理、强化学习、密码学、信息论、博弈论、数值分析、统计学、分布式、数据库、图形学、Web开发、云服务、超算等等方面均有涉猎。我想，你将有足够的底气和自信选择自己感兴趣的方向，无论是就业还是科研，你都将有相当的竞争力。
>
> 因为我坚信，既然你能坚持听我 BB 到这里，你一定不缺学好 CS 的能力，你只是没有一个好的老师，给你讲一门好的课程。而我，将力图根据我三年的体验，为你挑选这样的课程。

来源：[《CS自学指南》](https://csdiy.wiki/)

相比于上述两篇作者所在的学校（PKU & SJTU），复旦大学泛计算机类专业（计算机、信安、大数据、人工智能、智科等）的教育现状对于自学的需求可谓有过之而无不及。笔者在现有自学指南的基础上进行了一些补充和调整，以期能更加适合校内实际情况。

在指南的前半部分，笔者对校内泛计算机专业的主干课程提供了一些自学建议，包括可以替代/参考的更高质量的教材和自学课程（特别推荐以及推荐完成的课程Lab标注了☆），自学建议不局限于课程修读本身，也可作为自学某一特定内容的参考。在后半部分，考虑到校内前沿了解、科研素养、就业能力培养和训练的严重缺失与脱节，笔者以目前泛计算机类就业和研究的主流领域作为划分，补充了大量可以参考的自学资源（课程、书籍、博客等），希望能为同学们未来发展提供一些指引。

本指南面向的对象不局限于泛计算机专业的同学，对于相近专业以及任何想要了解和学习相关内容的同学，希望这个指南都能提供一些参考与指导。

祝各位学有所成。

