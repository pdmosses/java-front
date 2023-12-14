---
title: ArrayCreation.sdf3
hide:
  - toc
---

# `ArrayCreation.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/expressions/ArrayCreation.sdf3]

[pdmosses/java-front/lang.java/syntax/java/expressions/ArrayCreation.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/expressions/ArrayCreation.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/expressions/ArrayCreation_1_8" title="Multi-file references" data-urls="../ArrayAccess.sdf3/#java/expressions/ArrayCreation_7_3 line 7; ../Main.sdf3/#java/expressions/ArrayCreation_9_3 line 9">java/expressions/ArrayCreation</button>

<span class="layout">// 15.10.1. Array Creation Expressions</span>

<span class="keyword">imports</span>
  <a href="../../types/ReferenceTypes.sdf3/#java/types/ReferenceTypes_1_8" id="java/types/ReferenceTypes_6_3" title="Defined at ../../types/ReferenceTypes.sdf3 line 1">java/types/ReferenceTypes</a>
  <a href="../../types/PrimitiveTypes.sdf3/#java/types/PrimitiveTypes_1_8" id="java/types/PrimitiveTypes_7_3" title="Defined at ../../types/PrimitiveTypes.sdf3 line 1">java/types/PrimitiveTypes</a>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_1_8" id="java/interfaces/Annotations_8_3" title="Defined at ../../interfaces/Annotations.sdf3 line 1">java/interfaces/Annotations</a>
  <a href="../../arrays/ArrayInitializers.sdf3/#java/arrays/ArrayInitializers_1_8" id="java/arrays/ArrayInitializers_9_3" title="Defined at ../../arrays/ArrayInitializers.sdf3 line 1">java/arrays/ArrayInitializers</a>

<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="ArrayCreationExpression_13_3" title="Multi-file references" data-urls="#ArrayCreationExpression_19_16 line 19; ../ArrayAccess.sdf3/#ArrayCreationExpression_21_48 line 21">ArrayCreationExpression</button>
  <a href="#ArrayBaseType_20_44" id="ArrayBaseType_14_3" title="Referenced at line 20, 21">ArrayBaseType</a>
  <a href="#DimExpr_20_60" id="DimExpr_15_3" title="Referenced at line 20">DimExpr</a>

<span class="keyword">context-free syntax</span>
  
  <a href="#Expression_26_40" id="Expression_19_3" title="Referenced at line 26">Expression</a> = <a href="#ArrayCreationExpression_13_3" id="ArrayCreationExpression_19_16" title="Defined at line 13, 20, 21">ArrayCreationExpression</a>
  <button class="modal-open" id="ArrayCreationExpression_20_3" title="Multi-file references" data-urls="#ArrayCreationExpression_19_16 line 19; ../ArrayAccess.sdf3/#ArrayCreationExpression_21_48 line 21">ArrayCreationExpression</button>.<span class="cons_Constructor"><span id="NewArray_20_27" title="Not referenced">NewArray</span></span> = &lt;<span class="cons_String">new</span> &lt;<a href="#ArrayBaseType_14_3" id="ArrayBaseType_20_44" title="Defined at line 14, 23, 24">ArrayBaseType</a>&gt;&lt;{<a href="#DimExpr_15_3" id="DimExpr_20_60" title="Defined at line 15, 26">DimExpr</a> <span class="cons_Lit">" "</span>}+&gt;&lt;<a href="../../types/ReferenceTypes.sdf3/#AnnotatedDimsEmpty_18_3" id="AnnotatedDimsEmpty_20_75" title="Defined at ../../types/ReferenceTypes.sdf3 line 18, 40">AnnotatedDimsEmpty</a>&gt;&gt;
  <button class="modal-open" id="ArrayCreationExpression_21_3" title="Multi-file references" data-urls="#ArrayCreationExpression_19_16 line 19; ../ArrayAccess.sdf3/#ArrayCreationExpression_21_48 line 21">ArrayCreationExpression</button>.<span class="cons_Constructor"><span id="NewArrayInit_21_27" title="Not referenced">NewArrayInit</span></span> = &lt;<span class="cons_String">new</span> &lt;<a href="#ArrayBaseType_14_3" id="ArrayBaseType_21_48" title="Defined at line 14, 23, 24">ArrayBaseType</a>&gt;&lt;<a href="../../types/ReferenceTypes.sdf3/#AnnotatedDims_17_3" id="AnnotatedDims_21_63" title="Defined at ../../types/ReferenceTypes.sdf3 line 17, 39">AnnotatedDims</a>&gt;&lt;<a href="../../arrays/ArrayInitializers.sdf3/#ArrayInitializer_10_3" id="ArrayInitializer_21_78" title="Defined at ../../arrays/ArrayInitializers.sdf3 line 10, 14, 15">ArrayInitializer</a>&gt;&gt;
  
  <a href="#ArrayBaseType_20_44" id="ArrayBaseType_23_3" title="Referenced at line 20, 21">ArrayBaseType</a> = <a href="../../types/ReferenceTypes.sdf3/#ClassType_14_3" id="ClassType_23_19" title="Defined at ../../types/ReferenceTypes.sdf3 line 14, 26, 27">ClassType</a>
  <a href="#ArrayBaseType_20_44" id="ArrayBaseType_24_3" title="Referenced at line 20, 21">ArrayBaseType</a> = <a href="../../types/PrimitiveTypes.sdf3/#PrimitiveType_10_3" id="PrimitiveType_24_19" title="Defined at ../../types/PrimitiveTypes.sdf3 line 10, 15, 16">PrimitiveType</a>
  
  <a href="#DimExpr_20_60" id="DimExpr_26_3" title="Referenced at line 20">DimExpr</a>.<span class="cons_Constructor"><span id="Dim_26_11" title="Not referenced">Dim</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_26_20" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">[</span>&lt;<a href="#Expression_19_3" id="Expression_26_40" title="Defined at line 19">Expression</a>&gt;<span class="cons_String">]</span>&gt;
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
