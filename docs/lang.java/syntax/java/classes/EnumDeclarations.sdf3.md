---
title: EnumDeclarations.sdf3
hide:
  - toc
---

# `EnumDeclarations.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/classes/EnumDeclarations.sdf3]

[pdmosses/java-front/lang.java/syntax/java/classes/EnumDeclarations.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/classes/EnumDeclarations.sdf3 "The source file on GitHub"

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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/classes/EnumDeclarations_1_8" title="Multi-file references" data-urls="../ClassDeclarations.sdf3/#java/classes/EnumDeclarations_14_3 line 14; ../Main.sdf3/#java/classes/EnumDeclarations_9_3 line 9">java/classes/EnumDeclarations</button>

<span class="layout">// 8.9. Enum Types</span>

<span class="keyword">imports</span>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_6_3" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../ClassDeclarations.sdf3/#java/classes/ClassDeclarations_1_8" id="java/classes/ClassDeclarations_7_3" title="Defined at ../ClassDeclarations.sdf3 line 1">java/classes/ClassDeclarations</a>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_1_8" id="java/interfaces/Annotations_8_3" title="Defined at ../../interfaces/Annotations.sdf3 line 1">java/interfaces/Annotations</a>
  <a href="../../expressions/Main.sdf3/#java/expressions/Main_1_8" id="java/expressions/Main_9_3" title="Defined at ../../expressions/Main.sdf3 line 1">java/expressions/Main</a>

<span class="keyword">context-free sorts</span>

  <a href="../ClassDeclarations.sdf3/#EnumDeclaration_34_23" id="EnumDeclaration_13_3" title="Referenced at ../ClassDeclarations.sdf3 line 34">EnumDeclaration</a>
  <a href="#EnumConstant_22_7" id="EnumConstant_14_3" title="Referenced at line 22, 27">EnumConstant</a>
  <a href="#EnumConstantArgs_31_29" id="EnumConstantArgs_15_3" title="Referenced at line 31, 35">EnumConstantArgs</a>
  <a href="#EnumBodyDeclarations_23_6" id="EnumBodyDeclarations_16_3" title="Referenced at line 23, 28">EnumBodyDeclarations</a>

<span class="keyword">context-free syntax</span>

  <a href="../ClassDeclarations.sdf3/#EnumDeclaration_34_23" id="EnumDeclaration_20_3" title="Referenced at ../ClassDeclarations.sdf3 line 34">EnumDeclaration</a>.<span class="cons_Constructor"><span id="EnumDeclComma_20_19" title="Not referenced">EnumDeclComma</span></span> = &lt;
  &lt;{<a href="../ClassDeclarations.sdf3/#ClassModifier_24_3" id="ClassModifier_21_5" title="Defined at ../ClassDeclarations.sdf3 line 24, 41, 42, 43, 44, 45, 46, 47, 48">ClassModifier</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">enum</span> &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_21_32" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt; &lt;<a href="../ClassDeclarations.sdf3/#SuperInterfaces_27_3" id="SuperInterfaces_21_37" title="Defined at ../ClassDeclarations.sdf3 line 27, 56">SuperInterfaces</a>?&gt; <span class="cons_String">{</span>
    &lt;{<a href="#EnumConstant_14_3" id="EnumConstant_22_7" title="Defined at line 14, 30, 34">EnumConstant</a> <span class="cons_Lit">", "</span>}*&gt;<span class="cons_String">,</span>
    &lt;<a href="#EnumBodyDeclarations_16_3" id="EnumBodyDeclarations_23_6" title="Defined at line 16, 38">EnumBodyDeclarations</a>?&gt;
  <span class="cons_String">}</span>&gt;
  <a href="../ClassDeclarations.sdf3/#EnumDeclaration_34_23" id="EnumDeclaration_25_3" title="Referenced at ../ClassDeclarations.sdf3 line 34">EnumDeclaration</a>.<span class="cons_Constructor"><span id="EnumDecl_25_19" title="Not referenced">EnumDecl</span></span> = &lt;
  &lt;{<a href="../ClassDeclarations.sdf3/#ClassModifier_24_3" id="ClassModifier_26_5" title="Defined at ../ClassDeclarations.sdf3 line 24, 41, 42, 43, 44, 45, 46, 47, 48">ClassModifier</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">enum</span> &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_26_32" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt; &lt;<a href="../ClassDeclarations.sdf3/#SuperInterfaces_27_3" id="SuperInterfaces_26_37" title="Defined at ../ClassDeclarations.sdf3 line 27, 56">SuperInterfaces</a>?&gt; <span class="cons_String">{</span>
    &lt;{<a href="#EnumConstant_14_3" id="EnumConstant_27_7" title="Defined at line 14, 30, 34">EnumConstant</a> <span class="cons_Lit">", "</span>}*&gt;
    &lt;<a href="#EnumBodyDeclarations_16_3" id="EnumBodyDeclarations_28_6" title="Defined at line 16, 38">EnumBodyDeclarations</a>?&gt;
  <span class="cons_String">}</span>&gt;
  <a href="#EnumConstant_22_7" id="EnumConstant_30_3" title="Referenced at line 22, 27">EnumConstant</a>.<span class="cons_Constructor"><span id="EnumConst_30_16" title="Not referenced">EnumConst</span></span> = &lt;
  &lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_31_5" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_31_24" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt; &lt;<a href="#EnumConstantArgs_15_3" id="EnumConstantArgs_31_29" title="Defined at line 15, 37">EnumConstantArgs</a>?&gt;<span class="cons_String">{</span>
    &lt;{<a href="../ClassDeclarations.sdf3/#ClassBodyDeclaration_28_3" id="ClassBodyDeclaration_32_7" title="Defined at ../ClassDeclarations.sdf3 line 28, 58, 59, 60, 61">ClassBodyDeclaration</a> <span class="cons_Lit">"\n"</span>}*&gt;
  <span class="cons_String">}</span>&gt;
  <a href="#EnumConstant_22_7" id="EnumConstant_34_3" title="Referenced at line 22, 27">EnumConstant</a>.<span class="cons_Constructor"><span id="EnumConstNoBody_34_16" title="Not referenced">EnumConstNoBody</span></span> = &lt;
  &lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_35_5" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_35_24" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt; &lt;<a href="#EnumConstantArgs_15_3" id="EnumConstantArgs_35_29" title="Defined at line 15, 37">EnumConstantArgs</a>?&gt;&gt;
  
  <a href="#EnumConstantArgs_31_29" id="EnumConstantArgs_37_3" title="Referenced at line 31, 35">EnumConstantArgs</a>.<span class="cons_Constructor"><span id="EnumConstArgs_37_20" title="Not referenced">EnumConstArgs</span></span>    = &lt;<span class="cons_String">(</span>&lt;{<a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_37_43" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a> <span class="cons_Lit">", "</span>}*&gt;<span class="cons_String">)</span>&gt;
  <a href="#EnumBodyDeclarations_23_6" id="EnumBodyDeclarations_38_3" title="Referenced at line 23, 28">EnumBodyDeclarations</a>.<span class="cons_Constructor"><span id="EnumBodyDecs_38_24" title="Not referenced">EnumBodyDecs</span></span> = &lt;<span class="cons_String">;</span>  &lt;{<a href="../ClassDeclarations.sdf3/#ClassBodyDeclaration_28_3" id="ClassBodyDeclaration_38_45" title="Defined at ../ClassDeclarations.sdf3 line 28, 58, 59, 60, 61">ClassBodyDeclaration</a> <span class="cons_Lit">"\n"</span>}*&gt;&gt;
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
