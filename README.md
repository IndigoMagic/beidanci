# beidanci

    背单词神器，可以在命令行里背单词，伪装成工作：），内涵考研词汇本这个
    脚本是本人在考MBA期间为了快速熟悉单词而开发的。希望能够给其他人带来帮助，所以在github上分享

# 功能特点
   
    程序是使用js开发，在nodejs命令行中可以执行。
    
    原理是载入词库文本，进行解析，分析出词库中的单词和解释，分析原理是，如果遇到一行中顶格书写的词汇即认为是单词
    
    如果是后面用空格分割的内容则认为是描述，支持换行，换行的内容如果前面有空格或者制表符，则不会解析成单词，而解析成内容
    
    学习英语过程中最终要的一个环节是背单词，而背单词过程中质量的好坏很重要的因素就是是否专注，逐个背诵出词考意，
    是提高专注度的很号的方法。
    
    另外一个方法就是重复率，考验过程中有幸结识北京有名的英语名师指导，在此感谢太奇的邵宁，马洁等诸多恩师。
    他们经常提醒我们背单词最重要的就是你和它的见面次数，
    
    次数多了，自然就记住了。所以该软件的特点也是如此，核心思想是把词库先自如到内存中。你把会的单词扔掉，
    那么逐渐内存中的不认识的词汇越来越少。见面频率也越来越高
    
    等什么时候，使用者把所有词汇都熟悉了，词库清空，则会对词库中的单词有一个深层次的记忆。
    
    另外还有一个特点是词库就是一个文本文件，很容易编写和切割，可以根据使用者的需求，自己编写词库，也可以决定词库的大小，
    这样一开始背起来也不会干到压力那么大，利用这个特点也可以自己编写其他要背诵的东西，不一定非得是单词。

# 使用方法
    
    本程序需要先了解一下mac window linux下命令行使用的基础知识，然后安装nodejs，具体安装方法这里不再描述。
    1.首先进入项目目录，然后执行

> node beidanci.js hexin.txt

    这样就启动了背单词脚本，界面如下：
![Alt text](https://github.com/sioomy/beidanci/blob/master/resouce/01.png?raw=true)

    运行程序后，前两行提示解析单词的完成状态，然后是使用方法。
    然后下面是词库中单词数量。
    最后一行是绿色部分是考你的单词，右下角显示内存中单词剩余以及百分比。
    1) 如果用户已经认识这，想把它从内存中扔掉，就可以先输入一个'（即单引号）然后回车，这个时候单词就会从内存中删除。接下来就不会考你这个单词了
    2) 如果您对这个单词并不熟悉，则直接安回车，就会展示单词的意思，然后接下来考你其他的单词。

    3) 如果你之前扔掉的单词，后悔了，希望加深记忆，那么先输入空格，然后再按回车键，则会把上一个扔掉的单词恢复。

    4) 如果你对某一个单词印象模糊，你可以输入一个?(即问好)，然后按回车，则系统会给你提示。提示信息是顺序打乱的，只有其中一个是正确的。这样可以提高你的专注度。

    5) 输入print 然后按回车，则会展示词库中所有单词词和意思。

    下面展示一下各种命令的效果，（print命令单独展示）

![Alt text](https://github.com/sioomy/beidanci/blob/master/resouce/02.png?raw=true)
    
    上图中展示的就是作者分别按回车、输入'后再按回车、输入空格再按回车的效果

    
![Alt text](https://github.com/sioomy/beidanci/blob/master/resouce/02.png?raw=true)

    上图中展示的是作者输入print 安回车的效果，数据量比较大，请慎重

    好了，就这么多，程序虽然简单，但是效果还不错，请尽情享用吧！
