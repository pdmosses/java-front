---
title: BinaryOperators.sdf3
hide:
  - toc
---

# `BinaryOperators.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/expressions/BinaryOperators.sdf3]

[pdmosses/java-front/lang.java/syntax/java/expressions/BinaryOperators.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/expressions/BinaryOperators.sdf3 "The source file on GitHub"

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
32
33
34
35
36
37
38
39
40
41
42
43
44
45
46
47
48
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/expressions/BinaryOperators_1_8" title="Multi-file references" data-urls="../Disambiguation.sdf3/#java/expressions/BinaryOperators_7_3 line 7; ../Main.sdf3/#java/expressions/BinaryOperators_16_3 line 16">java/expressions/BinaryOperators</button>

<span class="layout">// 15.17. Multiplicative Operators</span>
<span class="layout">// 15.18. Additive Operators</span>
<span class="layout">// 15.19. Shift Operators</span>
<span class="layout">// 15.20. Relational Operators</span>
<span class="layout">// 15.21. Equality Operators</span>
<span class="layout">// 15.22. Bitwise and Logical Operators</span>
<span class="layout">// 15.23. Conditional-And Operator &amp;&amp;</span>
<span class="layout">// 15.24. Conditional-Or Operator ||</span>

<span class="keyword">imports</span>
  <a href="../../types/ReferenceTypes.sdf3/#java/types/ReferenceTypes_1_8" id="java/types/ReferenceTypes_13_3" title="Defined at ../../types/ReferenceTypes.sdf3 line 1">java/types/ReferenceTypes</a>

<span class="keyword">context-free syntax</span>
  
  <a href="#Expression_17_22" id="Expression_17_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#Mul_37_16" id="Mul_17_14" title="Referenced at ../Disambiguation.sdf3 line 37, 69">Mul</a></span> = &lt;&lt;<a href="#Expression_17_3" id="Expression_17_22" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">*</span> &lt;<a href="#Expression_17_3" id="Expression_17_37" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  <a href="#Expression_17_22" id="Expression_18_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#Div_38_16" id="Div_18_14" title="Referenced at ../Disambiguation.sdf3 line 38, 70">Div</a></span> = &lt;&lt;<a href="#Expression_17_3" id="Expression_18_22" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">/</span> &lt;<a href="#Expression_17_3" id="Expression_18_37" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  <a href="#Expression_17_22" id="Expression_19_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#Mod_39_16" id="Mod_19_14" title="Referenced at ../Disambiguation.sdf3 line 39, 71">Mod</a></span> = &lt;&lt;<a href="#Expression_17_3" id="Expression_19_22" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">%</span> &lt;<a href="#Expression_17_3" id="Expression_19_37" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  
  <a href="#Expression_17_22" id="Expression_21_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#Add_73_16" id="Add_21_14" title="Referenced at ../Disambiguation.sdf3 line 73">Add</a></span> = &lt;&lt;<a href="#Expression_17_3" id="Expression_21_22" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">+</span> &lt;<a href="#Expression_17_3" id="Expression_21_37" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  <a href="#Expression_17_22" id="Expression_22_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#Sub_74_16" id="Sub_22_14" title="Referenced at ../Disambiguation.sdf3 line 74">Sub</a></span> = &lt;&lt;<a href="#Expression_17_3" id="Expression_22_22" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">-</span> &lt;<a href="#Expression_17_3" id="Expression_22_37" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  
  <a href="#Expression_17_22" id="Expression_24_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#LeftShift_76_16" id="LeftShift_24_14" title="Referenced at ../Disambiguation.sdf3 line 76">LeftShift</a></span> = [[<a href="#Expression_17_3" id="Expression_24_28" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>] <span class="cons_String">&lt;&lt;</span> [<a href="#Expression_17_3" id="Expression_24_44" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>]] {<span class="keyword">left</span>}
  <a href="#Expression_17_22" id="Expression_25_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#RightShift_77_16" id="RightShift_25_14" title="Referenced at ../Disambiguation.sdf3 line 77">RightShift</a></span> = [[<a href="#Expression_17_3" id="Expression_25_29" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>] <span class="cons_String">&gt;&gt;</span> [<a href="#Expression_17_3" id="Expression_25_45" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>]] {<span class="keyword">left</span>}
  <a href="#Expression_17_22" id="Expression_26_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#URightShift_78_16" id="URightShift_26_14" title="Referenced at ../Disambiguation.sdf3 line 78">URightShift</a></span> = [[<a href="#Expression_17_3" id="Expression_26_30" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>] <span class="cons_String">&gt;&gt;&gt;</span> [<a href="#Expression_17_3" id="Expression_26_47" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>]] {<span class="keyword">left</span>}
  
  <a href="#Expression_17_22" id="Expression_28_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#Lt_81_16" id="Lt_28_14" title="Referenced at ../Disambiguation.sdf3 line 81">Lt</a></span>   = [[<a href="#Expression_17_3" id="Expression_28_23" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>] <span class="cons_String">&lt;</span> [<a href="#Expression_17_3" id="Expression_28_38" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>]] {<span class="keyword">left</span>}
  <a href="#Expression_17_22" id="Expression_29_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#Gt_82_16" id="Gt_29_14" title="Referenced at ../Disambiguation.sdf3 line 82">Gt</a></span>   = [[<a href="#Expression_17_3" id="Expression_29_23" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>] <span class="cons_String">&gt;</span> [<a href="#Expression_17_3" id="Expression_29_38" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>]] {<span class="keyword">left</span>}
  <a href="#Expression_17_22" id="Expression_30_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#LtEq_83_16" id="LtEq_30_14" title="Referenced at ../Disambiguation.sdf3 line 83">LtEq</a></span> = [[<a href="#Expression_17_3" id="Expression_30_23" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>] <span class="cons_String">&lt;=</span> [<a href="#Expression_17_3" id="Expression_30_39" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>]] {<span class="keyword">left</span>}
  <a href="#Expression_17_22" id="Expression_31_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#GtEq_84_16" id="GtEq_31_14" title="Referenced at ../Disambiguation.sdf3 line 84">GtEq</a></span> = [[<a href="#Expression_17_3" id="Expression_31_23" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>] <span class="cons_String">&gt;=</span> [<a href="#Expression_17_3" id="Expression_31_39" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>]] {<span class="keyword">left</span>}
  <a href="#Expression_17_22" id="Expression_32_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#InstanceOf_80_16" id="InstanceOf_32_14" title="Referenced at ../Disambiguation.sdf3 line 80">InstanceOf</a></span> = &lt;&lt;<a href="#Expression_17_3" id="Expression_32_29" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">instanceof</span> &lt;<a href="../../types/ReferenceTypes.sdf3/#ReferenceType_13_3" id="ReferenceType_32_53" title="Defined at ../../types/ReferenceTypes.sdf3 line 13, 23, 24">ReferenceType</a>&gt;&gt;
  
  <a href="#Expression_17_22" id="Expression_34_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#Eq_86_16" id="Eq_34_14" title="Referenced at ../Disambiguation.sdf3 line 86">Eq</a></span>    = &lt;&lt;<a href="#Expression_17_3" id="Expression_34_24" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">==</span> &lt;<a href="#Expression_17_3" id="Expression_34_40" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  <a href="#Expression_17_22" id="Expression_35_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#NotEq_87_16" id="NotEq_35_14" title="Referenced at ../Disambiguation.sdf3 line 87">NotEq</a></span> = &lt;&lt;<a href="#Expression_17_3" id="Expression_35_24" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">!=</span> &lt;<a href="#Expression_17_3" id="Expression_35_40" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  
  <a href="#Expression_17_22" id="Expression_37_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#And_88_14" id="And_37_14" title="Referenced at ../Disambiguation.sdf3 line 88">And</a></span> = &lt;&lt;<a href="#Expression_17_3" id="Expression_37_22" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">&amp;</span> &lt;<a href="#Expression_17_3" id="Expression_37_37" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  <a href="#Expression_17_22" id="Expression_38_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#Xor_89_14" id="Xor_38_14" title="Referenced at ../Disambiguation.sdf3 line 89">Xor</a></span> = &lt;&lt;<a href="#Expression_17_3" id="Expression_38_22" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">^</span> &lt;<a href="#Expression_17_3" id="Expression_38_37" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  <a href="#Expression_17_22" id="Expression_39_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#Or_90_14" id="Or_39_14" title="Referenced at ../Disambiguation.sdf3 line 90">Or</a></span>  = &lt;&lt;<a href="#Expression_17_3" id="Expression_39_22" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">|</span> &lt;<a href="#Expression_17_3" id="Expression_39_37" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  
  <a href="#Expression_17_22" id="Expression_41_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#LazyAnd_91_14" id="LazyAnd_41_14" title="Referenced at ../Disambiguation.sdf3 line 91">LazyAnd</a></span> = &lt;&lt;<a href="#Expression_17_3" id="Expression_41_26" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">&amp;&amp;</span> &lt;<a href="#Expression_17_3" id="Expression_41_42" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  <a href="#Expression_17_22" id="Expression_42_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#LazyOr_92_14" id="LazyOr_42_14" title="Referenced at ../Disambiguation.sdf3 line 92">LazyOr</a></span>  = &lt;&lt;<a href="#Expression_17_3" id="Expression_42_26" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">||</span> &lt;<a href="#Expression_17_3" id="Expression_42_42" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">left</span>}
  
  <a href="#Expression_17_22" id="Expression_44_3" title="Referenced at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#Cond_93_14" id="Cond_44_14" title="Referenced at ../Disambiguation.sdf3 line 93">Cond</a></span> = &lt;&lt;<a href="#Expression_17_3" id="Expression_44_23" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">?</span> &lt;<a href="#Expression_17_3" id="Expression_44_38" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt; <span class="cons_String">:</span> &lt;<a href="#Expression_17_3" id="Expression_44_53" title="Defined at line 17, 18, 19, 21, 22, 24, 25, 26, 28, 29, 30, 31, 32, 34, 35, 37, 38, 39, 41, 42, 44">Expression</a>&gt;&gt; {<span class="keyword">right</span>}
  
  
  
  
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
