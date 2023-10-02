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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/expressions/MethodReference_279_311" id="java/expressions/MethodReference_7_39" title="Referenced at ../Main.sdf3 line 13">java/expressions/MethodReference</a>

<span class="layout">// 15.13. Method Reference Expressions</span>

<span class="keyword">imports</span>
  <a href="../../types/ReferenceTypes.sdf3#java/types/ReferenceTypes_7_32" id="java/types/ReferenceTypes_91_116" title="Defined at ../../types/ReferenceTypes.sdf3 line 1">java/types/ReferenceTypes</a>
  <a href="../../types/ParameterizedTypes.sdf3#java/types/ParameterizedTypes_7_36" id="java/types/ParameterizedTypes_119_148" title="Defined at ../../types/ParameterizedTypes.sdf3 line 1">java/types/ParameterizedTypes</a>
  <a href="../../lexical/Identifiers.sdf3#java/lexical/Identifiers_7_31" id="java/lexical/Identifiers_151_175" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../../names/Names.sdf3#java/names/Names_7_23" id="java/names/Names_178_194" title="Defined at ../../names/Names.sdf3 line 1">java/names/Names</a>
  <a href="../UnaryOperators.sdf3#java/expressions/UnaryOperators_7_38" id="java/expressions/UnaryOperators_197_228" title="Defined at ../UnaryOperators.sdf3 line 1">java/expressions/UnaryOperators</a>

<span class="keyword">context-free syntax</span>
  
  <a href="#Expression_820_830" id="Expression_255_265" title="Referenced at line 23">Expression</a>.<span class="cons_Constructor"><span id="MethodReferenceRType_266_286" title="Not referenced locally, nor via imports">MethodReferenceRType</span></span>  = &lt;&lt;<a href="../../types/ReferenceTypes.sdf3#ReferenceType_218_231" id="ReferenceType_292_305" title="Defined at ../../types/ReferenceTypes.sdf3 line 13, 23, 24">ReferenceType</a>&gt;<span class="cons_String">::</span>&lt;<a href="../../types/ParameterizedTypes.sdf3#TypeArguments_157_170" id="TypeArguments_309_322" title="Defined at ../../types/ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>?&gt;&lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_325_327" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  <a href="#Expression_820_830" id="Expression_332_342" title="Referenced at line 23">Expression</a>.<span class="cons_Constructor"><a href="#MethodReferenceExpr_797_816" id="MethodReferenceExpr_343_362" title="Referenced at line 23">MethodReferenceExpr</a></span>   = &lt;&lt;<a href="#Expression_255_265" id="Expression_369_379" title="Defined at line 14, 15, 16, 17, 18, 19, 22">Expression</a>&gt;<span class="cons_String">::</span>&lt;<a href="../../types/ParameterizedTypes.sdf3#TypeArguments_157_170" id="TypeArguments_383_396" title="Defined at ../../types/ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>?&gt;&lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_399_401" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  <a href="#Expression_820_830" id="Expression_406_416" title="Referenced at line 23">Expression</a>.<span class="cons_Constructor"><span id="MethodReferenceSuper_417_437" title="Not referenced locally, nor via imports">MethodReferenceSuper</span></span>  = &lt;<span class="cons_String">super::</span>&lt;<a href="../../types/ParameterizedTypes.sdf3#TypeArguments_157_170" id="TypeArguments_450_463" title="Defined at ../../types/ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>?&gt;&lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_466_468" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  <a href="#Expression_820_830" id="Expression_473_483" title="Referenced at line 23">Expression</a>.<span class="cons_Constructor"><span id="MethodReferenceQSuper_484_505" title="Not referenced locally, nor via imports">MethodReferenceQSuper</span></span> = &lt;&lt;<a href="../../names/Names.sdf3#TypeName_145_153" id="TypeName_510_518" title="Defined at ../../names/Names.sdf3 line 11, 21, 22">TypeName</a>&gt;<span class="cons_String">.super::</span>&lt;<a href="../../types/ParameterizedTypes.sdf3#TypeArguments_157_170" id="TypeArguments_528_541" title="Defined at ../../types/ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>?&gt;&lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_544_546" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  <a href="#Expression_820_830" id="Expression_551_561" title="Referenced at line 23">Expression</a>.<span class="cons_Constructor"><span id="MethodReferenceCType_562_582" title="Not referenced locally, nor via imports">MethodReferenceCType</span></span> = &lt;&lt;<a href="../../types/ReferenceTypes.sdf3#ClassType_234_243" id="ClassType_587_596" title="Defined at ../../types/ReferenceTypes.sdf3 line 14, 26, 27">ClassType</a>&gt;<span class="cons_String">::</span>&lt;<a href="../../types/ParameterizedTypes.sdf3#TypeArguments_157_170" id="TypeArguments_600_613" title="Defined at ../../types/ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>?&gt; <span class="cons_String">new</span>&gt;
  <a href="#Expression_820_830" id="Expression_623_633" title="Referenced at line 23">Expression</a>.<span class="cons_Constructor"><span id="MethodReferenceAType_634_654" title="Not referenced locally, nor via imports">MethodReferenceAType</span></span> = &lt;&lt;<a href="../../types/ReferenceTypes.sdf3#ArrayType_261_270" id="ArrayType_659_668" title="Defined at ../../types/ReferenceTypes.sdf3 line 16, 37, 38">ArrayType</a>&gt;<span class="cons_String">::</span>&lt;<a href="../../types/ParameterizedTypes.sdf3#TypeArguments_157_170" id="TypeArguments_672_685" title="Defined at ../../types/ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>?&gt; <span class="cons_String">new</span>&gt;
  
<span class="keyword">context-free priorities</span>
  <a href="#Expression_255_265" id="Expression_722_732" title="Defined at line 14, 15, 16, 17, 18, 19, 22">Expression</a>.<span class="cons_Constructor"><a href="#MethodReferenceExpr_343_362" id="MethodReferenceExpr_733_752" title="Defined at line 15">MethodReferenceExpr</a></span> &gt; <a href="#Expression_820_830" id="Expression_755_765" title="Referenced at line 23">Expression</a> = <a href="../../names/Names.sdf3#ExpressionName_176_190" id="ExpressionName_768_782" title="Defined at ../../names/Names.sdf3 line 13, 25, 26">ExpressionName</a>,
  <a href="#Expression_255_265" id="Expression_786_796" title="Defined at line 14, 15, 16, 17, 18, 19, 22">Expression</a>.<span class="cons_Constructor"><a href="#MethodReferenceExpr_343_362" id="MethodReferenceExpr_797_816" title="Defined at line 15">MethodReferenceExpr</a></span> &gt;  <a href="#Expression_255_265" id="Expression_820_830" title="Defined at line 14, 15, 16, 17, 18, 19, 22">Expression</a>.<span class="cons_Constructor"><a href="../UnaryOperators.sdf3#CastReference_545_558" id="CastReference_831_844" title="Defined at ../UnaryOperators.sdf3 line 23">CastReference</a></span>
  
<span class="keyword">template options</span>
  
  <span class="keyword">tokenize</span> : "::"  
</code></pre></td></tr></tbody></table></div>