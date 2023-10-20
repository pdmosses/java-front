---
title: LocalVariableDeclarations.sdf3
hide:
  - toc
---

# `LocalVariableDeclarations.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/statements/LocalVariableDeclarations.sdf3]

[pdmosses/java-front/lang.java/syntax/java/statements/LocalVariableDeclarations.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/statements/LocalVariableDeclarations.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Blocks.sdf3/#java/statements/LocalVariableDeclarations_91_132" id="java/statements/LocalVariableDeclarations_7_48" title="Referenced at ../Blocks.sdf3 line 7; ../Main.sdf3 line 7">java/statements/LocalVariableDeclarations</a>

<span class="layout">// 14.4. Local Variable Declaration Statements</span>

<span class="keyword">imports</span>
  <a href="../../classes/FieldDeclarations.sdf3/#java/classes/FieldDeclarations_7_37" id="java/classes/FieldDeclarations_108_138" title="Defined at ../../classes/FieldDeclarations.sdf3 line 1">java/classes/FieldDeclarations</a>
  <a href="../../classes/MethodDeclarations.sdf3/#java/classes/MethodDeclarations_7_38" id="java/classes/MethodDeclarations_141_172" title="Defined at ../../classes/MethodDeclarations.sdf3 line 1">java/classes/MethodDeclarations</a>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_7_34" id="java/interfaces/Annotations_175_202" title="Defined at ../../interfaces/Annotations.sdf3 line 1">java/interfaces/Annotations</a>

<span class="keyword">context-free sorts</span>

  <a href="../Blocks.sdf3/#LocalVariableDeclarationStatement_307_340" id="LocalVariableDeclarationStatement_226_259" title="Referenced at ../Blocks.sdf3 line 21">LocalVariableDeclarationStatement</a>
  <a href="#LocalVariableDeclaration_363_387" id="LocalVariableDeclaration_262_286" title="Referenced at line 17">LocalVariableDeclaration</a>

<span class="keyword">context-free syntax</span>

  <a href="../Blocks.sdf3/#LocalVariableDeclarationStatement_307_340" id="LocalVariableDeclarationStatement_311_344" title="Referenced at ../Blocks.sdf3 line 21">LocalVariableDeclarationStatement</a>.<span class="cons_Constructor"><span id="LocVarDeclStm_345_358" title="Not referenced locally, nor via imports">LocVarDeclStm</span></span> = &lt;&lt;<a href="#LocalVariableDeclaration_262_286" id="LocalVariableDeclaration_363_387" title="Defined at line 13, 18">LocalVariableDeclaration</a>&gt;<span class="cons_String">;</span>&gt; <span class="layout">//{prefer}</span>
  <a href="#LocalVariableDeclaration_363_387" id="LocalVariableDeclaration_404_428" title="Referenced at line 17">LocalVariableDeclaration</a>.<span class="cons_Constructor"><span id="LocalVarDecl_429_441" title="Not referenced locally, nor via imports">LocalVarDecl</span></span> = &lt;
  &lt;{<a href="../../classes/MethodDeclarations.sdf3/#VariableModifier_462_478" id="VariableModifier_450_466" title="Defined at ../../classes/MethodDeclarations.sdf3 line 26, 73, 74">VariableModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../classes/FieldDeclarations.sdf3/#UnannType_403_412" id="UnannType_475_484" title="Defined at ../../classes/FieldDeclarations.sdf3 line 22, 50, 51">UnannType</a>&gt; &lt;{<a href="../../classes/FieldDeclarations.sdf3/#VarDecl_355_362" id="VarDecl_488_495" title="Defined at ../../classes/FieldDeclarations.sdf3 line 19, 33, 34">VarDecl</a> <span class="cons_Lit">", "</span>}+&gt;&gt; {<span class="keyword">prefer</span>}

</code></pre></td></tr></tbody></table></div>