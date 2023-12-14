---
title: UnaryOperators.sdf3
hide:
  - toc
---

# `UnaryOperators.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/expressions/UnaryOperators.sdf3]

[pdmosses/java-front/lang.java/syntax/java/expressions/UnaryOperators.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/expressions/UnaryOperators.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/expressions/UnaryOperators_1_8" title="Multi-file references" data-urls="../Disambiguation.sdf3/#java/expressions/UnaryOperators_6_3 line 6; ../Main.sdf3/#java/expressions/UnaryOperators_15_3 line 15; ../MethodReference.sdf3/#java/expressions/UnaryOperators_10_3 line 10">java/expressions/UnaryOperators</button>

<span class="layout">// 15.15. Unary Operators</span>

<span class="keyword">imports</span>
  <a href="../../types/PrimitiveTypes.sdf3/#java/types/PrimitiveTypes_1_8" id="java/types/PrimitiveTypes_6_3" title="Defined at ../../types/PrimitiveTypes.sdf3 line 1">java/types/PrimitiveTypes</a>
  <a href="../../types/ReferenceTypes.sdf3/#java/types/ReferenceTypes_1_8" id="java/types/ReferenceTypes_7_3" title="Defined at ../../types/ReferenceTypes.sdf3 line 1">java/types/ReferenceTypes</a>
  <a href="../LambdaExpressions.sdf3/#java/expressions/LambdaExpressions_1_8" id="java/expressions/LambdaExpressions_8_3" title="Defined at ../LambdaExpressions.sdf3 line 1">java/expressions/LambdaExpressions</a> 

<span class="keyword">context-free sorts</span>

  <a href="#AdditionalBound_23_50" id="AdditionalBound_12_3" title="Referenced at line 23">AdditionalBound</a>

<span class="keyword">context-free syntax</span>
  
  <a href="#Expression_16_25" id="Expression_16_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#Plus_46_16" id="Plus_16_14" title="Referenced at ../Disambiguation.sdf3 line 46, 50, 64">Plus</a></span>  = &lt;<span class="cons_String">+</span>&lt;<a href="#Expression_16_3" id="Expression_16_25" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>&gt;&gt;
  <a href="#Expression_16_25" id="Expression_17_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#Minus_47_16" id="Minus_17_14" title="Referenced at ../Disambiguation.sdf3 line 47, 51, 65">Minus</a></span> = &lt;<span class="cons_String">-</span>&lt;<a href="#Expression_16_3" id="Expression_17_25" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>&gt;&gt;
  <a href="#Expression_16_25" id="Expression_18_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#PreIncr_44_16" id="PreIncr_18_14" title="Referenced at ../Disambiguation.sdf3 line 44, 62">PreIncr</a></span> = &lt;<span class="cons_String">++</span>&lt;<a href="#Expression_16_3" id="Expression_18_28" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>&gt;&gt;
  <a href="#Expression_16_25" id="Expression_19_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#PreDecr_45_16" id="PreDecr_19_14" title="Referenced at ../Disambiguation.sdf3 line 45, 63">PreDecr</a></span> = &lt;<span class="cons_String">--</span>&lt;<a href="#Expression_16_3" id="Expression_19_28" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>&gt;&gt;
  <a href="#Expression_16_25" id="Expression_20_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#Complement_66_16" id="Complement_20_14" title="Referenced at ../Disambiguation.sdf3 line 66">Complement</a></span> = &lt;<span class="cons_String">~</span>&lt;<a href="#Expression_16_3" id="Expression_20_30" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>&gt;&gt;
  <a href="#Expression_16_25" id="Expression_21_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#Not_67_16" id="Not_21_14" title="Referenced at ../Disambiguation.sdf3 line 67">Not</a></span>        = &lt;<span class="cons_String">!</span>&lt;<a href="#Expression_16_3" id="Expression_21_30" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>&gt;&gt;
  <a href="#Expression_16_25" id="Expression_22_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#CastPrimitive_30_16" id="CastPrimitive_22_14" title="Referenced at ../Disambiguation.sdf3 line 30, 35">CastPrimitive</a></span> = &lt;<span class="cons_String">(</span>&lt;<a href="../../types/PrimitiveTypes.sdf3/#PrimitiveType_10_3" id="PrimitiveType_22_33" title="Defined at ../../types/PrimitiveTypes.sdf3 line 10, 15, 16">PrimitiveType</a>&gt;<span class="cons_String">)</span> &lt;<a href="#Expression_16_3" id="Expression_22_50" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>&gt;&gt;
  <a href="#Expression_16_25" id="Expression_23_3" title="Referenced at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>.<span class="cons_Constructor"><button class="modal-open" id="CastReference_23_14" title="Multi-file references" data-urls="../Disambiguation.sdf3/#CastReference_31_16 line 31, 43, 49; ../MethodReference.sdf3/#CastReference_23_48 line 23">CastReference</button></span> = &lt;<span class="cons_String">(</span>&lt;<a href="../../types/ReferenceTypes.sdf3/#ReferenceType_13_3" id="ReferenceType_23_33" title="Defined at ../../types/ReferenceTypes.sdf3 line 13, 23, 24">ReferenceType</a>&gt; &lt;{<a href="#AdditionalBound_12_3" id="AdditionalBound_23_50" title="Defined at line 12, 24">AdditionalBound</a> <span class="cons_Lit">" "</span>}*&gt;<span class="cons_String">)</span> &lt;<a href="#Expression_16_3" id="Expression_23_75" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>&gt;&gt;
  <a href="#AdditionalBound_23_50" id="AdditionalBound_24_3" title="Referenced at line 23">AdditionalBound</a>.<span class="cons_Constructor"><span id="AdditionalBound_24_19" title="Not referenced">AdditionalBound</span></span> = &lt;<span class="cons_String">&amp;</span> &lt;<a href="../../types/ReferenceTypes.sdf3/#ClassType_14_3" id="ClassType_24_41" title="Defined at ../../types/ReferenceTypes.sdf3 line 14, 26, 27">ClassType</a>&gt;&gt;
  
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
