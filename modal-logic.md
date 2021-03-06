# 模态逻辑：一种当代观点

原文请参见：[Modal Logic: A Contemporary View](http://www.iep.utm.edu/modal-lo/)

模态概念超越了简单的真或假，它将我们的所言所思嵌入更大的概念空间，指称什么是可能如此或本可以如此，什么是应该如此或本应该如此，或什么是可以继续如此的。模态表达式在各种自然语言中出现的范围都十分广泛，从必然性、可能性和偶然性，到时间、行动、变化、因果、信息、知识、信念、义务、许可，以及远远超出这些概念的范围。相应的，当代模态逻辑是表达这些概念并对其进行推理的一般研究。

尽管该研究的起源在哲学，自 1970 年代以来模态逻辑同样发展了与数学、计算机科学、语言学和经济学的密切接触，而且其朋友圈还在扩大。但与此同时，自从在 1950 年代和 1960 年代发现各种翻译可以将模态语言翻译到经典逻辑系统中，模态逻辑在其技术发展方面也变得更加丰富。模态研究也变成一种对表达力、推演和计算复杂性的精细结构的研究。这些研究对经典逻辑提供新的认识，并有创造性地与之互动。

本文本着《模态逻辑手册》的精神，给出当今模态逻辑的全景图，强调它与经典逻辑共有的数学手法，列出其跨越不同学科的主题和应用：从哲学和数学到计算机科学和经济学。尽管这种风格的介绍并不否认模态逻辑的形而上学起源，我只是把它作为通向模态推理模式的诸多有效道路之一。其他在本文旅行的道路还将穿越其他领域的哲学，如知识和信念的认识论，甚至穿越其他学科，如数学中空间的逻辑，或计算机科学和博弈论中程序、行动和博弈的逻辑。

## 1. 模态概念与推理模式：预备（a First Pass）

模态逻辑单独成为一个主题，开始于二十世纪早期对哲学概念必然性和可能性的形式研究。该传统仍然活跃于哲学当中（Williamson 2013）。但本文将在更大的画布上进行描绘，向读者介绍一个世纪之后作为研究领域的模态逻辑变成了什么。不过作为开始，认识到模态概念有一个很长的历史家谱是重要的。亚里士多德早已研究过它们，然后是中世纪的逻辑学家（Kneale & Kneale 1961），他们注意到这个领域的推理有很多奇特之处。这些研究往往从原始的推断直觉开始，它们可以采取若干形式。我们可以判断有些模式是有效的（比如，必然性蕴含真），我们可以判断其他模式是无效的（真不蕴含必然性），或者我们可以找到不同模态概念之间的联系，如某个命题 $$\phi$$ 的必然性等价于非 $$\phi$$ 的不可能性。然后模态逻辑学家通过引入符号使所有这些更加清晰明了。比如，将“$$\phi$$ 是必然真的”记作 $$\Box\phi$$，将“$$\phi$$ 是可能真的”记作 $$\Diamond\phi$$，这样上述论断就分别相当于：

- $$\Box\phi\to\phi$$ 是有效的
- $$\phi\to\Box\phi$$ 是无效的
- $$\Box\phi\leftrightarrow\neg\Diamond\neg\phi$$ 是有效的。

后来，经过 C. I. Lewis（Lewis & Langford 1932）的工作，更多哲学概念被纳入这个家族，特别是衍推（entailment）这个概念，它也叫“严格蕴含”，是两个命题之间的关系。相比普通的实质蕴涵 $$\phi\to\psi$$ 表达 $$\phi$$ 和 $$\neg\psi$$ 并非一起出现这个事实，衍推是更强的模态断言，它说的是二者**不能**（cannot）一起出现：$$\neg\Diamond(\phi\land\neg\psi)$$。

有了这些符号，我们就可以进入逻辑学家的第二个专业模式：通过有效的抽象推理步骤对这些形式进行操作，以发现新的洞察。例如，几步简单的推断再加合理的模态原则会表明，$$\neg\Diamond(\phi\land\neg\psi)$$ 和 $$\Box(\phi\to\psi)$$ 是模态等价的。这就对衍推给出了一种新的观点：这次衍推是作为实质蕴涵的必然性加强。有了这样的证明演算供使用，我们就能分析许多经典和现代文献中涉及模态的哲学论证。在 Arthor Prior、Peter Geach、Jaccko Hintikka、Stig Kanger、Saul Kripke、David Lewis、Robert Stalnaker 和其他先驱者的著作中有大量著名的例子，一直到当今哲学逻辑学家形成的新浪潮。但我们也可以独立使用逻辑证明演算（一旦我们确定了一个），对由支配模态的原则组成的抽象系统进行更多的揭示。