---
title: LambdaExpressions.sdf3
hide:
  - toc
---

# `LambdaExpressions.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/expressions/LambdaExpressions.sdf3]

[pdmosses/java-front/lang.java/syntax/java/expressions/LambdaExpressions.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/expressions/LambdaExpressions.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Disambiguation.sdf3/#java/expressions/LambdaExpressions_324_358" id="java/expressions/LambdaExpressions_7_41" title="Referenced at ../Disambiguation.sdf3 line 12; ../UnaryOperators.sdf3 line 8">java/expressions/LambdaExpressions</a>

<span class="layout">// 15.27. Lambda Expressions</span>

<span class="keyword">imports</span>
  <a href="../../statements/Blocks.sdf3/#java/statements/Blocks_7_29" id="java/statements/Blocks_83_105" title="Defined at ../../statements/Blocks.sdf3 line 1">java/statements/Blocks</a>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_7_31" id="java/lexical/Identifiers_108_132" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../../classes/MethodDeclarations.sdf3/#java/classes/MethodDeclarations_7_38" id="java/classes/MethodDeclarations_135_166" title="Defined at ../../classes/MethodDeclarations.sdf3 line 1">java/classes/MethodDeclarations</a>
  
<span class="keyword">context-free sorts</span>

  <a href="#LambdaParameters_274_290" id="LambdaParameters_192_208" title="Referenced at line 16, 17">LambdaParameters</a>

<span class="keyword">context-free syntax</span>

  <a href="#Expression_296_306" id="Expression_233_243" title="Referenced at line 16">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#LambdaExpression_2256_2272" id="LambdaExpression_244_260" title="Referenced at ../Disambiguation.sdf3 line 107">LambdaExpression</a></span>          = [[<a href="#LambdaParameters_192_208" id="LambdaParameters_274_290" title="Defined at line 12, 19, 20, 21">LambdaParameters</a>] <span class="cons_String">-&gt;</span> [<a href="#Expression_233_243" id="Expression_296_306" title="Defined at line 16, 17">Expression</a>]]
  <a href="#Expression_296_306" id="Expression_311_321" title="Referenced at line 16">Expression</a>.<span class="cons_Constructor"><span id="LambdaExpressionWithBlock_322_347" title="Not referenced locally, nor via imports">LambdaExpressionWithBlock</span></span> = [[<a href="#LambdaParameters_192_208" id="LambdaParameters_352_368" title="Defined at line 12, 19, 20, 21">LambdaParameters</a>] <span class="cons_String">-&gt;</span> [<a href="../../statements/Blocks.sdf3/#Block_185_190" id="Block_374_379" title="Defined at ../../statements/Blocks.sdf3 line 12, 17">Block</a>]]
  
  <a href="#LambdaParameters_274_290" id="LambdaParameters_387_403" title="Referenced at line 16, 17">LambdaParameters</a>.<span class="cons_Constructor"><span id="SingleInferredParam_404_423" title="Not referenced locally, nor via imports">SingleInferredParam</span></span> = <a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_426_428" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>
  <a href="#LambdaParameters_274_290" id="LambdaParameters_431_447" title="Referenced at line 16, 17">LambdaParameters</a>.<span class="cons_Constructor"><span id="Params_448_454" title="Not referenced locally, nor via imports">Params</span></span>              = &lt;<span class="cons_String">(</span>&lt;<a href="../../classes/MethodDeclarations.sdf3/#FormalParams_415_427" id="FormalParams_473_485" title="Defined at ../../classes/MethodDeclarations.sdf3 line 23, 62, 63, 64, 65, 66">FormalParams</a>&gt;<span class="cons_String">)</span>&gt;
  <a href="#LambdaParameters_274_290" id="LambdaParameters_491_507" title="Referenced at line 16, 17">LambdaParameters</a>.<span class="cons_Constructor"><span id="InferredParams_508_522" title="Not referenced locally, nor via imports">InferredParams</span></span>      = &lt;<span class="cons_String">(</span>&lt;{<a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_534_536" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a> <span class="cons_Lit">", "</span>}+&gt;<span class="cons_String">)</span>&gt;
</code></pre></td></tr></tbody></table></div>