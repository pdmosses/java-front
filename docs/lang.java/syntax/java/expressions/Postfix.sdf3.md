---
title: Postfix.sdf3
hide:
  - toc
---

# `Postfix.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/expressions/Postfix.sdf3]

[pdmosses/java-front/lang.java/syntax/java/expressions/Postfix.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/expressions/Postfix.sdf3 "The source file on GitHub"

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
12
13
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/expressions/Postfix_1_8" title="Multi-file references" data-urls="../Disambiguation.sdf3/#java/expressions/Postfix_5_3 line 5; ../Main.sdf3/#java/expressions/Postfix_14_3 line 14">java/expressions/Postfix</button>

<span class="layout">// 15.14. Postfix Expressions</span>

<span class="keyword">imports</span>
  <a href="../../names/Names.sdf3/#java/names/Names_1_8" id="java/names/Names_6_3" title="Defined at ../../names/Names.sdf3 line 1">java/names/Names</a>
  <a href="../Main.sdf3/#java/expressions/Main_1_8" id="java/expressions/Main_7_3" title="Defined at ../Main.sdf3 line 1">java/expressions/Main</a>

<span class="keyword">context-free syntax</span>
  
  <a href="#Expression_11_27" id="Expression_11_3" title="Referenced at line 11, 12">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#PostIncr_27_16" id="PostIncr_11_14" title="Referenced at ../Disambiguation.sdf3 line 27, 60">PostIncr</a></span> = &lt;&lt;<a href="#Expression_11_3" id="Expression_11_27" title="Defined at line 11, 12, 13">Expression</a>&gt;<span class="cons_String">++</span>&gt;
  <a href="#Expression_11_27" id="Expression_12_3" title="Referenced at line 11, 12">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#PostDecr_28_16" id="PostDecr_12_14" title="Referenced at ../Disambiguation.sdf3 line 28, 61">PostDecr</a></span> = &lt;&lt;<a href="#Expression_11_3" id="Expression_12_27" title="Defined at line 11, 12, 13">Expression</a>&gt;<span class="cons_String">--</span>&gt;
  <a href="#Expression_11_27" id="Expression_13_3" title="Referenced at line 11, 12">Expression</a> = <a href="../../names/Names.sdf3/#ExpressionName_13_3" id="ExpressionName_13_16" title="Defined at ../../names/Names.sdf3 line 13, 25, 26">ExpressionName</a>
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
