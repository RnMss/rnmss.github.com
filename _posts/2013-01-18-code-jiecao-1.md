---
layout: post
title: 代码节操系列（一）
summary: 那些你看不懂的代码
---

> 傻瓜都能写出机器能看懂的代码，聪明人才能写出人能看懂的代码。

<span style="padding-left: 5em">——某人  (这话谁说的我搜不到啊！)</span>

---

## 那些你不懂的东西有多牛

有一些代码，写起来容易，写的人知道是什么意思，但是读的人未必能懂。比如机器语言、汇编语言、或者……
下面这样的代码（想必你一定见过类似的东西）：

<pre class="prettyprint lang-cpp linenums">
#include &lt;stdio.h&gt; 
#define _ i 
#define __ n 
#define ___ _##__##t 
#define ____ scanf 
#define _____ printf 
#define ______ "%d" 
___ main() { 
    ___ _, __; 
    ____(______ ______, &_, &__); 
    _____(______ "\n", _+__); 
    return 0; 
}
</pre>

其实把“`#define`”展开，就变成了这个样子：

<pre class="prettyprint lang-cpp linenums">
#include &lt;stdio.h&gt; 
int main() { 
    int a, b; 
    scanf("%d%d", &a, &b); 
    printf("%d\n", a+b); 
    return 0; 
}
</pre>

啦啦啦~~ 一段你能看懂的代码，稍加修改，就变成了前面那个样子，几乎无法阅读了。

所以永远不要那些你看不懂的代码有什么值得膜拜的地方，有些只是他们写得不够简单易懂而已。

不要觉得那些你不懂的东西有多牛，因为那往往只是叙述者 *捉鸡* 的表达能力，或者故弄玄虚的卖 *节操* 行为~

## 为什么有些代码读不懂
