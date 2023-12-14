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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/expressions/LambdaExpressions_1_8" title="Multi-file references" data-urls="../Disambiguation.sdf3/#java/expressions/LambdaExpressions_12_3 line 12; ../UnaryOperators.sdf3/#java/expressions/LambdaExpressions_8_3 line 8">java/expressions/LambdaExpressions</button>

<span class="layout">// 15.27. Lambda Expressions</span>

<span class="keyword">imports</span>
  <a href="../../statements/Blocks.sdf3/#java/statements/Blocks_1_8" id="java/statements/Blocks_6_3" title="Defined at ../../statements/Blocks.sdf3 line 1">java/statements/Blocks</a>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_7_3" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../../classes/MethodDeclarations.sdf3/#java/classes/MethodDeclarations_1_8" id="java/classes/MethodDeclarations_8_3" title="Defined at ../../classes/MethodDeclarations.sdf3 line 1">java/classes/MethodDeclarations</a>
  
<span class="keyword">context-free sorts</span>

  <a href="#LambdaParameters_16_44" id="LambdaParameters_12_3" title="Referenced at line 16, 17">LambdaParameters</a>

<span class="keyword">context-free syntax</span>

  <a href="#Expression_16_66" id="Expression_16_3" title="Referenced at line 16">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#LambdaExpression_107_16" id="LambdaExpression_16_14" title="Referenced at ../Disambiguation.sdf3 line 107">LambdaExpression</a></span>          = [[<a href="#LambdaParameters_12_3" id="LambdaParameters_16_44" title="Defined at line 12, 19, 20, 21">LambdaParameters</a>] <span class="cons_String">-&gt;</span> [<a href="#Expression_16_3" id="Expression_16_66" title="Defined at line 16, 17">Expression</a>]]
  <a href="#Expression_16_66" id="Expression_17_3" title="Referenced at line 16">Expression</a>.<span class="cons_Constructor"><span id="LambdaExpressionWithBlock_17_14" title="Not referenced">LambdaExpressionWithBlock</span></span> = [[<a href="#LambdaParameters_12_3" id="LambdaParameters_17_44" title="Defined at line 12, 19, 20, 21">LambdaParameters</a>] <span class="cons_String">-&gt;</span> [<a href="../../statements/Blocks.sdf3/#Block_12_3" id="Block_17_66" title="Defined at ../../statements/Blocks.sdf3 line 12, 17">Block</a>]]
  
  <a href="#LambdaParameters_16_44" id="LambdaParameters_19_3" title="Referenced at line 16, 17">LambdaParameters</a>.<span class="cons_Constructor"><span id="SingleInferredParam_19_20" title="Not referenced">SingleInferredParam</span></span> = <a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_19_42" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>
  <a href="#LambdaParameters_16_44" id="LambdaParameters_20_3" title="Referenced at line 16, 17">LambdaParameters</a>.<span class="cons_Constructor"><span id="Params_20_20" title="Not referenced">Params</span></span>              = &lt;<span class="cons_String">(</span>&lt;<a href="../../classes/MethodDeclarations.sdf3/#FormalParams_23_3" id="FormalParams_20_45" title="Defined at ../../classes/MethodDeclarations.sdf3 line 23, 62, 63, 64, 65, 66">FormalParams</a>&gt;<span class="cons_String">)</span>&gt;
  <a href="#LambdaParameters_16_44" id="LambdaParameters_21_3" title="Referenced at line 16, 17">LambdaParameters</a>.<span class="cons_Constructor"><span id="InferredParams_21_20" title="Not referenced">InferredParams</span></span>      = &lt;<span class="cons_String">(</span>&lt;{<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_21_46" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a> <span class="cons_Lit">", "</span>}+&gt;<span class="cons_String">)</span>&gt;
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
