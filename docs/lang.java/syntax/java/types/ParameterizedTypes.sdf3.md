---
title: ParameterizedTypes.sdf3
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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../ReferenceTypes.sdf3#java/types/ParameterizedTypes_135_164" id="java/types/ParameterizedTypes_7_36" title="Referenced at ../ReferenceTypes.sdf3 line 8">java/types/ParameterizedTypes</a>

<span class="layout">// 4.5. Parameterized Types</span>

<span class="keyword">imports</span>
  <a href="../ReferenceTypes.sdf3#java/types/ReferenceTypes_7_32" id="java/types/ReferenceTypes_77_102" title="Defined at ../ReferenceTypes.sdf3 line 1">java/types/ReferenceTypes</a>
  <a href="../../interfaces/Annotations.sdf3#java/interfaces/Annotations_7_34" id="java/interfaces/Annotations_105_132" title="Defined at ../../interfaces/Annotations.sdf3 line 1">java/interfaces/Annotations</a> 

<span class="keyword">context-free sorts</span>

  <a href="../ReferenceTypes.sdf3#TypeArguments_565_578" id="TypeArguments_157_170" title="Referenced at ../ReferenceTypes.sdf3 line 27; ../../classes/ConstructorDeclarations.sdf3 line 37; ../../classes/FieldDeclarations.sdf3 line 60; ../../expressions/ClassInstanceCreation.sdf3 line 33; ../../expressions/MethodInvocation.sdf3 line 18; ../../expressions/MethodReference.sdf3 line 19">TypeArguments</a>
  <a href="#TypeArgument_255_267" id="TypeArgument_173_185" title="Referenced at line 17">TypeArgument</a>
  <a href="#WildCard_326_334" id="WildCard_188_196" title="Referenced at line 19">WildCard</a>

<span class="keyword">context-free syntax</span>

  <a href="../ReferenceTypes.sdf3#TypeArguments_565_578" id="TypeArguments_221_234" title="Referenced at ../ReferenceTypes.sdf3 line 27; ../../classes/ConstructorDeclarations.sdf3 line 37; ../../classes/FieldDeclarations.sdf3 line 60; ../../expressions/ClassInstanceCreation.sdf3 line 33; ../../expressions/MethodInvocation.sdf3 line 18; ../../expressions/MethodReference.sdf3 line 19">TypeArguments</a>.<span class="cons_Constructor"><span id="TypeArguments_235_248" title="Not referenced locally, nor via imports">TypeArguments</span></span> = [<span class="cons_String">&lt;</span>[{<a href="#TypeArgument_173_185" id="TypeArgument_255_267" title="Defined at line 12, 18, 19">TypeArgument</a> <span class="cons_Lit">", "</span>}+]<span class="cons_String">&gt;</span>]
  <a href="#TypeArgument_255_267" id="TypeArgument_280_292" title="Referenced at line 17">TypeArgument</a> = <a href="../ReferenceTypes.sdf3#ReferenceType_218_231" id="ReferenceType_295_308" title="Defined at ../ReferenceTypes.sdf3 line 13, 23, 24">ReferenceType</a>
  <a href="#TypeArgument_255_267" id="TypeArgument_311_323" title="Referenced at line 17">TypeArgument</a> = <a href="#WildCard_188_196" id="WildCard_326_334" title="Defined at line 13, 20, 21, 22">WildCard</a>
  <a href="#WildCard_326_334" id="WildCard_337_345" title="Referenced at line 19">WildCard</a>.<span class="cons_Constructor"><span id="WildCard_346_354" title="Not referenced locally, nor via imports">WildCard</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3#Annotation_158_168" id="Annotation_360_370" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">?</span>&gt;
  <a href="#WildCard_326_334" id="WildCard_383_391" title="Referenced at line 19">WildCard</a>.<span class="cons_Constructor"><span id="WildCardExtends_392_407" title="Not referenced locally, nor via imports">WildCardExtends</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3#Annotation_158_168" id="Annotation_413_423" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">?</span> <span class="cons_String">extends</span> &lt;<a href="../ReferenceTypes.sdf3#ReferenceType_218_231" id="ReferenceType_442_455" title="Defined at ../ReferenceTypes.sdf3 line 13, 23, 24">ReferenceType</a>&gt;&gt;
  <a href="#WildCard_326_334" id="WildCard_460_468" title="Referenced at line 19">WildCard</a>.<span class="cons_Constructor"><span id="WildCardSuper_469_482" title="Not referenced locally, nor via imports">WildCardSuper</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3#Annotation_158_168" id="Annotation_488_498" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">?</span> <span class="cons_String">super</span> &lt;<a href="../ReferenceTypes.sdf3#ReferenceType_218_231" id="ReferenceType_515_528" title="Defined at ../ReferenceTypes.sdf3 line 13, 23, 24">ReferenceType</a>&gt;&gt;
</code></pre></td></tr></tbody></table></div>