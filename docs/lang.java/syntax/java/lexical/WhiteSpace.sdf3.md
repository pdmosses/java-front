---
title: WhiteSpace.sdf3
hide:
  - toc
---

# `WhiteSpace.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/lexical/WhiteSpace.sdf3]

[pdmosses/java-front/lang.java/syntax/java/lexical/WhiteSpace.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/lexical/WhiteSpace.sdf3 "The source file on GitHub"

<div class="sdf3"><table class="highlighttable"><tbody><tr><td class="linenos"><div class="linenodiv"><pre><span></span>1
2
3
4
5
6
7
8
9
10
11
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/lexical/WhiteSpace_230_253" id="java/lexical/WhiteSpace_7_30" title="Referenced at ../Main.sdf3 line 12">java/lexical/WhiteSpace</a>

<span class="layout">// 3.6. White Space</span>

<span class="keyword">lexical syntax</span>

  <span class="keyword">LAYOUT</span> = [\ \t<span class="cons_Decimal">\12</span>\r\n]

<span class="keyword">context-free restrictions</span>

  <span class="keyword">LAYOUT</span>? -/- [\ \t<span class="cons_Decimal">\12</span>\n\r]
</code></pre></td></tr></tbody></table></div>