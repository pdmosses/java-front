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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/types/ParameterizedTypes_1_8" title="Multi-file references" data-urls="../ReferenceTypes.sdf3/#java/types/ParameterizedTypes_8_3 line 8; ../../classes/ConstructorDeclarations.sdf3/#java/types/ParameterizedTypes_10_3 line 10; ../../classes/FieldDeclarations.sdf3/#java/types/ParameterizedTypes_10_3 line 10; ../../expressions/ClassInstanceCreation.sdf3/#java/types/ParameterizedTypes_9_3 line 9; ../../expressions/MethodInvocation.sdf3/#java/types/ParameterizedTypes_8_3 line 8; ../../expressions/MethodReference.sdf3/#java/types/ParameterizedTypes_7_3 line 7">java/types/ParameterizedTypes</button>

<span class="layout">// 4.5. Parameterized Types</span>

<span class="keyword">imports</span>
  <a href="../ReferenceTypes.sdf3/#java/types/ReferenceTypes_1_8" id="java/types/ReferenceTypes_6_3" title="Defined at ../ReferenceTypes.sdf3 line 1">java/types/ReferenceTypes</a>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_1_8" id="java/interfaces/Annotations_7_3" title="Defined at ../../interfaces/Annotations.sdf3 line 1">java/interfaces/Annotations</a> 

<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="TypeArguments_11_3" title="Multi-file references" data-urls="../ReferenceTypes.sdf3/#TypeArguments_26_68 line 26, 27; ../../classes/ConstructorDeclarations.sdf3/#TypeArguments_35_47 line 35, 36, 37; ../../classes/FieldDeclarations.sdf3/#TypeArguments_59_58 line 59, 60; ../../expressions/ClassInstanceCreation.sdf3/#TypeArguments_24_8 line 24, 27, 33; ../../expressions/MethodInvocation.sdf3/#TypeArguments_16_47 line 16, 17, 18; ../../expressions/MethodReference.sdf3/#TypeArguments_14_57 line 14, 15, 16, 17, 18, 19">TypeArguments</button>
  <a href="#TypeArgument_17_37" id="TypeArgument_12_3" title="Referenced at line 17">TypeArgument</a>
  <a href="#WildCard_19_18" id="WildCard_13_3" title="Referenced at line 19">WildCard</a>

<span class="keyword">context-free syntax</span>

  <button class="modal-open" id="TypeArguments_17_3" title="Multi-file references" data-urls="../ReferenceTypes.sdf3/#TypeArguments_26_68 line 26, 27; ../../classes/ConstructorDeclarations.sdf3/#TypeArguments_35_47 line 35, 36, 37; ../../classes/FieldDeclarations.sdf3/#TypeArguments_59_58 line 59, 60; ../../expressions/ClassInstanceCreation.sdf3/#TypeArguments_24_8 line 24, 27, 33; ../../expressions/MethodInvocation.sdf3/#TypeArguments_16_47 line 16, 17, 18; ../../expressions/MethodReference.sdf3/#TypeArguments_14_57 line 14, 15, 16, 17, 18, 19">TypeArguments</button>.<span class="cons_Constructor"><span id="TypeArguments_17_17" title="Not referenced">TypeArguments</span></span> = [<span class="cons_String">&lt;</span>[{<a href="#TypeArgument_12_3" id="TypeArgument_17_37" title="Defined at line 12, 18, 19">TypeArgument</a> <span class="cons_Lit">", "</span>}+]<span class="cons_String">&gt;</span>]
  <a href="#TypeArgument_17_37" id="TypeArgument_18_3" title="Referenced at line 17">TypeArgument</a> = <a href="../ReferenceTypes.sdf3/#ReferenceType_13_3" id="ReferenceType_18_18" title="Defined at ../ReferenceTypes.sdf3 line 13, 23, 24">ReferenceType</a>
  <a href="#TypeArgument_17_37" id="TypeArgument_19_3" title="Referenced at line 17">TypeArgument</a> = <a href="#WildCard_13_3" id="WildCard_19_18" title="Defined at line 13, 20, 21, 22">WildCard</a>
  <a href="#WildCard_19_18" id="WildCard_20_3" title="Referenced at line 19">WildCard</a>.<span class="cons_Constructor"><span id="WildCard_20_12" title="Not referenced">WildCard</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_20_26" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">?</span>&gt;
  <a href="#WildCard_19_18" id="WildCard_21_3" title="Referenced at line 19">WildCard</a>.<span class="cons_Constructor"><span id="WildCardExtends_21_12" title="Not referenced">WildCardExtends</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_21_33" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">?</span> <span class="cons_String">extends</span> &lt;<a href="../ReferenceTypes.sdf3/#ReferenceType_13_3" id="ReferenceType_21_62" title="Defined at ../ReferenceTypes.sdf3 line 13, 23, 24">ReferenceType</a>&gt;&gt;
  <a href="#WildCard_19_18" id="WildCard_22_3" title="Referenced at line 19">WildCard</a>.<span class="cons_Constructor"><span id="WildCardSuper_22_12" title="Not referenced">WildCardSuper</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_22_31" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">?</span> <span class="cons_String">super</span> &lt;<a href="../ReferenceTypes.sdf3/#ReferenceType_13_3" id="ReferenceType_22_58" title="Defined at ../ReferenceTypes.sdf3 line 13, 23, 24">ReferenceType</a>&gt;&gt;
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
