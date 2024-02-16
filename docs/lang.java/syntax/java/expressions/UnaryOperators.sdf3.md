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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/expressions/UnaryOperators_1_8" title="a definition with multiple references" data-urls="../Disambiguation.sdf3/#java/expressions/UnaryOperators line 6_3; ../Main.sdf3/#java/expressions/UnaryOperators line 15_3; ../MethodReference.sdf3/#java/expressions/UnaryOperators line 10_3">java/expressions/UnaryOperators</button>

<span class="layout">// 15.15. Unary Operators</span>

<span class="keyword">imports</span>
  <a href="../../types/PrimitiveTypes.sdf3/#java/types/PrimitiveTypes_1_8" id="java/types/PrimitiveTypes_6_3" title="a reference to a single-file definition">java/types/PrimitiveTypes</a>
  <a href="../../types/ReferenceTypes.sdf3/#java/types/ReferenceTypes_1_8" id="java/types/ReferenceTypes_7_3" title="a reference to a single-file definition">java/types/ReferenceTypes</a>
  <a href="../LambdaExpressions.sdf3/#java/expressions/LambdaExpressions_1_8" id="java/expressions/LambdaExpressions_8_3" title="a reference to a single-file definition">java/expressions/LambdaExpressions</a> 

<span class="keyword">context-free sorts</span>

  <a href="#AdditionalBound_23_50" id="AdditionalBound_12_3" title="a definition with a single reference">AdditionalBound</a>

<span class="keyword">context-free syntax</span>
  
  <button class="modal-open" id="Expression_16_3" title="a definition with multiple references" data-urls="#Expression line 16_25, 17_25, 18_28, 19_28, 20_30, 21_30, 22_50, 23_75">Expression</button>.<span class="cons_Constructor"><button class="modal-open" id="Plus_16_14" title="a definition with multiple references" data-urls="../Disambiguation.sdf3/#Plus line 46_16, 50_16, 64_16">Plus</button></span>  = &lt;<span class="cons_String">+</span>&lt;<a href="#Expression_16_3" id="Expression_16_25" title="a reference to a single-file definition">Expression</a>&gt;&gt;
  <button class="modal-open" id="Expression_17_3" title="a definition with multiple references" data-urls="#Expression line 16_25, 17_25, 18_28, 19_28, 20_30, 21_30, 22_50, 23_75">Expression</button>.<span class="cons_Constructor"><button class="modal-open" id="Minus_17_14" title="a definition with multiple references" data-urls="../Disambiguation.sdf3/#Minus line 47_16, 51_16, 65_16">Minus</button></span> = &lt;<span class="cons_String">-</span>&lt;<a href="#Expression_16_3" id="Expression_17_25" title="a reference to a single-file definition">Expression</a>&gt;&gt;
  <button class="modal-open" id="Expression_18_3" title="a definition with multiple references" data-urls="#Expression line 16_25, 17_25, 18_28, 19_28, 20_30, 21_30, 22_50, 23_75">Expression</button>.<span class="cons_Constructor"><button class="modal-open" id="PreIncr_18_14" title="a definition with multiple references" data-urls="../Disambiguation.sdf3/#PreIncr line 44_16, 62_16">PreIncr</button></span> = &lt;<span class="cons_String">++</span>&lt;<a href="#Expression_16_3" id="Expression_18_28" title="a reference to a single-file definition">Expression</a>&gt;&gt;
  <button class="modal-open" id="Expression_19_3" title="a definition with multiple references" data-urls="#Expression line 16_25, 17_25, 18_28, 19_28, 20_30, 21_30, 22_50, 23_75">Expression</button>.<span class="cons_Constructor"><button class="modal-open" id="PreDecr_19_14" title="a definition with multiple references" data-urls="../Disambiguation.sdf3/#PreDecr line 45_16, 63_16">PreDecr</button></span> = &lt;<span class="cons_String">--</span>&lt;<a href="#Expression_16_3" id="Expression_19_28" title="a reference to a single-file definition">Expression</a>&gt;&gt;
  <button class="modal-open" id="Expression_20_3" title="a definition with multiple references" data-urls="#Expression line 16_25, 17_25, 18_28, 19_28, 20_30, 21_30, 22_50, 23_75">Expression</button>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#Complement_66_16" id="Complement_20_14" title="a definition with a single reference">Complement</a></span> = &lt;<span class="cons_String">~</span>&lt;<a href="#Expression_16_3" id="Expression_20_30" title="a reference to a single-file definition">Expression</a>&gt;&gt;
  <button class="modal-open" id="Expression_21_3" title="a definition with multiple references" data-urls="#Expression line 16_25, 17_25, 18_28, 19_28, 20_30, 21_30, 22_50, 23_75">Expression</button>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#Not_67_16" id="Not_21_14" title="a definition with a single reference">Not</a></span>        = &lt;<span class="cons_String">!</span>&lt;<a href="#Expression_16_3" id="Expression_21_30" title="a reference to a single-file definition">Expression</a>&gt;&gt;
  <button class="modal-open" id="Expression_22_3" title="a definition with multiple references" data-urls="#Expression line 16_25, 17_25, 18_28, 19_28, 20_30, 21_30, 22_50, 23_75">Expression</button>.<span class="cons_Constructor"><button class="modal-open" id="CastPrimitive_22_14" title="a definition with multiple references" data-urls="../Disambiguation.sdf3/#CastPrimitive line 30_16, 35_14">CastPrimitive</button></span> = &lt;<span class="cons_String">(</span>&lt;<a href="../../types/PrimitiveTypes.sdf3/#PrimitiveType_10_3" id="PrimitiveType_22_33" title="a reference to a single-file definition">PrimitiveType</a>&gt;<span class="cons_String">)</span> &lt;<a href="#Expression_16_3" id="Expression_22_50" title="a reference to a single-file definition">Expression</a>&gt;&gt;
  <button class="modal-open" id="Expression_23_3" title="a definition with multiple references" data-urls="#Expression line 16_25, 17_25, 18_28, 19_28, 20_30, 21_30, 22_50, 23_75">Expression</button>.<span class="cons_Constructor"><button class="modal-open" id="CastReference_23_14" title="a definition with multiple references" data-urls="../Disambiguation.sdf3/#CastReference line 31_16, 43_14, 49_14; ../MethodReference.sdf3/#CastReference line 23_48">CastReference</button></span> = &lt;<span class="cons_String">(</span>&lt;<a href="../../types/ReferenceTypes.sdf3/#ReferenceType_13_3" id="ReferenceType_23_33" title="a reference to a single-file definition">ReferenceType</a>&gt; &lt;{<a href="#AdditionalBound_12_3" id="AdditionalBound_23_50" title="a reference to a single-file definition">AdditionalBound</a> <span class="cons_Lit">" "</span>}*&gt;<span class="cons_String">)</span> &lt;<a href="#Expression_16_3" id="Expression_23_75" title="a reference to a single-file definition">Expression</a>&gt;&gt;
  <a href="#AdditionalBound_23_50" id="AdditionalBound_24_3" title="a definition with a single reference">AdditionalBound</a>.<span class="cons_Constructor"><span id="AdditionalBound_24_19" title="a definition with no references">AdditionalBound</span></span> = &lt;<span class="cons_String">&amp;</span> &lt;<a href="../../types/ReferenceTypes.sdf3/#ClassType_14_3" id="ClassType_24_41" title="a reference to a single-file definition">ClassType</a>&gt;&gt;
  
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
