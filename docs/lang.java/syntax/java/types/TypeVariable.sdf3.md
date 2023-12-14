---
title: TypeVariable.sdf3
hide:
  - toc
---

# `TypeVariable.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/types/TypeVariable.sdf3]

[pdmosses/java-front/lang.java/syntax/java/types/TypeVariable.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/types/TypeVariable.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../../classes/ClassDeclarations.sdf3/#java/types/TypeVariable_18_3" id="java/types/TypeVariable_1_8" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 18">java/types/TypeVariable</a>

<span class="layout">// 4.4. Type Variables</span>

<span class="keyword">imports</span>
  <a href="../ReferenceTypes.sdf3/#java/types/ReferenceTypes_1_8" id="java/types/ReferenceTypes_6_3" title="Defined at ../ReferenceTypes.sdf3 line 1">java/types/ReferenceTypes</a>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_7_3" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_1_8" id="java/interfaces/Annotations_8_3" title="Defined at ../../interfaces/Annotations.sdf3 line 1">java/interfaces/Annotations</a>

<span class="keyword">context-free sorts</span>

  <a href="../../classes/ClassDeclarations.sdf3/#TypeParameter_50_53" id="TypeParameter_12_3" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 50">TypeParameter</a>

<span class="keyword">context-free syntax</span>

  <a href="../../classes/ClassDeclarations.sdf3/#TypeParameter_50_53" id="TypeParameter_16_3" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 50">TypeParameter</a>.<span class="cons_Constructor"><span id="TypeParameter_16_17" title="Not referenced">TypeParameter</span></span>        = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_16_43" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_16_62" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  <a href="../../classes/ClassDeclarations.sdf3/#TypeParameter_50_53" id="TypeParameter_17_3" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 50">TypeParameter</a>.<span class="cons_Constructor"><span id="TypeParameterExtends_17_17" title="Not referenced">TypeParameterExtends</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_17_43" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_17_62" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt; <span class="cons_String">extends</span> &lt;{<a href="../ReferenceTypes.sdf3/#ClassType_14_3" id="ClassType_17_76" title="Defined at ../ReferenceTypes.sdf3 line 14, 26, 27">ClassType</a> <span class="cons_Lit">"&amp; "</span>}+&gt;&gt;

</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
