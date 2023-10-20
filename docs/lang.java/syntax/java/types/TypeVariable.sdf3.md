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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../../classes/ClassDeclarations.sdf3/#java/types/TypeVariable_460_483" id="java/types/TypeVariable_7_30" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 18">java/types/TypeVariable</a>

<span class="layout">// 4.4. Type Variables</span>

<span class="keyword">imports</span>
  <a href="../ReferenceTypes.sdf3/#java/types/ReferenceTypes_7_32" id="java/types/ReferenceTypes_66_91" title="Defined at ../ReferenceTypes.sdf3 line 1">java/types/ReferenceTypes</a>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_7_31" id="java/lexical/Identifiers_94_118" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_7_34" id="java/interfaces/Annotations_121_148" title="Defined at ../../interfaces/Annotations.sdf3 line 1">java/interfaces/Annotations</a>

<span class="keyword">context-free sorts</span>

  <a href="../../classes/ClassDeclarations.sdf3/#TypeParameter_1213_1226" id="TypeParameter_172_185" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 50">TypeParameter</a>

<span class="keyword">context-free syntax</span>

  <a href="../../classes/ClassDeclarations.sdf3/#TypeParameter_1213_1226" id="TypeParameter_210_223" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 50">TypeParameter</a>.<span class="cons_Constructor"><span id="TypeParameter_224_237" title="Not referenced locally, nor via imports">TypeParameter</span></span>        = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_158_168" id="Annotation_250_260" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_269_271" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  <a href="../../classes/ClassDeclarations.sdf3/#TypeParameter_1213_1226" id="TypeParameter_276_289" title="Referenced at ../../classes/ClassDeclarations.sdf3 line 50">TypeParameter</a>.<span class="cons_Constructor"><span id="TypeParameterExtends_290_310" title="Not referenced locally, nor via imports">TypeParameterExtends</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_158_168" id="Annotation_316_326" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_335_337" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt; <span class="cons_String">extends</span> &lt;{<a href="../ReferenceTypes.sdf3/#ClassType_234_243" id="ClassType_349_358" title="Defined at ../ReferenceTypes.sdf3 line 14, 26, 27">ClassType</a> <span class="cons_Lit">"&amp; "</span>}+&gt;&gt;

</code></pre></td></tr></tbody></table></div>