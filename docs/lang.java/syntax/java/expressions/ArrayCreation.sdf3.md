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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/expressions/ArrayCreation_148_178" id="java/expressions/ArrayCreation_7_37" title="Referenced at ../Main.sdf3 line 9">java/expressions/ArrayCreation</a>

<span class="layout">// 15.10.1. Array Creation Expressions</span>

<span class="keyword">imports</span>
  <a href="../../types/ReferenceTypes.sdf3#java/types/ReferenceTypes_7_32" id="java/types/ReferenceTypes_89_114" title="Defined at ../../types/ReferenceTypes.sdf3 line 1">java/types/ReferenceTypes</a>
  <a href="../../types/PrimitiveTypes.sdf3#java/types/PrimitiveTypes_7_32" id="java/types/PrimitiveTypes_117_142" title="Defined at ../../types/PrimitiveTypes.sdf3 line 1">java/types/PrimitiveTypes</a>
  <a href="../../interfaces/Annotations.sdf3#java/interfaces/Annotations_7_34" id="java/interfaces/Annotations_145_172" title="Defined at ../../interfaces/Annotations.sdf3 line 1">java/interfaces/Annotations</a>
  <a href="../../arrays/ArrayInitializers.sdf3#java/arrays/ArrayInitializers_7_36" id="java/arrays/ArrayInitializers_175_204" title="Defined at ../../arrays/ArrayInitializers.sdf3 line 1">java/arrays/ArrayInitializers</a>

<span class="keyword">context-free sorts</span>

  <a href="#ArrayCreationExpression_317_340" id="ArrayCreationExpression_228_251" title="Referenced at line 19; ../ArrayAccess.sdf3 line 21">ArrayCreationExpression</a>
  <a href="#ArrayBaseType_483_496" id="ArrayBaseType_254_267" title="Referenced at line 21">ArrayBaseType</a>
  <a href="#DimExpr_400_407" id="DimExpr_270_277" title="Referenced at line 20">DimExpr</a>

<span class="keyword">context-free syntax</span>
  
  <a href="#Expression_637_647" id="Expression_304_314" title="Referenced at line 26">Expression</a> = <a href="#ArrayCreationExpression_228_251" id="ArrayCreationExpression_317_340" title="Defined at line 13, 20, 21">ArrayCreationExpression</a>
  <a href="#ArrayCreationExpression_317_340" id="ArrayCreationExpression_343_366" title="Referenced at line 19; ../ArrayAccess.sdf3 line 21">ArrayCreationExpression</a>.<span class="cons_Constructor"><span id="NewArray_367_375" title="Not referenced locally, nor via imports">NewArray</span></span> = &lt;<span class="cons_String">new</span> &lt;<a href="#ArrayBaseType_254_267" id="ArrayBaseType_384_397" title="Defined at line 14, 23, 24">ArrayBaseType</a>&gt;&lt;{<a href="#DimExpr_270_277" id="DimExpr_400_407" title="Defined at line 15, 26">DimExpr</a> <span class="cons_Lit">" "</span>}+&gt;&lt;<a href="../../types/ReferenceTypes.sdf3#AnnotatedDimsEmpty_289_307" id="AnnotatedDimsEmpty_415_433" title="Defined at ../../types/ReferenceTypes.sdf3 line 18, 40">AnnotatedDimsEmpty</a>&gt;&gt;
  <a href="#ArrayCreationExpression_317_340" id="ArrayCreationExpression_438_461" title="Referenced at line 19; ../ArrayAccess.sdf3 line 21">ArrayCreationExpression</a>.<span class="cons_Constructor"><span id="NewArrayInit_462_474" title="Not referenced locally, nor via imports">NewArrayInit</span></span> = &lt;<span class="cons_String">new</span> &lt;<a href="#ArrayBaseType_254_267" id="ArrayBaseType_483_496" title="Defined at line 14, 23, 24">ArrayBaseType</a>&gt;&lt;<a href="../../types/ReferenceTypes.sdf3#AnnotatedDims_273_286" id="AnnotatedDims_498_511" title="Defined at ../../types/ReferenceTypes.sdf3 line 17, 39">AnnotatedDims</a>&gt;&lt;<a href="../../arrays/ArrayInitializers.sdf3#ArrayInitializer_133_149" id="ArrayInitializer_513_529" title="Defined at ../../arrays/ArrayInitializers.sdf3 line 10, 14, 15">ArrayInitializer</a>&gt;&gt;
  
  <a href="#ArrayBaseType_483_496" id="ArrayBaseType_537_550" title="Referenced at line 21">ArrayBaseType</a> = <a href="../../types/ReferenceTypes.sdf3#ClassType_234_243" id="ClassType_553_562" title="Defined at ../../types/ReferenceTypes.sdf3 line 14, 26, 27">ClassType</a>
  <a href="#ArrayBaseType_483_496" id="ArrayBaseType_565_578" title="Referenced at line 21">ArrayBaseType</a> = <a href="../../types/PrimitiveTypes.sdf3#PrimitiveType_131_144" id="PrimitiveType_581_594" title="Defined at ../../types/PrimitiveTypes.sdf3 line 10, 15, 16">PrimitiveType</a>
  
  <a href="#DimExpr_400_407" id="DimExpr_600_607" title="Referenced at line 20">DimExpr</a>.<span class="cons_Constructor"><span id="Dim_608_611" title="Not referenced locally, nor via imports">Dim</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3#Annotation_158_168" id="Annotation_617_627" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">[</span>&lt;<a href="#Expression_304_314" id="Expression_637_647" title="Defined at line 19">Expression</a>&gt;<span class="cons_String">]</span>&gt;
</code></pre></td></tr></tbody></table></div>