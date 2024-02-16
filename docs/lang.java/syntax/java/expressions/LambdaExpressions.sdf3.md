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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/expressions/LambdaExpressions_1_8" title="a definition with multiple references" data-urls="../Disambiguation.sdf3/#java/expressions/LambdaExpressions line 12_3; ../UnaryOperators.sdf3/#java/expressions/LambdaExpressions line 8_3">java/expressions/LambdaExpressions</button>

<span class="layout">// 15.27. Lambda Expressions</span>

<span class="keyword">imports</span>
  <a href="../../statements/Blocks.sdf3/#java/statements/Blocks_1_8" id="java/statements/Blocks_6_3" title="a reference to a single-file definition">java/statements/Blocks</a>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_7_3" title="a reference to a single-file definition">java/lexical/Identifiers</a>
  <a href="../../classes/MethodDeclarations.sdf3/#java/classes/MethodDeclarations_1_8" id="java/classes/MethodDeclarations_8_3" title="a reference to a single-file definition">java/classes/MethodDeclarations</a>
  
<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="LambdaParameters_12_3" title="a definition with multiple references" data-urls="#LambdaParameters line 16_44, 17_44">LambdaParameters</button>

<span class="keyword">context-free syntax</span>

  <a href="#Expression_16_66" id="Expression_16_3" title="a definition with a single reference">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#LambdaExpression_107_16" id="LambdaExpression_16_14" title="a definition with a single reference">LambdaExpression</a></span>          = [[<a href="#LambdaParameters_12_3" id="LambdaParameters_16_44" title="a reference to a single-file definition">LambdaParameters</a>] <span class="cons_String">-&gt;</span> [<a href="#Expression_16_3" id="Expression_16_66" title="a reference to a single-file definition">Expression</a>]]
  <a href="#Expression_16_66" id="Expression_17_3" title="a definition with a single reference">Expression</a>.<span class="cons_Constructor"><span id="LambdaExpressionWithBlock_17_14" title="a definition with no references">LambdaExpressionWithBlock</span></span> = [[<a href="#LambdaParameters_12_3" id="LambdaParameters_17_44" title="a reference to a single-file definition">LambdaParameters</a>] <span class="cons_String">-&gt;</span> [<a href="../../statements/Blocks.sdf3/#Block_12_3" id="Block_17_66" title="a reference to a single-file definition">Block</a>]]
  
  <button class="modal-open" id="LambdaParameters_19_3" title="a definition with multiple references" data-urls="#LambdaParameters line 16_44, 17_44">LambdaParameters</button>.<span class="cons_Constructor"><span id="SingleInferredParam_19_20" title="a definition with no references">SingleInferredParam</span></span> = <a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_19_42" title="a reference to a single-file definition">Id</a>
  <button class="modal-open" id="LambdaParameters_20_3" title="a definition with multiple references" data-urls="#LambdaParameters line 16_44, 17_44">LambdaParameters</button>.<span class="cons_Constructor"><span id="Params_20_20" title="a definition with no references">Params</span></span>              = &lt;<span class="cons_String">(</span>&lt;<a href="../../classes/MethodDeclarations.sdf3/#FormalParams_23_3" id="FormalParams_20_45" title="a reference to a single-file definition">FormalParams</a>&gt;<span class="cons_String">)</span>&gt;
  <button class="modal-open" id="LambdaParameters_21_3" title="a definition with multiple references" data-urls="#LambdaParameters line 16_44, 17_44">LambdaParameters</button>.<span class="cons_Constructor"><span id="InferredParams_21_20" title="a definition with no references">InferredParams</span></span>      = &lt;<span class="cons_String">(</span>&lt;{<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_21_46" title="a reference to a single-file definition">Id</a> <span class="cons_Lit">", "</span>}+&gt;<span class="cons_String">)</span>&gt;
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
