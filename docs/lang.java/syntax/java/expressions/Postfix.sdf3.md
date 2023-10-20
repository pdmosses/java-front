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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Disambiguation.sdf3/#java/expressions/Postfix_91_115" id="java/expressions/Postfix_7_31" title="Referenced at ../Disambiguation.sdf3 line 5; ../Main.sdf3 line 14">java/expressions/Postfix</a>

<span class="layout">// 15.14. Postfix Expressions</span>

<span class="keyword">imports</span>
  <a href="../../names/Names.sdf3/#java/names/Names_7_23" id="java/names/Names_74_90" title="Defined at ../../names/Names.sdf3 line 1">java/names/Names</a>
  <a href="../Main.sdf3/#java/expressions/Main_7_28" id="java/expressions/Main_93_114" title="Defined at ../Main.sdf3 line 1">java/expressions/Main</a>

<span class="keyword">context-free syntax</span>
  
  <a href="#Expression_165_175" id="Expression_141_151" title="Referenced at line 11, 12">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#PostIncr_605_613" id="PostIncr_152_160" title="Referenced at ../Disambiguation.sdf3 line 27, 60">PostIncr</a></span> = &lt;&lt;<a href="#Expression_141_151" id="Expression_165_175" title="Defined at line 11, 12, 13">Expression</a>&gt;<span class="cons_String">++</span>&gt;
  <a href="#Expression_165_175" id="Expression_182_192" title="Referenced at line 11, 12">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#PostDecr_630_638" id="PostDecr_193_201" title="Referenced at ../Disambiguation.sdf3 line 28, 61">PostDecr</a></span> = &lt;&lt;<a href="#Expression_141_151" id="Expression_206_216" title="Defined at line 11, 12, 13">Expression</a>&gt;<span class="cons_String">--</span>&gt;
  <a href="#Expression_165_175" id="Expression_223_233" title="Referenced at line 11, 12">Expression</a> = <a href="../../names/Names.sdf3/#ExpressionName_176_190" id="ExpressionName_236_250" title="Defined at ../../names/Names.sdf3 line 13, 25, 26">ExpressionName</a>
</code></pre></td></tr></tbody></table></div>