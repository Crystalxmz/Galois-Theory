# Galois-Theory
本讲义是对于伽罗瓦理论的一个简要概括.

伽罗瓦理论是由法国数学家埃瓦里斯特·伽罗瓦(Évariste Galois)在19世纪创立的理论.其所有内容都包含在\cite{Galois}中,而该论文的艰涩难懂导致其险些被历史所湮没,伽罗瓦在此论文中使用置换群来描述给定的多项式的根与系数间的关系.其之后由戴德金(Julius Wilhelm Richard Dedekind),利奥波德·克罗内克(Leopold Kronecker),埃米尔·阿廷(Emil Artin)在此论文的基础上用现代语言改进并完善了伽罗瓦理论,形成了我们现在看到的形式,即伽罗瓦对应\ref{thm:finite-Galois-corr}.所以本讲义所介绍的即为现代伽罗瓦理论,而删繁就简,省去了许多历史渊源.对于此,可参考\cite{Artin}\cite{YH}.

本讲义例子较为稀少,少部分记号和定义未给出详细说明,多数定理未给出(严格)证明,其中人名定理都已标注,请自行参考文献和互联网资源.

除参考文献外,本讲义主要参考维基百科,采用的记号和翻译也以主流为准,同时在有歧义时给出注解.多数记号命名思路可参考索引中的中英对照,同时记号尽简洁而避繁杂,便于记忆,采取全文通用的形式,非首次出现则不再解释.

同时本讲义具备了目录,索引,参考文献,网址超链接,可谓麻雀虽小五脏俱全.对于文中的交叉引用也附有超链接,但考虑到线性阅读的流畅性,尽量减少交叉引用的使用,而是通过调整结构顺序来避免这一麻烦.

附录A为语音学相关知识,和伽罗瓦理论无关,仅供感兴趣的读者阅读.由于本人对法语一窍不通,如有纰漏,敬请指正.

考虑到\TeX 对多语言的支持较为困难(如希伯来语),且表格绘制过于繁琐,附录B是由PowerPoint制作,作为PDF文件添加到\TeX 中的.这里简单用到了\texttt{pdfpages}宏包,意外地好用,整体风格上也不显得过于突兀.

本讲义是对\LaTeX 编译的一次尝试,很多功能和宏包是第一次使用.感谢李文威老师提供的\cite{LW}之\TeX 源码(见 https://gitee.com/wen-wei-li ),这对编写一份不算厚的讲义来说省去了大量的工夫.但也正因如此,存在着不少小问题.同时,李文威老师的写作功底也十分扎实,语言流畅自然,我非常推荐在写作前阅读李文威老师主页(见 https://wwli.asia )上的数学写作漫谈.

在编译本讲义的过程中我也学习到很多有趣的技巧,诸如超链接和索引是我认为编写现代阅读物不可或缺的功能,而这主要依赖于\texttt{hyperref}和\texttt{makeidx}宏包.这也是为何在体量不大的情形下仍旧使用目录和索引.

同时在编译过程中依旧遇到许多问题,有诸如宏包导入顺序出错而导致的功能残缺,和一些在其他文档中能正常编译却在本文档中出错的怪异现象.但是大部分问题都可通过多次尝试编译和网络和纸质文献的搜寻来解决,而对于尝试许久仍无法解决的问题,我想另辟蹊径不失为一个正确的选择.在讲义编写完成之际,我会将所有源码上传至GitHub,作为参考和备份.

版本的更新说明:

v3.14:20220227 继续增加了目录长度;修改了4.1节并扩充至4.2节;改正了第四章导言中的笔误,并扩写了导言;添加了附录B;增加了前言;增加了可迁的定义;增加了参考文献.

v3.1:20220225 增加了目录长度;由于体量的增大,改按section编号;增加了Hilbert基定理;将正文中``伽罗瓦''一律改为拉丁字母,以保持人名标记的一致性;增加了法语末尾辅音的发音说明;索引字号重新变大.

v2.718:20220214 更换了章节顺序和部分章节名称; $\tt{linkcolor}$参数值变为$\tt{purple}$;完成了第二章并对伽罗瓦扩张重新定义;前言有所改动;增加章节结构图;附录A.3中增加格罗滕迪克;索引字号变小;增加了部分参考文献;部分章节增加引言;另有部分小改动.

v2.71:20220130 较上一版本改进了附录B.2和B.3,有大幅删改;增加了附录B.4和第一章的内容,其中1.3未竟;增加了两本参考文献;删去了第零章各节的尾言;增加了裴蜀定理; Creative Commons标识改为中文;增加了前言;另有部分小改动.

有对本讲义内容或\TeX 源码有疑问的可以私信我,我的微信ID: $\tt{Ihaku5}$.
