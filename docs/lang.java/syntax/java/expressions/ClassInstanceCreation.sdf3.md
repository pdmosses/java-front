---
title: ClassInstanceCreation.sdf3
hide:
  - toc
---

# `ClassInstanceCreation.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/expressions/ClassInstanceCreation.sdf3]

[pdmosses/java-front/lang.java/syntax/java/expressions/ClassInstanceCreation.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/expressions/ClassInstanceCreation.sdf3 "The source file on GitHub"

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
24
25
26
27
28
29
30
31
32
33
34
35
36
37
38
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <a href="../Disambiguation.sdf3/#java/expressions/ClassInstanceCreation_50_88" id="java/expressions/ClassInstanceCreation_7_45" title="Referenced at ../Disambiguation.sdf3 line 4; ../Main.sdf3 line 8">java/expressions/ClassInstanceCreation</a>

<span class="layout">// 15.9. Class Instance Creation Expressions</span>

<span class="keyword">imports</span>
  <a href="../../names/Names.sdf3/#java/names/Names_7_23" id="java/names/Names_103_119" title="Defined at ../../names/Names.sdf3 line 1">java/names/Names</a>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_7_31" id="java/lexical/Identifiers_122_146" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_7_34" id="java/interfaces/Annotations_149_176" title="Defined at ../../interfaces/Annotations.sdf3 line 1">java/interfaces/Annotations</a>
  <a href="../../types/ParameterizedTypes.sdf3/#java/types/ParameterizedTypes_7_36" id="java/types/ParameterizedTypes_179_208" title="Defined at ../../types/ParameterizedTypes.sdf3 line 1">java/types/ParameterizedTypes</a>
  <a href="../../classes/ClassDeclarations.sdf3/#java/classes/ClassDeclarations_7_37" id="java/classes/ClassDeclarations_211_241" title="Defined at ../../classes/ClassDeclarations.sdf3 line 1">java/classes/ClassDeclarations</a>

<span class="keyword">context-free sorts</span>

  <a href="#UnqualifiedInstance_376_395" id="UnqualifiedInstance_265_284" title="Referenced at line 20, 21">UnqualifiedInstance</a>
  <a href="#QualifiedId_556_567" id="QualifiedId_287_298" title="Referenced at line 24, 27">QualifiedId</a>
  <a href="#TypeArgumentsOrDiamond_571_593" id="TypeArgumentsOrDiamond_301_323" title="Referenced at line 24, 27">TypeArgumentsOrDiamond</a>

<span class="keyword">context-free syntax</span>
  
  <a href="#Expression_431_441" id="Expression_350_360" title="Referenced at line 21, 24, 27">Expression</a>              = <a href="#UnqualifiedInstance_265_284" id="UnqualifiedInstance_376_395" title="Defined at line 14, 23, 26">UnqualifiedInstance</a>
  <a href="#Expression_431_441" id="Expression_398_408" title="Referenced at line 21, 24, 27">Expression</a>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#QualifiedInstance_558_575" id="QualifiedInstance_409_426" title="Referenced at ../Disambiguation.sdf3 line 25">QualifiedInstance</a></span> = &lt;&lt;<a href="#Expression_350_360" id="Expression_431_441" title="Defined at line 20, 21">Expression</a>&gt;<span class="cons_String">.</span>&lt;<a href="#UnqualifiedInstance_265_284" id="UnqualifiedInstance_444_463" title="Defined at line 14, 23, 26">UnqualifiedInstance</a>&gt;&gt;
  
  <a href="#UnqualifiedInstance_376_395" id="UnqualifiedInstance_471_490" title="Referenced at line 20, 21">UnqualifiedInstance</a>.<span class="cons_Constructor"><span id="NewInstance_491_502" title="Not referenced locally, nor via imports">NewInstance</span></span> = &lt;
  <span class="cons_String">new</span> &lt;<a href="../../types/ParameterizedTypes.sdf3/#TypeArguments_157_170" id="TypeArguments_514_527" title="Defined at ../../types/ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>?&gt; &lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_158_168" id="Annotation_532_542" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_551_553" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt; &lt;<a href="#QualifiedId_287_298" id="QualifiedId_556_567" title="Defined at line 15, 31">QualifiedId</a>*&gt; &lt;<a href="#TypeArgumentsOrDiamond_301_323" id="TypeArgumentsOrDiamond_571_593" title="Defined at line 16, 33, 34">TypeArgumentsOrDiamond</a>?&gt;<span class="cons_String">(</span>&lt;{<a href="#Expression_350_360" id="Expression_598_608" title="Defined at line 20, 21">Expression</a> <span class="cons_Lit">","</span>}*&gt;<span class="cons_String">)</span> &gt;
  
  <a href="#UnqualifiedInstance_376_395" id="UnqualifiedInstance_624_643" title="Referenced at line 20, 21">UnqualifiedInstance</a>.<span class="cons_Constructor"><span id="NewInstance_644_655" title="Not referenced locally, nor via imports">NewInstance</span></span> = &lt;  
  <span class="cons_String">new</span> &lt;<a href="../../types/ParameterizedTypes.sdf3/#TypeArguments_157_170" id="TypeArguments_669_682" title="Defined at ../../types/ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>?&gt; &lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_158_168" id="Annotation_687_697" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_706_708" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt; &lt;<a href="#QualifiedId_287_298" id="QualifiedId_711_722" title="Defined at line 15, 31">QualifiedId</a>*&gt; &lt;<a href="#TypeArgumentsOrDiamond_301_323" id="TypeArgumentsOrDiamond_726_748" title="Defined at line 16, 33, 34">TypeArgumentsOrDiamond</a>?&gt;<span class="cons_String">(</span>&lt;{<a href="#Expression_350_360" id="Expression_753_763" title="Defined at line 20, 21">Expression</a> <span class="cons_Lit">","</span>}*&gt;<span class="cons_String">)</span> <span class="cons_String">{</span>
    &lt;{<a href="../../classes/ClassDeclarations.sdf3/#ClassBodyDeclaration_615_635" id="ClassBodyDeclaration_780_800" title="Defined at ../../classes/ClassDeclarations.sdf3 line 28, 58, 59, 60, 61">ClassBodyDeclaration</a> <span class="cons_Lit">"\n"</span>}*&gt;
  <span class="cons_String">}</span>&gt;
  
  <a href="#QualifiedId_556_567" id="QualifiedId_819_830" title="Referenced at line 24, 27">QualifiedId</a>.<span class="cons_Constructor"><span id="QualifiedId_831_842" title="Not referenced locally, nor via imports">QualifiedId</span></span> = &lt;<span class="cons_String">.</span>&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_158_168" id="Annotation_849_859" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_141_143" id="Id_868_870" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  
  <a href="#TypeArgumentsOrDiamond_571_593" id="TypeArgumentsOrDiamond_878_900" title="Referenced at line 24, 27">TypeArgumentsOrDiamond</a>         = <a href="../../types/ParameterizedTypes.sdf3/#TypeArguments_157_170" id="TypeArguments_911_924" title="Defined at ../../types/ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>
  <a href="#TypeArgumentsOrDiamond_571_593" id="TypeArgumentsOrDiamond_927_949" title="Referenced at line 24, 27">TypeArgumentsOrDiamond</a>.<span class="cons_Constructor"><span id="Diamond_950_957" title="Not referenced locally, nor via imports">Diamond</span></span> = [<span class="cons_String">&lt;&gt;</span>]

<span class="keyword">template options</span>  
  
  <span class="keyword">tokenize</span> : "&lt;" 
</code></pre></td></tr></tbody></table></div>