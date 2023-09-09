---
title: PrimaryExpressions.sdf3
---

# `PrimaryExpressions.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/expressions/PrimaryExpressions.sdf3]

[pdmosses/java-front/lang.java/syntax/java/expressions/PrimaryExpressions.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/expressions/PrimaryExpressions.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Main.sdf3#java/expressions/PrimaryExpressions_69_104" id="java/expressions/PrimaryExpressions_7_42" title="Referenced at ../Main.sdf3 line 7">java/expressions/PrimaryExpressions</a>

<span class="layout">// 15.8. Primary Expressions</span>

<span class="keyword">imports</span>
  <a href="../../literals/Main.sdf3#java/literals/Main_7_25" id="java/literals/Main_84_102" title="Defined at ../../literals/Main.sdf3 line 1">java/literals/Main</a>
  <a href="../../names/Names.sdf3#java/names/Names_7_23" id="java/names/Names_105_121" title="Defined at ../../names/Names.sdf3 line 1">java/names/Names</a>
  <a href="../../types/PrimitiveTypes.sdf3#java/types/PrimitiveTypes_7_32" id="java/types/PrimitiveTypes_124_149" title="Defined at ../../types/PrimitiveTypes.sdf3 line 1">java/types/PrimitiveTypes</a>
  
<span class="keyword">context-free sorts</span>

  <a href="#ClassLiteral_257_269" id="ClassLiteral_175_187" title="Referenced at line 18">ClassLiteral</a>
  <a href="#Dims_568_572" id="Dims_190_194" title="Referenced at line 25">Dims</a>

<span class="keyword">context-free syntax</span>
  
  <a href="#Expression_354_364" id="Expression_221_231" title="Referenced at line 21">Expression</a> = <a href="../../literals/Main.sdf3#Literal_274_281" id="Literal_234_241" title="Defined at ../../literals/Main.sdf3 line 15, 19, 20, 21, 22, 23, 24">Literal</a>
  <a href="#Expression_354_364" id="Expression_244_254" title="Referenced at line 21">Expression</a> = <a href="#ClassLiteral_175_187" id="ClassLiteral_257_269" title="Defined at line 12, 23, 24, 25, 26">ClassLiteral</a>
  <a href="#Expression_354_364" id="Expression_272_282" title="Referenced at line 21">Expression</a>.<span class="cons_Constructor"><span id="This_283_287" title="Not referenced locally, nor via imports">This</span></span> = <span class="cons_Lit">"this"</span>
  <a href="#Expression_354_364" id="Expression_299_309" title="Referenced at line 21">Expression</a>.<span class="cons_Constructor"><span id="QThis_310_315" title="Not referenced locally, nor via imports">QThis</span></span> = &lt;&lt;<a href="../../names/Names.sdf3#TypeName_145_153" id="TypeName_320_328" title="Defined at ../../names/Names.sdf3 line 11, 21, 22">TypeName</a>&gt;<span class="cons_String">.this</span>&gt;
  <a href="#Expression_354_364" id="Expression_338_348" title="Referenced at line 21">Expression</a> = &lt;<span class="cons_String">(</span>&lt;<a href="#Expression_221_231" id="Expression_354_364" title="Defined at line 17, 18, 19, 20, 21">Expression</a>&gt;<span class="cons_String">)</span>&gt; {<span class="keyword">bracket</span>}
  
  <a href="#ClassLiteral_257_269" id="ClassLiteral_383_395" title="Referenced at line 18">ClassLiteral</a>.<span class="cons_Constructor"><span id="TypeNameClassLiteral_396_416" title="Not referenced locally, nor via imports">TypeNameClassLiteral</span></span>    = &lt;&lt;<a href="../../names/Names.sdf3#TypeName_145_153" id="TypeName_424_432" title="Defined at ../../names/Names.sdf3 line 11, 21, 22">TypeName</a>&gt;&lt;<a href="#Dims_190_194" id="Dims_434_438" title="Defined at line 13, 28">Dims</a>*&gt;<span class="cons_String">.class</span>&gt;
  <a href="#ClassLiteral_257_269" id="ClassLiteral_450_462" title="Referenced at line 18">ClassLiteral</a>.<span class="cons_Constructor"><span id="NumericTypeClassLiteral_463_486" title="Not referenced locally, nor via imports">NumericTypeClassLiteral</span></span> = &lt;&lt;<a href="../../types/PrimitiveTypes.sdf3#NumericType_147_158" id="NumericType_491_502" title="Defined at ../../types/PrimitiveTypes.sdf3 line 11, 17, 18, 19, 20, 21, 22, 23">NumericType</a>&gt;&lt;<a href="#Dims_190_194" id="Dims_504_508" title="Defined at line 13, 28">Dims</a>*&gt;<span class="cons_String">.class</span>&gt;
  <a href="#ClassLiteral_257_269" id="ClassLiteral_520_532" title="Referenced at line 18">ClassLiteral</a>.<span class="cons_Constructor"><span id="BooleanClassLiteral_533_552" title="Not referenced locally, nor via imports">BooleanClassLiteral</span></span>     = &lt;<span class="cons_String">boolean</span>&lt;<a href="#Dims_190_194" id="Dims_568_572" title="Defined at line 13, 28">Dims</a>*&gt;<span class="cons_String">.class</span>&gt;
  <a href="#ClassLiteral_257_269" id="ClassLiteral_584_596" title="Referenced at line 18">ClassLiteral</a>.<span class="cons_Constructor"><span id="VoidClassLiteral_597_613" title="Not referenced locally, nor via imports">VoidClassLiteral</span></span>        = &lt;<span class="cons_String">void.class</span>&gt;
  
  <a href="#Dims_568_572" id="Dims_641_645" title="Referenced at line 25">Dims</a>.<span class="cons_Constructor"><span id="Dimension_646_655" title="Not referenced locally, nor via imports">Dimension</span></span> = &lt;<span class="cons_String">[]</span>&gt;

<span class="keyword">template options</span>

  <span class="keyword">tokenize</span> : ".["
  
  

  
</code></pre></td></tr></tbody></table></div>