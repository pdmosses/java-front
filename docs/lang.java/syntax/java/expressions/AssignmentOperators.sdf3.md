---
title: AssignmentOperators.sdf3
hide:
  - toc
---

# `AssignmentOperators.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/expressions/AssignmentOperators.sdf3]

[pdmosses/java-front/lang.java/syntax/java/expressions/AssignmentOperators.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/expressions/AssignmentOperators.sdf3 "The source file on GitHub"

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
14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
29
30
31
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/expressions/AssignmentOperators_1_8" title="Multi-file references" data-urls="../Disambiguation.sdf3/#java/expressions/AssignmentOperators_11_3 line 11; ../Main.sdf3/#java/expressions/AssignmentOperators_17_3 line 17">java/expressions/AssignmentOperators</button>

<span class="layout">// 15.26. Assignment Operators</span>

<span class="keyword">imports</span>
  <a href="../ArrayAccess.sdf3/#java/expressions/ArrayAccess_1_8" id="java/expressions/ArrayAccess_6_3" title="Defined at ../ArrayAccess.sdf3 line 1">java/expressions/ArrayAccess</a>
  <a href="../FieldAccess.sdf3/#java/expressions/FieldAccess_1_8" id="java/expressions/FieldAccess_7_3" title="Defined at ../FieldAccess.sdf3 line 1">java/expressions/FieldAccess</a>
  <a href="../../names/Names.sdf3/#java/names/Names_1_8" id="java/names/Names_8_3" title="Defined at ../../names/Names.sdf3 line 1">java/names/Names</a>

<span class="keyword">context-free sorts</span>

  <a href="#LHS_16_36" id="LHS_12_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">LHS</a>

<span class="keyword">context-free syntax</span>
  
  <a href="#Expression_16_44" id="Expression_16_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#Assign_21_14" id="Assign_16_14" title="Referenced at ../Disambiguation.sdf3 line 21, 95">Assign</a></span>            = &lt;&lt;<a href="#LHS_12_3" id="LHS_16_36" title="Defined at line 12, 29, 30, 31">LHS</a>&gt; <span class="cons_String">=</span> &lt;<a href="#Expression_16_3" id="Expression_16_44" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>&gt;&gt;
  <a href="#Expression_16_44" id="Expression_17_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#AssignMul_96_16" id="AssignMul_17_14" title="Referenced at ../Disambiguation.sdf3 line 96">AssignMul</a></span>         = &lt;&lt;<a href="#LHS_12_3" id="LHS_17_36" title="Defined at line 12, 29, 30, 31">LHS</a>&gt; <span class="cons_String">*=</span> &lt;<a href="#Expression_16_3" id="Expression_17_45" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>&gt;&gt;
  <a href="#Expression_16_44" id="Expression_18_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#AssignDiv_97_16" id="AssignDiv_18_14" title="Referenced at ../Disambiguation.sdf3 line 97">AssignDiv</a></span>         = &lt;&lt;<a href="#LHS_12_3" id="LHS_18_36" title="Defined at line 12, 29, 30, 31">LHS</a>&gt; <span class="cons_String">/=</span> &lt;<a href="#Expression_16_3" id="Expression_18_45" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>&gt;&gt;
  <a href="#Expression_16_44" id="Expression_19_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#AssignMod_98_16" id="AssignMod_19_14" title="Referenced at ../Disambiguation.sdf3 line 98">AssignMod</a></span>         = &lt;&lt;<a href="#LHS_12_3" id="LHS_19_36" title="Defined at line 12, 29, 30, 31">LHS</a>&gt; <span class="cons_String">%=</span> &lt;<a href="#Expression_16_3" id="Expression_19_45" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>&gt;&gt;
  <a href="#Expression_16_44" id="Expression_20_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#AssignAdd_99_16" id="AssignAdd_20_14" title="Referenced at ../Disambiguation.sdf3 line 99">AssignAdd</a></span>         = &lt;&lt;<a href="#LHS_12_3" id="LHS_20_36" title="Defined at line 12, 29, 30, 31">LHS</a>&gt; <span class="cons_String">+=</span> &lt;<a href="#Expression_16_3" id="Expression_20_45" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>&gt;&gt;
  <a href="#Expression_16_44" id="Expression_21_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#AssignSub_100_16" id="AssignSub_21_14" title="Referenced at ../Disambiguation.sdf3 line 100">AssignSub</a></span>         = &lt;&lt;<a href="#LHS_12_3" id="LHS_21_36" title="Defined at line 12, 29, 30, 31">LHS</a>&gt; <span class="cons_String">-=</span> &lt;<a href="#Expression_16_3" id="Expression_21_45" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>&gt;&gt;
  <a href="#Expression_16_44" id="Expression_22_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#AssignLeftShift_101_16" id="AssignLeftShift_22_14" title="Referenced at ../Disambiguation.sdf3 line 101">AssignLeftShift</a></span>   = [[<a href="#LHS_12_3" id="LHS_22_36" title="Defined at line 12, 29, 30, 31">LHS</a>] <span class="cons_String">&lt;&lt;=</span> [<a href="#Expression_16_3" id="Expression_22_46" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>]]
  <a href="#Expression_16_44" id="Expression_23_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#AssignRightShift_102_16" id="AssignRightShift_23_14" title="Referenced at ../Disambiguation.sdf3 line 102">AssignRightShift</a></span>  = [[<a href="#LHS_12_3" id="LHS_23_36" title="Defined at line 12, 29, 30, 31">LHS</a>] <span class="cons_String">&gt;&gt;=</span> [<a href="#Expression_16_3" id="Expression_23_46" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>]]
  <a href="#Expression_16_44" id="Expression_24_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#AssignURightShift_103_16" id="AssignURightShift_24_14" title="Referenced at ../Disambiguation.sdf3 line 103">AssignURightShift</a></span> = [[<a href="#LHS_12_3" id="LHS_24_36" title="Defined at line 12, 29, 30, 31">LHS</a>] <span class="cons_String">&gt;&gt;&gt;=</span> [<a href="#Expression_16_3" id="Expression_24_47" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>]]
  <a href="#Expression_16_44" id="Expression_25_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#AssignAnd_104_16" id="AssignAnd_25_14" title="Referenced at ../Disambiguation.sdf3 line 104">AssignAnd</a></span>         = &lt;&lt;<a href="#LHS_12_3" id="LHS_25_36" title="Defined at line 12, 29, 30, 31">LHS</a>&gt; <span class="cons_String">&amp;=</span> &lt;<a href="#Expression_16_3" id="Expression_25_45" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>&gt;&gt;
  <a href="#Expression_16_44" id="Expression_26_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#AssignXor_105_16" id="AssignXor_26_14" title="Referenced at ../Disambiguation.sdf3 line 105">AssignXor</a></span>         = &lt;&lt;<a href="#LHS_12_3" id="LHS_26_36" title="Defined at line 12, 29, 30, 31">LHS</a>&gt; <span class="cons_String">^=</span> &lt;<a href="#Expression_16_3" id="Expression_26_45" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>&gt;&gt;
  <a href="#Expression_16_44" id="Expression_27_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#AssignOr_106_16" id="AssignOr_27_14" title="Referenced at ../Disambiguation.sdf3 line 106">AssignOr</a></span>          = &lt;&lt;<a href="#LHS_12_3" id="LHS_27_36" title="Defined at line 12, 29, 30, 31">LHS</a>&gt; <span class="cons_String">|=</span> &lt;<a href="#Expression_16_3" id="Expression_27_45" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>&gt;&gt;
  
  <a href="#LHS_16_36" id="LHS_29_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">LHS</a> = <a href="../../names/Names.sdf3/#ExpressionName_13_3" id="ExpressionName_29_9" title="Defined at ../../names/Names.sdf3 line 13, 25, 26">ExpressionName</a>
  <a href="#LHS_16_36" id="LHS_30_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">LHS</a> = <a href="../FieldAccess.sdf3/#FieldAccess_12_3" id="FieldAccess_30_9" title="Defined at ../FieldAccess.sdf3 line 12, 18, 19, 20">FieldAccess</a>
  <a href="#LHS_16_36" id="LHS_31_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">LHS</a> = <a href="../ArrayAccess.sdf3/#ArrayAccess_11_3" id="ArrayAccess_31_9" title="Defined at ../ArrayAccess.sdf3 line 11, 17">ArrayAccess</a>
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
