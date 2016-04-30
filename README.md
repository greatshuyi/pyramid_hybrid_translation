# pyramid_hybrid_translation
Translation of Pyramid Zope Plone

前言

这是一本关于框架使用及其背后构建思想的翻译工作。
这是一个朋友间合作的翻译项目，完全是出于兴趣，因为我们都喜爱Python、C/C++，工作中常用Python。
翻译的内容主要是pyramid、zope 3和plone的文档或书籍。我们的目标是尽量力求翻译的准确性、逻辑性，
希望我们的翻译能够作为后续学习人员的高质量参考，也为工作中需要的同行们带来方便，也欢迎大家共同
参与。

pyramid、zope和plone实际上有着很强的内在联系，zope为plone提供了最基础的框架，plone将zope应用带到了
一个新的高度；pyramid是在总结zope得失的基础上，吸收了很多新型框架优点而成的。在本翻译中，我们将采用
“倒叙”的方式来翻译三者，即按照pyramid、zope、plone的顺序翻译。诚然一个刚接触其中之一的的陌生人会发现：
很多概念难以理解头绪不多，抛开zope和plone这一“臭名昭著”的文档匮乏不谈，即便众所周知pyramid的文档是三
者中最好的，且提供了丰富的背景概念和知识的解释，要想快速掌握其框架原理并得心应手的使用和扩展扔需要付
出大量的努力。作为“痛苦的过来人”我们愿意分享我们的工作所得，帮助“解救痛苦者”。

这一翻译过程我们预想是一个很长的过程。我们目前暂定翻译会主要分成四个阶段：第一阶段翻译pyramid，其次翻译
能够找到的zope内容并以zope 3为主，然后翻译plone的文档，最后会用我们自己的实际工作替换翻译中的某些内容（
以一个商务网站和一个企业内网的管理系统（文档、资产、项目、经济运行）最为主要内容替换译文中的原有的示例，
希望我们的工作能为同行们提供一些参考（当然不要和那些会为Java、J2EE站台的人太激烈的争辩，也不要和PHP的拥趸
们辩论，我们的主旨是分享观点）！不过整体的时间还不知道需要多久，但第一阶段大概持续45天左右，后续的内容涉及
到我们自身的一些代码和工作原因，需要的时间还很难确定，但我们的主旨是坚持下去，也为我们自身的兴趣寻找到载体。

在我们的工作中体会到，pyramid是一个灵活强大的框架，希望用户们可以在日后的使用中体会到。zope是最厚重的框架，
其中的思想也是最具开创性的，pyramid也和zope有着千丝万缕的联系。在我们看来这也为口头流传的名词design pattern的一个最好的pythonic示例。也许这一观点存在争议，但只要能对读者产生足够的启发就足够了，我们希望
能够在技术这一根本性土壤园地中，早日开出属于chinese的、具有广大影响力的、一个原创性成果的出现。Plone
则是一个非常棒的框架，在Version 5.0之前一直基于zope 2和zope CMF构建。在5.0版本中，已经可以见到它开始
抛弃zope 2，但由于厚重的历史包袱难于一下做到。但无论如何，转变已经开始，如果读者能贡献一份力量最好。
Plone的易用性、功能设计在CMS系统中独树一帜，因此这里我们也要阐述对某个观点，十分流行的观点的态度：
zope已死，plone也日渐没落——不，肉体已死，灵魂永续；同时我们也有和当前观点一致的一面：如果采用pyramid来
构建plone则是幸事一件。

zope我们主要参考三分文档和一份书籍，官方的《Zope 2 Book》、《Zope Development Guide》、《Web Component Development
with Zope 3》，此外还有很多的第三方文档、博客，使用者经验谈。pyramid的翻译内容主要参考其官方的文档，中间会
参考http://pyramidoc.lofter.com的一些翻译内容（十分感谢）。
plone主要是参考官方文档。总体上，我们希望此处的翻译
内容能为各位带来的一定的启发性。对于能够看到的读者，当我们未能完成翻译时，也许读起来还是无法构成相应的只是体系，
但一旦完成或后面在回头按照zope、pyramid、plone的顺序快速通读一边就会有很多的收获，也许那时你的头脑中就会构建
起一副完整的、图像式的知识体系。

在翻译中，我们倾向使用Word文档作为翻译的载体形式。这也与我们工作中所形成的习惯有关。一句题外话：做设计
的最深的感受是文档的编写，设计大体就等效于写文档（虽然我们的主要工作是系统设计，和硬件与系统构建相关，但感受仍是
思想和文档才是价值的最大的载体）。

谢谢大家的关注。
