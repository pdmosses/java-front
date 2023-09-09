---
title: AssignmentOperators.sdf3
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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/expressions/AssignmentOperators_410_446" id="java/expressions/AssignmentOperators_7_43" title="Referenced at ../Main.sdf3 line 17">java/expressions/AssignmentOperators</a>

<span class="layout">// 15.26. Assignment Operators</span>

<span class="keyword">imports</span>
  <a href="../ArrayAccess.sdf3#java/expressions/ArrayAccess_7_35" id="java/expressions/ArrayAccess_87_115" title="Defined at ../ArrayAccess.sdf3 line 1">java/expressions/ArrayAccess</a>
  <a href="../FieldAccess.sdf3#java/expressions/FieldAccess_7_35" id="java/expressions/FieldAccess_118_146" title="Defined at ../FieldAccess.sdf3 line 1">java/expressions/FieldAccess</a>
  <a href="../../names/Names.sdf3#java/names/Names_7_23" id="java/names/Names_149_165" title="Defined at ../../names/Names.sdf3 line 1">java/names/Names</a>

<span class="keyword">context-free sorts</span>

  <a href="#LHS_882_885" id="LHS_189_192" title="Referenced at line 27">LHS</a>

<span class="keyword">context-free syntax</span>
  
  <a href="#Expression_891_901" id="Expression_219_229" title="Referenced at line 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#Assign_1939_1945" id="Assign_230_236" title="Referenced at ../Disambiguation.sdf3 line 95">Assign</a></span>            = &lt;&lt;<a href="#LHS_189_192" id="LHS_252_255" title="Defined at line 12, 29, 30, 31">LHS</a>&gt; <span class="cons_String">=</span> &lt;<a href="#Expression_219_229" id="Expression_260_270" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>&gt;&gt;
  <a href="#Expression_891_901" id="Expression_275_285" title="Referenced at line 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#AssignMul_1961_1970" id="AssignMul_286_295" title="Referenced at ../Disambiguation.sdf3 line 96">AssignMul</a></span>         = &lt;&lt;<a href="#LHS_189_192" id="LHS_308_311" title="Defined at line 12, 29, 30, 31">LHS</a>&gt; <span class="cons_String">*=</span> &lt;<a href="#Expression_219_229" id="Expression_317_327" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>&gt;&gt;
  <a href="#Expression_891_901" id="Expression_332_342" title="Referenced at line 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#AssignDiv_1986_1995" id="AssignDiv_343_352" title="Referenced at ../Disambiguation.sdf3 line 97">AssignDiv</a></span>         = &lt;&lt;<a href="#LHS_189_192" id="LHS_365_368" title="Defined at line 12, 29, 30, 31">LHS</a>&gt; <span class="cons_String">/=</span> &lt;<a href="#Expression_219_229" id="Expression_374_384" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>&gt;&gt;
  <a href="#Expression_891_901" id="Expression_389_399" title="Referenced at line 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#AssignMod_2011_2020" id="AssignMod_400_409" title="Referenced at ../Disambiguation.sdf3 line 98">AssignMod</a></span>         = &lt;&lt;<a href="#LHS_189_192" id="LHS_422_425" title="Defined at line 12, 29, 30, 31">LHS</a>&gt; <span class="cons_String">%=</span> &lt;<a href="#Expression_219_229" id="Expression_431_441" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>&gt;&gt;
  <a href="#Expression_891_901" id="Expression_446_456" title="Referenced at line 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#AssignAdd_2036_2045" id="AssignAdd_457_466" title="Referenced at ../Disambiguation.sdf3 line 99">AssignAdd</a></span>         = &lt;&lt;<a href="#LHS_189_192" id="LHS_479_482" title="Defined at line 12, 29, 30, 31">LHS</a>&gt; <span class="cons_String">+=</span> &lt;<a href="#Expression_219_229" id="Expression_488_498" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>&gt;&gt;
  <a href="#Expression_891_901" id="Expression_503_513" title="Referenced at line 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#AssignSub_2061_2070" id="AssignSub_514_523" title="Referenced at ../Disambiguation.sdf3 line 100">AssignSub</a></span>         = &lt;&lt;<a href="#LHS_189_192" id="LHS_536_539" title="Defined at line 12, 29, 30, 31">LHS</a>&gt; <span class="cons_String">-=</span> &lt;<a href="#Expression_219_229" id="Expression_545_555" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>&gt;&gt;
  <a href="#Expression_891_901" id="Expression_560_570" title="Referenced at line 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#AssignLeftShift_2086_2101" id="AssignLeftShift_571_586" title="Referenced at ../Disambiguation.sdf3 line 101">AssignLeftShift</a></span>   = [[<a href="#LHS_189_192" id="LHS_593_596" title="Defined at line 12, 29, 30, 31">LHS</a>] <span class="cons_String">&lt;&lt;=</span> [<a href="#Expression_219_229" id="Expression_603_613" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>]]
  <a href="#Expression_891_901" id="Expression_618_628" title="Referenced at line 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#AssignRightShift_2117_2133" id="AssignRightShift_629_645" title="Referenced at ../Disambiguation.sdf3 line 102">AssignRightShift</a></span>  = [[<a href="#LHS_189_192" id="LHS_651_654" title="Defined at line 12, 29, 30, 31">LHS</a>] <span class="cons_String">&gt;&gt;=</span> [<a href="#Expression_219_229" id="Expression_661_671" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>]]
  <a href="#Expression_891_901" id="Expression_676_686" title="Referenced at line 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#AssignURightShift_2149_2166" id="AssignURightShift_687_704" title="Referenced at ../Disambiguation.sdf3 line 103">AssignURightShift</a></span> = [[<a href="#LHS_189_192" id="LHS_709_712" title="Defined at line 12, 29, 30, 31">LHS</a>] <span class="cons_String">&gt;&gt;&gt;=</span> [<a href="#Expression_219_229" id="Expression_720_730" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>]]
  <a href="#Expression_891_901" id="Expression_735_745" title="Referenced at line 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#AssignAnd_2182_2191" id="AssignAnd_746_755" title="Referenced at ../Disambiguation.sdf3 line 104">AssignAnd</a></span>         = &lt;&lt;<a href="#LHS_189_192" id="LHS_768_771" title="Defined at line 12, 29, 30, 31">LHS</a>&gt; <span class="cons_String">&amp;=</span> &lt;<a href="#Expression_219_229" id="Expression_777_787" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>&gt;&gt;
  <a href="#Expression_891_901" id="Expression_792_802" title="Referenced at line 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#AssignXor_2207_2216" id="AssignXor_803_812" title="Referenced at ../Disambiguation.sdf3 line 105">AssignXor</a></span>         = &lt;&lt;<a href="#LHS_189_192" id="LHS_825_828" title="Defined at line 12, 29, 30, 31">LHS</a>&gt; <span class="cons_String">^=</span> &lt;<a href="#Expression_219_229" id="Expression_834_844" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>&gt;&gt;
  <a href="#Expression_891_901" id="Expression_849_859" title="Referenced at line 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#AssignOr_2232_2240" id="AssignOr_860_868" title="Referenced at ../Disambiguation.sdf3 line 106">AssignOr</a></span>          = &lt;&lt;<a href="#LHS_189_192" id="LHS_882_885" title="Defined at line 12, 29, 30, 31">LHS</a>&gt; <span class="cons_String">|=</span> &lt;<a href="#Expression_219_229" id="Expression_891_901" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27">Expression</a>&gt;&gt;
  
  <a href="#LHS_882_885" id="LHS_909_912" title="Referenced at line 27">LHS</a> = <a href="../../names/Names.sdf3#ExpressionName_176_190" id="ExpressionName_915_929" title="Defined at ../../names/Names.sdf3 line 13, 25, 26">ExpressionName</a>
  <a href="#LHS_882_885" id="LHS_932_935" title="Referenced at line 27">LHS</a> = <a href="../FieldAccess.sdf3#FieldAccess_174_185" id="FieldAccess_938_949" title="Defined at ../FieldAccess.sdf3 line 12, 18, 19, 20">FieldAccess</a>
  <a href="#LHS_882_885" id="LHS_952_955" title="Referenced at line 27">LHS</a> = <a href="../ArrayAccess.sdf3#ArrayAccess_158_169" id="ArrayAccess_958_969" title="Defined at ../ArrayAccess.sdf3 line 11, 17">ArrayAccess</a>
</code></pre></td></tr></tbody></table></div>