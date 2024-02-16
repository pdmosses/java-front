---
title: ParameterizedTypes.sdf3
hide:
  - toc
---

# `ParameterizedTypes.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/types/ParameterizedTypes.sdf3]

[pdmosses/java-front/lang.java/syntax/java/types/ParameterizedTypes.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/types/ParameterizedTypes.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/types/ParameterizedTypes_1_8" title="a definition with multiple references" data-urls="../ReferenceTypes.sdf3/#java/types/ParameterizedTypes line 8_3; ../../classes/ConstructorDeclarations.sdf3/#java/types/ParameterizedTypes line 10_3; ../../classes/FieldDeclarations.sdf3/#java/types/ParameterizedTypes line 10_3; ../../expressions/ClassInstanceCreation.sdf3/#java/types/ParameterizedTypes line 9_3; ../../expressions/MethodInvocation.sdf3/#java/types/ParameterizedTypes line 8_3; ../../expressions/MethodReference.sdf3/#java/types/ParameterizedTypes line 7_3">java/types/ParameterizedTypes</button>

<span class="layout">// 4.5. Parameterized Types</span>

<span class="keyword">imports</span>
  <a href="../ReferenceTypes.sdf3/#java/types/ReferenceTypes_1_8" id="java/types/ReferenceTypes_6_3" title="a reference to a single-file definition">java/types/ReferenceTypes</a>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_1_8" id="java/interfaces/Annotations_7_3" title="a reference to a single-file definition">java/interfaces/Annotations</a> 

<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="TypeArguments_11_3" title="a definition with multiple references" data-urls="../ReferenceTypes.sdf3/#TypeArguments line 26_68, 27_80; ../../classes/ConstructorDeclarations.sdf3/#TypeArguments line 35_47, 36_47, 37_60; ../../classes/FieldDeclarations.sdf3/#TypeArguments line 59_58, 60_95; ../../expressions/ClassInstanceCreation.sdf3/#TypeArguments line 24_8, 27_8, 33_36; ../../expressions/MethodInvocation.sdf3/#TypeArguments line 16_47, 17_40, 18_51; ../../expressions/MethodReference.sdf3/#TypeArguments line 14_57, 15_54, 16_47, 17_58, 18_52, 19_52">TypeArguments</button>
  <a href="#TypeArgument_17_37" id="TypeArgument_12_3" title="a definition with a single reference">TypeArgument</a>
  <a href="#WildCard_19_18" id="WildCard_13_3" title="a definition with a single reference">WildCard</a>

<span class="keyword">context-free syntax</span>

  <button class="modal-open" id="TypeArguments_17_3" title="a definition with multiple references" data-urls="../ReferenceTypes.sdf3/#TypeArguments line 26_68, 27_80; ../../classes/ConstructorDeclarations.sdf3/#TypeArguments line 35_47, 36_47, 37_60; ../../classes/FieldDeclarations.sdf3/#TypeArguments line 59_58, 60_95; ../../expressions/ClassInstanceCreation.sdf3/#TypeArguments line 24_8, 27_8, 33_36; ../../expressions/MethodInvocation.sdf3/#TypeArguments line 16_47, 17_40, 18_51; ../../expressions/MethodReference.sdf3/#TypeArguments line 14_57, 15_54, 16_47, 17_58, 18_52, 19_52">TypeArguments</button>.<span class="cons_Constructor"><span id="TypeArguments_17_17" title="a definition with no references">TypeArguments</span></span> = [<span class="cons_String">&lt;</span>[{<a href="#TypeArgument_12_3" id="TypeArgument_17_37" title="a reference to a single-file definition">TypeArgument</a> <span class="cons_Lit">", "</span>}+]<span class="cons_String">&gt;</span>]
  <a href="#TypeArgument_17_37" id="TypeArgument_18_3" title="a definition with a single reference">TypeArgument</a> = <a href="../ReferenceTypes.sdf3/#ReferenceType_13_3" id="ReferenceType_18_18" title="a reference to a single-file definition">ReferenceType</a>
  <a href="#TypeArgument_17_37" id="TypeArgument_19_3" title="a definition with a single reference">TypeArgument</a> = <a href="#WildCard_13_3" id="WildCard_19_18" title="a reference to a single-file definition">WildCard</a>
  <a href="#WildCard_19_18" id="WildCard_20_3" title="a definition with a single reference">WildCard</a>.<span class="cons_Constructor"><span id="WildCard_20_12" title="a definition with no references">WildCard</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_20_26" title="a reference to a single-file definition">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">?</span>&gt;
  <a href="#WildCard_19_18" id="WildCard_21_3" title="a definition with a single reference">WildCard</a>.<span class="cons_Constructor"><span id="WildCardExtends_21_12" title="a definition with no references">WildCardExtends</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_21_33" title="a reference to a single-file definition">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">?</span> <span class="cons_String">extends</span> &lt;<a href="../ReferenceTypes.sdf3/#ReferenceType_13_3" id="ReferenceType_21_62" title="a reference to a single-file definition">ReferenceType</a>&gt;&gt;
  <a href="#WildCard_19_18" id="WildCard_22_3" title="a definition with a single reference">WildCard</a>.<span class="cons_Constructor"><span id="WildCardSuper_22_12" title="a definition with no references">WildCardSuper</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_22_31" title="a reference to a single-file definition">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">?</span> <span class="cons_String">super</span> &lt;<a href="../ReferenceTypes.sdf3/#ReferenceType_13_3" id="ReferenceType_22_58" title="a reference to a single-file definition">ReferenceType</a>&gt;&gt;
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
