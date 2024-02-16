---
title: ConstantDeclarations.sdf3
hide:
  - toc
---

# `ConstantDeclarations.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/interfaces/ConstantDeclarations.sdf3]

[pdmosses/java-front/lang.java/syntax/java/interfaces/ConstantDeclarations.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/interfaces/ConstantDeclarations.sdf3 "The source file on GitHub"

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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/interfaces/ConstantDeclarations_1_8" title="a definition with multiple references" data-urls="../AnnotationTypes.sdf3/#java/interfaces/ConstantDeclarations line 12_3; ../InterfaceDeclarations.sdf3/#java/interfaces/ConstantDeclarations line 12_3; ../Main.sdf3/#java/interfaces/ConstantDeclarations line 10_3">java/interfaces/ConstantDeclarations</button>

<span class="layout">// 9.3. Field (Constant) Declarations</span>

<span class="keyword">imports</span>
  <a href="../../lexical/Modifiers.sdf3/#java/lexical/Modifiers_1_8" id="java/lexical/Modifiers_6_3" title="a reference to a single-file definition">java/lexical/Modifiers</a>
  <a href="../../classes/FieldDeclarations.sdf3/#java/classes/FieldDeclarations_1_8" id="java/classes/FieldDeclarations_7_3" title="a reference to a single-file definition">java/classes/FieldDeclarations</a>
  <a href="../Annotations.sdf3/#java/interfaces/Annotations_1_8" id="java/interfaces/Annotations_8_3" title="a reference to a single-file definition">java/interfaces/Annotations</a>

<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="ConstantDeclaration_12_3" title="a definition with multiple references" data-urls="../AnnotationTypes.sdf3/#ConstantDeclaration line 32_37; ../InterfaceDeclarations.sdf3/#ConstantDeclaration line 43_32">ConstantDeclaration</button>
  <a href="#ConstantModifier_18_5" id="ConstantModifier_13_3" title="a definition with a single reference">ConstantModifier</a>

<span class="keyword">context-free syntax</span>
  
  <button class="modal-open" id="ConstantDeclaration_17_3" title="a definition with multiple references" data-urls="../AnnotationTypes.sdf3/#ConstantDeclaration line 32_37; ../InterfaceDeclarations.sdf3/#ConstantDeclaration line 43_32">ConstantDeclaration</button>.<span class="cons_Constructor"><span id="ConstantDecl_17_23" title="a definition with no references">ConstantDecl</span></span> = &lt;
  &lt;{<a href="#ConstantModifier_13_3" id="ConstantModifier_18_5" title="a reference to a single-file definition">ConstantModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../classes/FieldDeclarations.sdf3/#UnannType_22_3" id="UnannType_18_30" title="a reference to a single-file definition">UnannType</a>&gt; &lt;{<a href="../../classes/FieldDeclarations.sdf3/#VarDecl_19_3" id="VarDecl_18_43" title="a reference to a single-file definition">VarDecl</a> <span class="cons_Lit">", "</span>}+&gt;&gt;
  
  <a href="#ConstantModifier_18_5" id="ConstantModifier_20_3" title="a definition with a single reference">ConstantModifier</a> = <a href="../Annotations.sdf3/#Annotation_12_3" id="Annotation_20_22" title="a reference to a single-file definition">Annotation</a>
  <a href="#ConstantModifier_18_5" id="ConstantModifier_21_3" title="a definition with a single reference">ConstantModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Public_14_3" id="Public_21_22" title="a reference to a single-file definition">Public</a>
  <a href="#ConstantModifier_18_5" id="ConstantModifier_22_3" title="a definition with a single reference">ConstantModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Static_15_3" id="Static_22_22" title="a reference to a single-file definition">Static</a>
  <a href="#ConstantModifier_18_5" id="ConstantModifier_23_3" title="a definition with a single reference">ConstantModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Final_10_3" id="Final_23_22" title="a reference to a single-file definition">Final</a>
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
