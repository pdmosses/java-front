---
title: Annotations.sdf3
hide:
  - toc
---

# `Annotations.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/interfaces/Annotations.sdf3]

[pdmosses/java-front/lang.java/syntax/java/interfaces/Annotations.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/interfaces/Annotations.sdf3 "The source file on GitHub"

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
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/interfaces/Annotations_1_8" title="Multi-file references" data-urls="../AnnotationTypes.sdf3/#java/interfaces/Annotations_14_3 line 14; ../ConstantDeclarations.sdf3/#java/interfaces/Annotations_8_3 line 8; ../InterfaceDeclarations.sdf3/#java/interfaces/Annotations_11_3 line 11; ../InterfaceMethodDeclarations.sdf3/#java/interfaces/Annotations_8_3 line 8; ../Main.sdf3/#java/interfaces/Annotations_9_3 line 9; ../../classes/ClassDeclarations.sdf3/#java/interfaces/Annotations_16_3 line 16; ../../classes/ConstructorDeclarations.sdf3/#java/interfaces/Annotations_12_3 line 12; ../../classes/EnumDeclarations.sdf3/#java/interfaces/Annotations_8_3 line 8; ../../classes/FieldDeclarations.sdf3/#java/interfaces/Annotations_11_3 line 11; ../../classes/MethodDeclarations.sdf3/#java/interfaces/Annotations_10_3 line 10; ../../expressions/ArrayCreation.sdf3/#java/interfaces/Annotations_8_3 line 8; ../../expressions/ClassInstanceCreation.sdf3/#java/interfaces/Annotations_8_3 line 8; ../../packages/PackageDeclarations.sdf3/#java/interfaces/Annotations_7_3 line 7; ../../statements/LocalVariableDeclarations.sdf3/#java/interfaces/Annotations_8_3 line 8; ../../types/ParameterizedTypes.sdf3/#java/interfaces/Annotations_7_3 line 7; ../../types/PrimitiveTypes.sdf3/#java/interfaces/Annotations_6_3 line 6; ../../types/ReferenceTypes.sdf3/#java/interfaces/Annotations_9_3 line 9; ../../types/TypeVariable.sdf3/#java/interfaces/Annotations_8_3 line 8">java/interfaces/Annotations</button>

<span class="layout">// 9.7. Annotations</span>

<span class="keyword">imports</span>
  <a href="../../names/Names.sdf3/#java/names/Names_1_8" id="java/names/Names_6_3" title="Defined at ../../names/Names.sdf3 line 1">java/names/Names</a>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_7_3" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../../expressions/Main.sdf3/#java/expressions/Main_1_8" id="java/expressions/Main_8_3" title="Defined at ../../expressions/Main.sdf3 line 1">java/expressions/Main</a>

<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="Annotation_12_3" title="Multi-file references" data-urls="#Annotation_26_18 line 26; ../AnnotationTypes.sdf3/#Annotation_40_35 line 40; ../ConstantDeclarations.sdf3/#Annotation_20_22 line 20; ../InterfaceDeclarations.sdf3/#Annotation_33_23 line 33; ../InterfaceMethodDeclarations.sdf3/#Annotation_20_29 line 20; ../../classes/ClassDeclarations.sdf3/#Annotation_41_19 line 41; ../../classes/ConstructorDeclarations.sdf3/#Annotation_30_25 line 30; ../../classes/EnumDeclarations.sdf3/#Annotation_31_5 line 31, 35; ../../classes/FieldDeclarations.sdf3/#Annotation_39_19 line 39, 60; ../../classes/MethodDeclarations.sdf3/#Annotation_37_22 line 37, 45, 59, 60, 69, 73; ../../expressions/ArrayCreation.sdf3/#Annotation_26_20 line 26; ../../expressions/ClassInstanceCreation.sdf3/#Annotation_24_26 line 24, 27, 31; ../../packages/PackageDeclarations.sdf3/#Annotation_15_46 line 15; ../../types/ParameterizedTypes.sdf3/#Annotation_20_26 line 20, 21, 22; ../../types/PrimitiveTypes.sdf3/#Annotation_15_34 line 15, 16; ../../types/ReferenceTypes.sdf3/#Annotation_26_45 line 26, 27, 35, 41; ../../types/TypeVariable.sdf3/#Annotation_16_43 line 16, 17">Annotation</button>
  <a href="#ElementValuePair_19_36" id="ElementValuePair_13_3" title="Referenced at line 19">ElementValuePair</a>
  <button class="modal-open" id="ElementValue_14_3" title="Multi-file references" data-urls="#ElementValue_21_45 line 21, 23, 28, 29; ../AnnotationTypes.sdf3/#ElementValue_44_39 line 44">ElementValue</button>
  <a href="#ElementValueArrayInitializer_25_18" id="ElementValueArrayInitializer_15_3" title="Referenced at line 25">ElementValueArrayInitializer</a>

<span class="keyword">context-free syntax</span>

  <button class="modal-open" id="Annotation_19_3" title="Multi-file references" data-urls="#Annotation_26_18 line 26; ../AnnotationTypes.sdf3/#Annotation_40_35 line 40; ../ConstantDeclarations.sdf3/#Annotation_20_22 line 20; ../InterfaceDeclarations.sdf3/#Annotation_33_23 line 33; ../InterfaceMethodDeclarations.sdf3/#Annotation_20_29 line 20; ../../classes/ClassDeclarations.sdf3/#Annotation_41_19 line 41; ../../classes/ConstructorDeclarations.sdf3/#Annotation_30_25 line 30; ../../classes/EnumDeclarations.sdf3/#Annotation_31_5 line 31, 35; ../../classes/FieldDeclarations.sdf3/#Annotation_39_19 line 39, 60; ../../classes/MethodDeclarations.sdf3/#Annotation_37_22 line 37, 45, 59, 60, 69, 73; ../../expressions/ArrayCreation.sdf3/#Annotation_26_20 line 26; ../../expressions/ClassInstanceCreation.sdf3/#Annotation_24_26 line 24, 27, 31; ../../packages/PackageDeclarations.sdf3/#Annotation_15_46 line 15; ../../types/ParameterizedTypes.sdf3/#Annotation_20_26 line 20, 21, 22; ../../types/PrimitiveTypes.sdf3/#Annotation_15_34 line 15, 16; ../../types/ReferenceTypes.sdf3/#Annotation_26_45 line 26, 27, 35, 41; ../../types/TypeVariable.sdf3/#Annotation_16_43 line 16, 17">Annotation</button>.<span class="cons_Constructor"><span id="Anno_19_14" title="Not referenced">Anno</span></span> = &lt;<span class="cons_String">@</span>&lt;<a href="../../names/Names.sdf3/#TypeName_11_3" id="TypeName_19_24" title="Defined at ../../names/Names.sdf3 line 11, 21, 22">TypeName</a>&gt;<span class="cons_String">(</span>&lt;{<a href="#ElementValuePair_13_3" id="ElementValuePair_19_36" title="Defined at line 13, 23">ElementValuePair</a> <span class="cons_Lit">", "</span>}*&gt;<span class="cons_String">)</span>&gt;
  <button class="modal-open" id="Annotation_20_3" title="Multi-file references" data-urls="#Annotation_26_18 line 26; ../AnnotationTypes.sdf3/#Annotation_40_35 line 40; ../ConstantDeclarations.sdf3/#Annotation_20_22 line 20; ../InterfaceDeclarations.sdf3/#Annotation_33_23 line 33; ../InterfaceMethodDeclarations.sdf3/#Annotation_20_29 line 20; ../../classes/ClassDeclarations.sdf3/#Annotation_41_19 line 41; ../../classes/ConstructorDeclarations.sdf3/#Annotation_30_25 line 30; ../../classes/EnumDeclarations.sdf3/#Annotation_31_5 line 31, 35; ../../classes/FieldDeclarations.sdf3/#Annotation_39_19 line 39, 60; ../../classes/MethodDeclarations.sdf3/#Annotation_37_22 line 37, 45, 59, 60, 69, 73; ../../expressions/ArrayCreation.sdf3/#Annotation_26_20 line 26; ../../expressions/ClassInstanceCreation.sdf3/#Annotation_24_26 line 24, 27, 31; ../../packages/PackageDeclarations.sdf3/#Annotation_15_46 line 15; ../../types/ParameterizedTypes.sdf3/#Annotation_20_26 line 20, 21, 22; ../../types/PrimitiveTypes.sdf3/#Annotation_15_34 line 15, 16; ../../types/ReferenceTypes.sdf3/#Annotation_26_45 line 26, 27, 35, 41; ../../types/TypeVariable.sdf3/#Annotation_16_43 line 16, 17">Annotation</button>.<span class="cons_Constructor"><span id="MarkerAnno_20_14" title="Not referenced">MarkerAnno</span></span> = &lt;<span class="cons_String">@</span>&lt;<a href="../../names/Names.sdf3/#TypeName_11_3" id="TypeName_20_30" title="Defined at ../../names/Names.sdf3 line 11, 21, 22">TypeName</a>&gt;&gt;
  <button class="modal-open" id="Annotation_21_3" title="Multi-file references" data-urls="#Annotation_26_18 line 26; ../AnnotationTypes.sdf3/#Annotation_40_35 line 40; ../ConstantDeclarations.sdf3/#Annotation_20_22 line 20; ../InterfaceDeclarations.sdf3/#Annotation_33_23 line 33; ../InterfaceMethodDeclarations.sdf3/#Annotation_20_29 line 20; ../../classes/ClassDeclarations.sdf3/#Annotation_41_19 line 41; ../../classes/ConstructorDeclarations.sdf3/#Annotation_30_25 line 30; ../../classes/EnumDeclarations.sdf3/#Annotation_31_5 line 31, 35; ../../classes/FieldDeclarations.sdf3/#Annotation_39_19 line 39, 60; ../../classes/MethodDeclarations.sdf3/#Annotation_37_22 line 37, 45, 59, 60, 69, 73; ../../expressions/ArrayCreation.sdf3/#Annotation_26_20 line 26; ../../expressions/ClassInstanceCreation.sdf3/#Annotation_24_26 line 24, 27, 31; ../../packages/PackageDeclarations.sdf3/#Annotation_15_46 line 15; ../../types/ParameterizedTypes.sdf3/#Annotation_20_26 line 20, 21, 22; ../../types/PrimitiveTypes.sdf3/#Annotation_15_34 line 15, 16; ../../types/ReferenceTypes.sdf3/#Annotation_26_45 line 26, 27, 35, 41; ../../types/TypeVariable.sdf3/#Annotation_16_43 line 16, 17">Annotation</button>.<span class="cons_Constructor"><span id="SingleElemAnno_21_14" title="Not referenced">SingleElemAnno</span></span> = &lt;<span class="cons_String">@</span>&lt;<a href="../../names/Names.sdf3/#TypeName_11_3" id="TypeName_21_34" title="Defined at ../../names/Names.sdf3 line 11, 21, 22">TypeName</a>&gt;<span class="cons_String">(</span>&lt;<a href="#ElementValue_14_3" id="ElementValue_21_45" title="Defined at line 14, 24, 25, 26">ElementValue</a>&gt;<span class="cons_String">)</span>&gt;
  
  <a href="#ElementValuePair_19_36" id="ElementValuePair_23_3" title="Referenced at line 19">ElementValuePair</a>.<span class="cons_Constructor"><span id="ElemValPair_23_20" title="Not referenced">ElemValPair</span></span> = &lt;&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_23_36" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt; <span class="cons_String">=</span> &lt;<a href="#ElementValue_14_3" id="ElementValue_23_43" title="Defined at line 14, 24, 25, 26">ElementValue</a>&gt;&gt;
  <button class="modal-open" id="ElementValue_24_3" title="Multi-file references" data-urls="#ElementValue_21_45 line 21, 23, 28, 29; ../AnnotationTypes.sdf3/#ElementValue_44_39 line 44">ElementValue</button> = <a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_24_18" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>  
  <button class="modal-open" id="ElementValue_25_3" title="Multi-file references" data-urls="#ElementValue_21_45 line 21, 23, 28, 29; ../AnnotationTypes.sdf3/#ElementValue_44_39 line 44">ElementValue</button> = <a href="#ElementValueArrayInitializer_15_3" id="ElementValueArrayInitializer_25_18" title="Defined at line 15, 28, 29">ElementValueArrayInitializer</a>
  <button class="modal-open" id="ElementValue_26_3" title="Multi-file references" data-urls="#ElementValue_21_45 line 21, 23, 28, 29; ../AnnotationTypes.sdf3/#ElementValue_44_39 line 44">ElementValue</button> = <a href="#Annotation_12_3" id="Annotation_26_18" title="Defined at line 12, 19, 20, 21">Annotation</a>
  
  <a href="#ElementValueArrayInitializer_25_18" id="ElementValueArrayInitializer_28_3" title="Referenced at line 25">ElementValueArrayInitializer</a>.<span class="cons_Constructor"><span id="ElementValArrayInit_28_32" title="Not referenced">ElementValArrayInit</span></span> = &lt;<span class="cons_String">{</span>&lt;{<a href="#ElementValue_14_3" id="ElementValue_28_58" title="Defined at line 14, 24, 25, 26">ElementValue</a> <span class="cons_Lit">","</span>}*&gt;<span class="cons_String">}</span>&gt;
  <a href="#ElementValueArrayInitializer_25_18" id="ElementValueArrayInitializer_29_3" title="Referenced at line 25">ElementValueArrayInitializer</a>.<span class="cons_Constructor"><span id="ElementValArrayInitComma_29_32" title="Not referenced">ElementValArrayInitComma</span></span> = &lt;<span class="cons_String">{</span>&lt;{<a href="#ElementValue_14_3" id="ElementValue_29_63" title="Defined at line 14, 24, 25, 26">ElementValue</a> <span class="cons_Lit">","</span>}*&gt;<span class="cons_String">,</span> <span class="cons_String">}</span>&gt;
  
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
