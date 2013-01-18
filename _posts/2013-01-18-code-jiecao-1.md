---
layout: post
title: 代码节操系列（一）
summary: 那些你看不懂的代码
---

_傻瓜都能写出机器能看懂的代码，聪明人才能写出人能看懂的代码。_

——— 某人  (这话谁说的我搜不到啊！)

---

## 那些你不懂的东西有多牛

有一些代码，写起来容易，写的人知道是什么意思，但是读的人未必能懂。比如机器语言、汇编语言、或者……
下面这样的代码（想必你一定见过类似的东西）：

<pre class="prettyprint lang-cpp linenums">
#include <stdio.h> 
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
