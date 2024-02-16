---
title: MethodReference.sdf3
hide:
  - toc
---

# `MethodReference.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/expressions/MethodReference.sdf3]

[pdmosses/java-front/lang.java/syntax/java/expressions/MethodReference.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/expressions/MethodReference.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3/#java/expressions/MethodReference_13_3" id="java/expressions/MethodReference_1_8" title="a definition with a single reference">java/expressions/MethodReference</a>

<span class="layout">// 15.13. Method Reference Expressions</span>

<span class="keyword">imports</span>
  <a href="../../types/ReferenceTypes.sdf3/#java/types/ReferenceTypes_1_8" id="java/types/ReferenceTypes_6_3" title="a reference to a single-file definition">java/types/ReferenceTypes</a>
  <a href="../../types/ParameterizedTypes.sdf3/#java/types/ParameterizedTypes_1_8" id="java/types/ParameterizedTypes_7_3" title="a reference to a single-file definition">java/types/ParameterizedTypes</a>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_8_3" title="a reference to a single-file definition">java/lexical/Identifiers</a>
  <a href="../../names/Names.sdf3/#java/names/Names_1_8" id="java/names/Names_9_3" title="a reference to a single-file definition">java/names/Names</a>
  <a href="../UnaryOperators.sdf3/#java/expressions/UnaryOperators_1_8" id="java/expressions/UnaryOperators_10_3" title="a reference to a single-file definition">java/expressions/UnaryOperators</a>

<span class="keyword">context-free syntax</span>
  
  <button class="modal-open" id="Expression_14_3" title="a definition with multiple references" data-urls="#Expression line 15_40, 22_3, 23_3, 23_37">Expression</button>.<span class="cons_Constructor"><span id="MethodReferenceRType_14_14" title="a definition with no references">MethodReferenceRType</span></span>  = &lt;&lt;<a href="../../types/ReferenceTypes.sdf3/#ReferenceType_13_3" id="ReferenceType_14_40" title="a reference to a single-file definition">ReferenceType</a>&gt;<span class="cons_String">::</span>&lt;<a href="../../types/ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_14_57" title="a reference to a single-file definition">TypeArguments</a>?&gt;&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_14_73" title="a reference to a single-file definition">Id</a>&gt;&gt;
  <button class="modal-open" id="Expression_15_3" title="a definition with multiple references" data-urls="#Expression line 15_40, 22_3, 23_3, 23_37">Expression</button>.<span class="cons_Constructor"><button class="modal-open" id="MethodReferenceExpr_15_14" title="a definition with multiple references" data-urls="#MethodReferenceExpr line 22_14, 23_14">MethodReferenceExpr</button></span>   = &lt;&lt;<a href="#Expression_14_3" id="Expression_15_40" title="a reference to a single-file definition">Expression</a>&gt;<span class="cons_String">::</span>&lt;<a href="../../types/ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_15_54" title="a reference to a single-file definition">TypeArguments</a>?&gt;&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_15_70" title="a reference to a single-file definition">Id</a>&gt;&gt;
  <button class="modal-open" id="Expression_16_3" title="a definition with multiple references" data-urls="#Expression line 15_40, 22_3, 23_3, 23_37">Expression</button>.<span class="cons_Constructor"><span id="MethodReferenceSuper_16_14" title="a definition with no references">MethodReferenceSuper</span></span>  = &lt;<span class="cons_String">super::</span>&lt;<a href="../../types/ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_16_47" title="a reference to a single-file definition">TypeArguments</a>?&gt;&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_16_63" title="a reference to a single-file definition">Id</a>&gt;&gt;
  <button class="modal-open" id="Expression_17_3" title="a definition with multiple references" data-urls="#Expression line 15_40, 22_3, 23_3, 23_37">Expression</button>.<span class="cons_Constructor"><span id="MethodReferenceQSuper_17_14" title="a definition with no references">MethodReferenceQSuper</span></span> = &lt;&lt;<a href="../../names/Names.sdf3/#TypeName_11_3" id="TypeName_17_40" title="a reference to a single-file definition">TypeName</a>&gt;<span class="cons_String">.super::</span>&lt;<a href="../../types/ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_17_58" title="a reference to a single-file definition">TypeArguments</a>?&gt;&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_17_74" title="a reference to a single-file definition">Id</a>&gt;&gt;
  <button class="modal-open" id="Expression_18_3" title="a definition with multiple references" data-urls="#Expression line 15_40, 22_3, 23_3, 23_37">Expression</button>.<span class="cons_Constructor"><span id="MethodReferenceCType_18_14" title="a definition with no references">MethodReferenceCType</span></span> = &lt;&lt;<a href="../../types/ReferenceTypes.sdf3/#ClassType_14_3" id="ClassType_18_39" title="a reference to a single-file definition">ClassType</a>&gt;<span class="cons_String">::</span>&lt;<a href="../../types/ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_18_52" title="a reference to a single-file definition">TypeArguments</a>?&gt; <span class="cons_String">new</span>&gt;
  <button class="modal-open" id="Expression_19_3" title="a definition with multiple references" data-urls="#Expression line 15_40, 22_3, 23_3, 23_37">Expression</button>.<span class="cons_Constructor"><span id="MethodReferenceAType_19_14" title="a definition with no references">MethodReferenceAType</span></span> = &lt;&lt;<a href="../../types/ReferenceTypes.sdf3/#ArrayType_16_3" id="ArrayType_19_39" title="a reference to a single-file definition">ArrayType</a>&gt;<span class="cons_String">::</span>&lt;<a href="../../types/ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_19_52" title="a reference to a single-file definition">TypeArguments</a>?&gt; <span class="cons_String">new</span>&gt;
  
<span class="keyword">context-free priorities</span>
  <a href="#Expression_14_3" id="Expression_22_3" title="a reference to a single-file definition">Expression</a>.<span class="cons_Constructor"><a href="#MethodReferenceExpr_15_14" id="MethodReferenceExpr_22_14" title="a reference to a single-file definition">MethodReferenceExpr</a></span> &gt; <button class="modal-open" id="Expression_22_36" title="a definition with multiple references" data-urls="#Expression line 15_40, 22_3, 23_3, 23_37">Expression</button> = <a href="../../names/Names.sdf3/#ExpressionName_13_3" id="ExpressionName_22_49" title="a reference to a single-file definition">ExpressionName</a>,
  <a href="#Expression_14_3" id="Expression_23_3" title="a reference to a single-file definition">Expression</a>.<span class="cons_Constructor"><a href="#MethodReferenceExpr_15_14" id="MethodReferenceExpr_23_14" title="a reference to a single-file definition">MethodReferenceExpr</a></span> &gt;  <a href="#Expression_14_3" id="Expression_23_37" title="a reference to a single-file definition">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3/#CastReference_23_14" id="CastReference_23_48" title="a reference to a single-file definition">CastReference</a></span>
  
<span class="keyword">template options</span>
  
  <span class="keyword">tokenize</span> : "::"  
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
