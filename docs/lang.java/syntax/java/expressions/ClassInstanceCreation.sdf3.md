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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/expressions/ClassInstanceCreation_1_8" title="a definition with multiple references" data-urls="../Disambiguation.sdf3/#java/expressions/ClassInstanceCreation line 4_3; ../Main.sdf3/#java/expressions/ClassInstanceCreation line 8_3">java/expressions/ClassInstanceCreation</button>

<span class="layout">// 15.9. Class Instance Creation Expressions</span>

<span class="keyword">imports</span>
  <a href="../../names/Names.sdf3/#java/names/Names_1_8" id="java/names/Names_6_3" title="a reference to a single-file definition">java/names/Names</a>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_7_3" title="a reference to a single-file definition">java/lexical/Identifiers</a>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_1_8" id="java/interfaces/Annotations_8_3" title="a reference to a single-file definition">java/interfaces/Annotations</a>
  <a href="../../types/ParameterizedTypes.sdf3/#java/types/ParameterizedTypes_1_8" id="java/types/ParameterizedTypes_9_3" title="a reference to a single-file definition">java/types/ParameterizedTypes</a>
  <a href="../../classes/ClassDeclarations.sdf3/#java/classes/ClassDeclarations_1_8" id="java/classes/ClassDeclarations_10_3" title="a reference to a single-file definition">java/classes/ClassDeclarations</a>

<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="UnqualifiedInstance_14_3" title="a definition with multiple references" data-urls="#UnqualifiedInstance line 20_29, 21_49">UnqualifiedInstance</button>
  <button class="modal-open" id="QualifiedId_15_3" title="a definition with multiple references" data-urls="#QualifiedId line 24_50, 27_50">QualifiedId</button>
  <button class="modal-open" id="TypeArgumentsOrDiamond_16_3" title="a definition with multiple references" data-urls="#TypeArgumentsOrDiamond line 24_65, 27_65">TypeArgumentsOrDiamond</button>

<span class="keyword">context-free syntax</span>
  
  <button class="modal-open" id="Expression_20_3" title="a definition with multiple references" data-urls="#Expression line 21_36, 24_92, 27_92">Expression</button>              = <a href="#UnqualifiedInstance_14_3" id="UnqualifiedInstance_20_29" title="a reference to a single-file definition">UnqualifiedInstance</a>
  <button class="modal-open" id="Expression_21_3" title="a definition with multiple references" data-urls="#Expression line 21_36, 24_92, 27_92">Expression</button>.<span class="cons_Constructor"><a href="../Disambiguation.sdf3/#QualifiedInstance_25_14" id="QualifiedInstance_21_14" title="a definition with a single reference">QualifiedInstance</a></span> = &lt;&lt;<a href="#Expression_20_3" id="Expression_21_36" title="a reference to a single-file definition">Expression</a>&gt;<span class="cons_String">.</span>&lt;<a href="#UnqualifiedInstance_14_3" id="UnqualifiedInstance_21_49" title="a reference to a single-file definition">UnqualifiedInstance</a>&gt;&gt;
  
  <button class="modal-open" id="UnqualifiedInstance_23_3" title="a definition with multiple references" data-urls="#UnqualifiedInstance line 20_29, 21_49">UnqualifiedInstance</button>.<span class="cons_Constructor"><span id="NewInstance_23_23" title="a definition with no references">NewInstance</span></span> = &lt;
  <span class="cons_String">new</span> &lt;<a href="../../types/ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_24_8" title="a reference to a single-file definition">TypeArguments</a>?&gt; &lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_24_26" title="a reference to a single-file definition">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_24_45" title="a reference to a single-file definition">Id</a>&gt; &lt;<a href="#QualifiedId_15_3" id="QualifiedId_24_50" title="a reference to a single-file definition">QualifiedId</a>*&gt; &lt;<a href="#TypeArgumentsOrDiamond_16_3" id="TypeArgumentsOrDiamond_24_65" title="a reference to a single-file definition">TypeArgumentsOrDiamond</a>?&gt;<span class="cons_String">(</span>&lt;{<a href="#Expression_20_3" id="Expression_24_92" title="a reference to a single-file definition">Expression</a> <span class="cons_Lit">","</span>}*&gt;<span class="cons_String">)</span> &gt;
  
  <button class="modal-open" id="UnqualifiedInstance_26_3" title="a definition with multiple references" data-urls="#UnqualifiedInstance line 20_29, 21_49">UnqualifiedInstance</button>.<span class="cons_Constructor"><span id="NewInstance_26_23" title="a definition with no references">NewInstance</span></span> = &lt;  
  <span class="cons_String">new</span> &lt;<a href="../../types/ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_27_8" title="a reference to a single-file definition">TypeArguments</a>?&gt; &lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_27_26" title="a reference to a single-file definition">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_27_45" title="a reference to a single-file definition">Id</a>&gt; &lt;<a href="#QualifiedId_15_3" id="QualifiedId_27_50" title="a reference to a single-file definition">QualifiedId</a>*&gt; &lt;<a href="#TypeArgumentsOrDiamond_16_3" id="TypeArgumentsOrDiamond_27_65" title="a reference to a single-file definition">TypeArgumentsOrDiamond</a>?&gt;<span class="cons_String">(</span>&lt;{<a href="#Expression_20_3" id="Expression_27_92" title="a reference to a single-file definition">Expression</a> <span class="cons_Lit">","</span>}*&gt;<span class="cons_String">)</span> <span class="cons_String">{</span>
    &lt;{<a href="../../classes/ClassDeclarations.sdf3/#ClassBodyDeclaration_28_3" id="ClassBodyDeclaration_28_7" title="a reference to a single-file definition">ClassBodyDeclaration</a> <span class="cons_Lit">"\n"</span>}*&gt;
  <span class="cons_String">}</span>&gt;
  
  <button class="modal-open" id="QualifiedId_31_3" title="a definition with multiple references" data-urls="#QualifiedId line 24_50, 27_50">QualifiedId</button>.<span class="cons_Constructor"><span id="QualifiedId_31_15" title="a definition with no references">QualifiedId</span></span> = &lt;<span class="cons_String">.</span>&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_31_33" title="a reference to a single-file definition">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_31_52" title="a reference to a single-file definition">Id</a>&gt;&gt;
  
  <button class="modal-open" id="TypeArgumentsOrDiamond_33_3" title="a definition with multiple references" data-urls="#TypeArgumentsOrDiamond line 24_65, 27_65">TypeArgumentsOrDiamond</button>         = <a href="../../types/ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_33_36" title="a reference to a single-file definition">TypeArguments</a>
  <button class="modal-open" id="TypeArgumentsOrDiamond_34_3" title="a definition with multiple references" data-urls="#TypeArgumentsOrDiamond line 24_65, 27_65">TypeArgumentsOrDiamond</button>.<span class="cons_Constructor"><span id="Diamond_34_26" title="a definition with no references">Diamond</span></span> = [<span class="cons_String">&lt;&gt;</span>]

<span class="keyword">template options</span>  
  
  <span class="keyword">tokenize</span> : "&lt;" 
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
