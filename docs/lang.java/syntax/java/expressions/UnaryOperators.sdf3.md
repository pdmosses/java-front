---
title: UnaryOperators.sdf3
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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../MethodReference.sdf3#java/expressions/UnaryOperators_197_228" id="java/expressions/UnaryOperators_7_38" title="Referenced at ../MethodReference.sdf3 line 10">java/expressions/UnaryOperators</a>

<span class="layout">// 15.15. Unary Operators</span>

<span class="keyword">imports</span>
  <a href="../../types/PrimitiveTypes.sdf3#java/types/PrimitiveTypes_7_32" id="java/types/PrimitiveTypes_77_102" title="Defined at ../../types/PrimitiveTypes.sdf3 line 1">java/types/PrimitiveTypes</a>
  <a href="../../types/ReferenceTypes.sdf3#java/types/ReferenceTypes_7_32" id="java/types/ReferenceTypes_105_130" title="Defined at ../../types/ReferenceTypes.sdf3 line 1">java/types/ReferenceTypes</a>
  <a href="../LambdaExpressions.sdf3#java/expressions/LambdaExpressions_7_41" id="java/expressions/LambdaExpressions_133_167" title="Defined at ../LambdaExpressions.sdf3 line 1">java/expressions/LambdaExpressions</a> 

<span class="keyword">context-free sorts</span>

  <a href="#AdditionalBound_581_596" id="AdditionalBound_192_207" title="Referenced at line 23">AdditionalBound</a>

<span class="keyword">context-free syntax</span>
  
  <a href="#Expression_606_616" id="Expression_234_244" title="Referenced at line 23">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#Plus_1318_1322" id="Plus_245_249" title="Referenced at ../Disambiguation.sdf3 line 64">Plus</a></span>  = &lt;<span class="cons_String">+</span>&lt;<a href="#Expression_234_244" id="Expression_256_266" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>&gt;&gt;
  <a href="#Expression_606_616" id="Expression_271_281" title="Referenced at line 23">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#Minus_1339_1344" id="Minus_282_287" title="Referenced at ../Disambiguation.sdf3 line 65">Minus</a></span> = &lt;<span class="cons_String">-</span>&lt;<a href="#Expression_234_244" id="Expression_293_303" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>&gt;&gt;
  <a href="#Expression_606_616" id="Expression_308_318" title="Referenced at line 23">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#PreIncr_1270_1277" id="PreIncr_319_326" title="Referenced at ../Disambiguation.sdf3 line 62">PreIncr</a></span> = &lt;<span class="cons_String">++</span>&lt;<a href="#Expression_234_244" id="Expression_333_343" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>&gt;&gt;
  <a href="#Expression_606_616" id="Expression_348_358" title="Referenced at line 23">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#PreDecr_1294_1301" id="PreDecr_359_366" title="Referenced at ../Disambiguation.sdf3 line 63">PreDecr</a></span> = &lt;<span class="cons_String">--</span>&lt;<a href="#Expression_234_244" id="Expression_373_383" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>&gt;&gt;
  <a href="#Expression_606_616" id="Expression_388_398" title="Referenced at line 23">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#Complement_1361_1371" id="Complement_399_409" title="Referenced at ../Disambiguation.sdf3 line 66">Complement</a></span> = &lt;<span class="cons_String">~</span>&lt;<a href="#Expression_234_244" id="Expression_415_425" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>&gt;&gt;
  <a href="#Expression_606_616" id="Expression_430_440" title="Referenced at line 23">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#Not_1388_1391" id="Not_441_444" title="Referenced at ../Disambiguation.sdf3 line 67">Not</a></span>        = &lt;<span class="cons_String">!</span>&lt;<a href="#Expression_234_244" id="Expression_457_467" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>&gt;&gt;
  <a href="#Expression_606_616" id="Expression_472_482" title="Referenced at line 23">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#CastPrimitive_750_763" id="CastPrimitive_483_496" title="Referenced at ../Disambiguation.sdf3 line 35">CastPrimitive</a></span> = &lt;<span class="cons_String">(</span>&lt;<a href="../../types/PrimitiveTypes.sdf3#PrimitiveType_131_144" id="PrimitiveType_502_515" title="Defined at ../../types/PrimitiveTypes.sdf3 line 10, 15, 16">PrimitiveType</a>&gt;<span class="cons_String">)</span> &lt;<a href="#Expression_234_244" id="Expression_519_529" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>&gt;&gt;
  <a href="#Expression_606_616" id="Expression_534_544" title="Referenced at line 23">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3#CastReference_1003_1016" id="CastReference_545_558" title="Referenced at ../Disambiguation.sdf3 line 49; ../MethodReference.sdf3 line 23">CastReference</a></span> = &lt;<span class="cons_String">(</span>&lt;<a href="../../types/ReferenceTypes.sdf3#ReferenceType_218_231" id="ReferenceType_564_577" title="Defined at ../../types/ReferenceTypes.sdf3 line 13, 23, 24">ReferenceType</a>&gt; &lt;{<a href="#AdditionalBound_192_207" id="AdditionalBound_581_596" title="Defined at line 12, 24">AdditionalBound</a> <span class="cons_Lit">" "</span>}*&gt;<span class="cons_String">)</span> &lt;<a href="#Expression_234_244" id="Expression_606_616" title="Defined at line 16, 17, 18, 19, 20, 21, 22, 23">Expression</a>&gt;&gt;
  <a href="#AdditionalBound_581_596" id="AdditionalBound_621_636" title="Referenced at line 23">AdditionalBound</a>.<span class="cons_Constructor"><span id="AdditionalBound_637_652" title="Not referenced locally, nor via imports">AdditionalBound</span></span> = &lt;<span class="cons_String">&amp;</span> &lt;<a href="../../types/ReferenceTypes.sdf3#ClassType_234_243" id="ClassType_659_668" title="Defined at ../../types/ReferenceTypes.sdf3 line 14, 26, 27">ClassType</a>&gt;&gt;
  
</code></pre></td></tr></tbody></table></div>