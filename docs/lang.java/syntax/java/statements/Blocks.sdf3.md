---
title: Blocks.sdf3
hide:
  - toc
---

# `Blocks.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/statements/Blocks.sdf3]

[pdmosses/java-front/lang.java/syntax/java/statements/Blocks.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/statements/Blocks.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Statements.sdf3#java/statements/Blocks_160_182" id="java/statements/Blocks_7_29" title="Referenced at ../Statements.sdf3 line 9">java/statements/Blocks</a>

<span class="layout">// 14.2. Blocks</span>

<span class="keyword">imports</span>
  <a href="../../classes/ClassDeclarations.sdf3#java/classes/ClassDeclarations_7_37" id="java/classes/ClassDeclarations_58_88" title="Defined at ../../classes/ClassDeclarations.sdf3 line 1">java/classes/ClassDeclarations</a>
  <a href="../LocalVariableDeclarations.sdf3#java/statements/LocalVariableDeclarations_7_48" id="java/statements/LocalVariableDeclarations_91_132" title="Defined at ../LocalVariableDeclarations.sdf3 line 1">java/statements/LocalVariableDeclarations</a>
  <a href="../Statements.sdf3#java/statements/Statements_7_33" id="java/statements/Statements_135_161" title="Defined at ../Statements.sdf3 line 1">java/statements/Statements</a>

<span class="keyword">context-free sorts</span>

  <a href="../Statements.sdf3#Block_3181_3186" id="Block_185_190" title="Referenced at ../Statements.sdf3 line 126; ../../classes/InstanceInitializers.sdf3 line 14; ../../classes/MethodDeclarations.sdf3 line 56; ../../classes/StaticInitializers.sdf3 line 14; ../../expressions/LambdaExpressions.sdf3 line 17">Block</a>
  <a href="#BlockStatement_260_274" id="BlockStatement_193_207" title="Referenced at line 19; ../Statements.sdf3 line 72; ../../classes/ConstructorDeclarations.sdf3 line 27">BlockStatement</a>

<span class="keyword">context-free syntax</span>
  
  <a href="../Statements.sdf3#Block_3181_3186" id="Block_234_239" title="Referenced at ../Statements.sdf3 line 126; ../../classes/InstanceInitializers.sdf3 line 14; ../../classes/MethodDeclarations.sdf3 line 56; ../../classes/StaticInitializers.sdf3 line 14; ../../expressions/LambdaExpressions.sdf3 line 17">Block</a>.<span class="cons_Constructor"><span id="Block_240_245" title="Not referenced locally, nor via imports">Block</span></span> = &lt;
  <span class="cons_String">{</span>
    &lt;{<a href="#BlockStatement_193_207" id="BlockStatement_260_274" title="Defined at line 13, 21, 22, 23">BlockStatement</a> <span class="cons_Lit">"\n"</span>}*&gt;
  <span class="cons_String">}</span>&gt;
  <a href="#BlockStatement_260_274" id="BlockStatement_290_304" title="Referenced at line 19; ../Statements.sdf3 line 72; ../../classes/ConstructorDeclarations.sdf3 line 27">BlockStatement</a> = <a href="../LocalVariableDeclarations.sdf3#LocalVariableDeclarationStatement_226_259" id="LocalVariableDeclarationStatement_307_340" title="Defined at ../LocalVariableDeclarations.sdf3 line 12, 17">LocalVariableDeclarationStatement</a>
  <a href="#BlockStatement_260_274" id="BlockStatement_343_357" title="Referenced at line 19; ../Statements.sdf3 line 72; ../../classes/ConstructorDeclarations.sdf3 line 27">BlockStatement</a>   = <a href="../../classes/ClassDeclarations.sdf3#ClassDeclaration_507_523" id="ClassDeclaration_362_378" title="Defined at ../../classes/ClassDeclarations.sdf3 line 22, 33, 34">ClassDeclaration</a>
  <a href="#BlockStatement_260_274" id="BlockStatement_381_395" title="Referenced at line 19; ../Statements.sdf3 line 72; ../../classes/ConstructorDeclarations.sdf3 line 27">BlockStatement</a>    = <a href="../Statements.sdf3#Statement_277_286" id="Statement_401_410" title="Defined at ../Statements.sdf3 line 16, 34, 36, 37, 39, 41, 42, 51, 53, 55, 57, 58, 59, 61, 62, 64, 79, 83, 84, 86, 87, 89, 90, 92, 94, 96, 100, 110, 114, 118, 123">Statement</a>
</code></pre></td></tr></tbody></table></div>