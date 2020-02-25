---
title: "gallery3"
date: 2018-03-06T16:01:23+08:00
lastmod: 2018-03-07T16:01:23+08:00
draft: false
tags: ["hugo"]
categories: ["Web","index"]
author: "dan"

# You can also close(false) or open(true) something for this content.
# P.S. comment can only be closed
# comment: false
# toc: false

# You can also define another contentCopyright. e.g. contentCopyright: "This is another copyright."
contentCopyright: '<a href="https://github.com/gohugoio/hugoBasicExample" rel="noopener" target="_blank">See origin</a>'
# reward: false
mathjax: true



menu:
  main:
    parent: "Docs"
    weight: 1
---

201807
 <script src="https://mermaidjs.github.io/scripts/mermaid.min.js"></script>
<script> mermaid.initialize({ startOnLoad: true });  </script>
 
<div class="mermaid">
graph LR
    A --- B
    B-->C[fa:fa-ban forbidden]
    B-->D(fa:fa-spinner);
</div>

<pre class="mermaid">graph LR
A[Bob<br>输入明文P] -->|P|B["Bob的私钥PRbob<br>加密算法(如RSA)<br>C=E(PRbob,P)"];
B -->|传输数字签名C|C["Alice的公钥环{PUbob,……}<br>解密算法(如RSA)<br>P=D(PUbob,C)"];
C -->|P|D["Alice<br>输出明文P"];</pre>


<div class="firstTest">
   graph LR;
    A--合并-->B;
    A-->C;
    B-->D;
    C-->D;
</div>
<script>     
 mermaid.init({noteMargin: 10}, ".firstTest");
</script>
————————————————
版权声明：本文为CSDN博主「赶路人儿」的原创文章，遵循 CC 4.0 BY-SA 版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/liuxiao723846/article/details/83544588