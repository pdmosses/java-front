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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/statements/LocalVariableDeclarations_1_8" title="a definition with multiple references" data-urls="../Blocks.sdf3/#java/statements/LocalVariableDeclarations line 7_3; ../Main.sdf3/#java/statements/LocalVariableDeclarations line 7_3">java/statements/LocalVariableDeclarations</button>

<span class="layout">// 14.4. Local Variable Declaration Statements</span>

<span class="keyword">imports</span>
  <a href="../../classes/FieldDeclarations.sdf3/#java/classes/FieldDeclarations_1_8" id="java/classes/FieldDeclarations_6_3" title="a reference to a single-file definition">java/classes/FieldDeclarations</a>
  <a href="../../classes/MethodDeclarations.sdf3/#java/classes/MethodDeclarations_1_8" id="java/classes/MethodDeclarations_7_3" title="a reference to a single-file definition">java/classes/MethodDeclarations</a>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_1_8" id="java/interfaces/Annotations_8_3" title="a reference to a single-file definition">java/interfaces/Annotations</a>

<span class="keyword">context-free sorts</span>

  <a href="../Blocks.sdf3/#LocalVariableDeclarationStatement_21_20" id="LocalVariableDeclarationStatement_12_3" title="a definition with a single reference">LocalVariableDeclarationStatement</a>
  <a href="#LocalVariableDeclaration_17_55" id="LocalVariableDeclaration_13_3" title="a definition with a single reference">LocalVariableDeclaration</a>

<span class="keyword">context-free syntax</span>

  <a href="../Blocks.sdf3/#LocalVariableDeclarationStatement_21_20" id="LocalVariableDeclarationStatement_17_3" title="a definition with a single reference">LocalVariableDeclarationStatement</a>.<span class="cons_Constructor"><span id="LocVarDeclStm_17_37" title="a definition with no references">LocVarDeclStm</span></span> = &lt;&lt;<a href="#LocalVariableDeclaration_13_3" id="LocalVariableDeclaration_17_55" title="a reference to a single-file definition">LocalVariableDeclaration</a>&gt;<span class="cons_String">;</span>&gt; <span class="layout">//{prefer}</span>
  <a href="#LocalVariableDeclaration_17_55" id="LocalVariableDeclaration_18_3" title="a definition with a single reference">LocalVariableDeclaration</a>.<span class="cons_Constructor"><span id="LocalVarDecl_18_28" title="a definition with no references">LocalVarDecl</span></span> = &lt;
  &lt;{<a href="../../classes/MethodDeclarations.sdf3/#VariableModifier_26_3" id="VariableModifier_19_5" title="a reference to a single-file definition">VariableModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../classes/FieldDeclarations.sdf3/#UnannType_22_3" id="UnannType_19_30" title="a reference to a single-file definition">UnannType</a>&gt; &lt;{<a href="../../classes/FieldDeclarations.sdf3/#VarDecl_19_3" id="VarDecl_19_43" title="a reference to a single-file definition">VarDecl</a> <span class="cons_Lit">", "</span>}+&gt;&gt; {<span class="keyword">prefer</span>}

</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
