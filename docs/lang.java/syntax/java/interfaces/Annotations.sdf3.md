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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/interfaces/Annotations_1_8" title="a definition with multiple references" data-urls="../AnnotationTypes.sdf3/#java/interfaces/Annotations line 14_3; ../ConstantDeclarations.sdf3/#java/interfaces/Annotations line 8_3; ../InterfaceDeclarations.sdf3/#java/interfaces/Annotations line 11_3; ../InterfaceMethodDeclarations.sdf3/#java/interfaces/Annotations line 8_3; ../Main.sdf3/#java/interfaces/Annotations line 9_3; ../../classes/ClassDeclarations.sdf3/#java/interfaces/Annotations line 16_3; ../../classes/ConstructorDeclarations.sdf3/#java/interfaces/Annotations line 12_3; ../../classes/EnumDeclarations.sdf3/#java/interfaces/Annotations line 8_3; ../../classes/FieldDeclarations.sdf3/#java/interfaces/Annotations line 11_3; ../../classes/MethodDeclarations.sdf3/#java/interfaces/Annotations line 10_3; ../../expressions/ArrayCreation.sdf3/#java/interfaces/Annotations line 8_3; ../../expressions/ClassInstanceCreation.sdf3/#java/interfaces/Annotations line 8_3; ../../packages/PackageDeclarations.sdf3/#java/interfaces/Annotations line 7_3; ../../statements/LocalVariableDeclarations.sdf3/#java/interfaces/Annotations line 8_3; ../../types/ParameterizedTypes.sdf3/#java/interfaces/Annotations line 7_3; ../../types/PrimitiveTypes.sdf3/#java/interfaces/Annotations line 6_3; ../../types/ReferenceTypes.sdf3/#java/interfaces/Annotations line 9_3; ../../types/TypeVariable.sdf3/#java/interfaces/Annotations line 8_3">java/interfaces/Annotations</button>

<span class="layout">// 9.7. Annotations</span>

<span class="keyword">imports</span>
  <a href="../../names/Names.sdf3/#java/names/Names_1_8" id="java/names/Names_6_3" title="a reference to a single-file definition">java/names/Names</a>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_7_3" title="a reference to a single-file definition">java/lexical/Identifiers</a>
  <a href="../../expressions/Main.sdf3/#java/expressions/Main_1_8" id="java/expressions/Main_8_3" title="a reference to a single-file definition">java/expressions/Main</a>

<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="Annotation_12_3" title="a definition with multiple references" data-urls="#Annotation line 26_18; ../AnnotationTypes.sdf3/#Annotation line 40_35; ../ConstantDeclarations.sdf3/#Annotation line 20_22; ../InterfaceDeclarations.sdf3/#Annotation line 33_23; ../InterfaceMethodDeclarations.sdf3/#Annotation line 20_29; ../../classes/ClassDeclarations.sdf3/#Annotation line 41_19; ../../classes/ConstructorDeclarations.sdf3/#Annotation line 30_25; ../../classes/EnumDeclarations.sdf3/#Annotation line 31_5, 35_5; ../../classes/FieldDeclarations.sdf3/#Annotation line 39_19, 60_72; ../../classes/MethodDeclarations.sdf3/#Annotation line 37_22, 45_20, 59_40, 60_40, 69_76, 73_22; ../../expressions/ArrayCreation.sdf3/#Annotation line 26_20; ../../expressions/ClassInstanceCreation.sdf3/#Annotation line 24_26, 27_26, 31_33; ../../packages/PackageDeclarations.sdf3/#Annotation line 15_46; ../../types/ParameterizedTypes.sdf3/#Annotation line 20_26, 21_33, 22_31; ../../types/PrimitiveTypes.sdf3/#Annotation line 15_34, 16_34; ../../types/ReferenceTypes.sdf3/#Annotation line 26_45, 27_57, 35_29, 41_33; ../../types/TypeVariable.sdf3/#Annotation line 16_43, 17_43">Annotation</button>
  <a href="#ElementValuePair_19_36" id="ElementValuePair_13_3" title="a definition with a single reference">ElementValuePair</a>
  <button class="modal-open" id="ElementValue_14_3" title="a definition with multiple references" data-urls="#ElementValue line 21_45, 23_43, 28_58, 29_63; ../AnnotationTypes.sdf3/#ElementValue line 44_39">ElementValue</button>
  <a href="#ElementValueArrayInitializer_25_18" id="ElementValueArrayInitializer_15_3" title="a definition with a single reference">ElementValueArrayInitializer</a>

<span class="keyword">context-free syntax</span>

  <button class="modal-open" id="Annotation_19_3" title="a definition with multiple references" data-urls="#Annotation line 26_18; ../AnnotationTypes.sdf3/#Annotation line 40_35; ../ConstantDeclarations.sdf3/#Annotation line 20_22; ../InterfaceDeclarations.sdf3/#Annotation line 33_23; ../InterfaceMethodDeclarations.sdf3/#Annotation line 20_29; ../../classes/ClassDeclarations.sdf3/#Annotation line 41_19; ../../classes/ConstructorDeclarations.sdf3/#Annotation line 30_25; ../../classes/EnumDeclarations.sdf3/#Annotation line 31_5, 35_5; ../../classes/FieldDeclarations.sdf3/#Annotation line 39_19, 60_72; ../../classes/MethodDeclarations.sdf3/#Annotation line 37_22, 45_20, 59_40, 60_40, 69_76, 73_22; ../../expressions/ArrayCreation.sdf3/#Annotation line 26_20; ../../expressions/ClassInstanceCreation.sdf3/#Annotation line 24_26, 27_26, 31_33; ../../packages/PackageDeclarations.sdf3/#Annotation line 15_46; ../../types/ParameterizedTypes.sdf3/#Annotation line 20_26, 21_33, 22_31; ../../types/PrimitiveTypes.sdf3/#Annotation line 15_34, 16_34; ../../types/ReferenceTypes.sdf3/#Annotation line 26_45, 27_57, 35_29, 41_33; ../../types/TypeVariable.sdf3/#Annotation line 16_43, 17_43">Annotation</button>.<span class="cons_Constructor"><span id="Anno_19_14" title="a definition with no references">Anno</span></span> = &lt;<span class="cons_String">@</span>&lt;<a href="../../names/Names.sdf3/#TypeName_11_3" id="TypeName_19_24" title="a reference to a single-file definition">TypeName</a>&gt;<span class="cons_String">(</span>&lt;{<a href="#ElementValuePair_13_3" id="ElementValuePair_19_36" title="a reference to a single-file definition">ElementValuePair</a> <span class="cons_Lit">", "</span>}*&gt;<span class="cons_String">)</span>&gt;
  <button class="modal-open" id="Annotation_20_3" title="a definition with multiple references" data-urls="#Annotation line 26_18; ../AnnotationTypes.sdf3/#Annotation line 40_35; ../ConstantDeclarations.sdf3/#Annotation line 20_22; ../InterfaceDeclarations.sdf3/#Annotation line 33_23; ../InterfaceMethodDeclarations.sdf3/#Annotation line 20_29; ../../classes/ClassDeclarations.sdf3/#Annotation line 41_19; ../../classes/ConstructorDeclarations.sdf3/#Annotation line 30_25; ../../classes/EnumDeclarations.sdf3/#Annotation line 31_5, 35_5; ../../classes/FieldDeclarations.sdf3/#Annotation line 39_19, 60_72; ../../classes/MethodDeclarations.sdf3/#Annotation line 37_22, 45_20, 59_40, 60_40, 69_76, 73_22; ../../expressions/ArrayCreation.sdf3/#Annotation line 26_20; ../../expressions/ClassInstanceCreation.sdf3/#Annotation line 24_26, 27_26, 31_33; ../../packages/PackageDeclarations.sdf3/#Annotation line 15_46; ../../types/ParameterizedTypes.sdf3/#Annotation line 20_26, 21_33, 22_31; ../../types/PrimitiveTypes.sdf3/#Annotation line 15_34, 16_34; ../../types/ReferenceTypes.sdf3/#Annotation line 26_45, 27_57, 35_29, 41_33; ../../types/TypeVariable.sdf3/#Annotation line 16_43, 17_43">Annotation</button>.<span class="cons_Constructor"><span id="MarkerAnno_20_14" title="a definition with no references">MarkerAnno</span></span> = &lt;<span class="cons_String">@</span>&lt;<a href="../../names/Names.sdf3/#TypeName_11_3" id="TypeName_20_30" title="a reference to a single-file definition">TypeName</a>&gt;&gt;
  <button class="modal-open" id="Annotation_21_3" title="a definition with multiple references" data-urls="#Annotation line 26_18; ../AnnotationTypes.sdf3/#Annotation line 40_35; ../ConstantDeclarations.sdf3/#Annotation line 20_22; ../InterfaceDeclarations.sdf3/#Annotation line 33_23; ../InterfaceMethodDeclarations.sdf3/#Annotation line 20_29; ../../classes/ClassDeclarations.sdf3/#Annotation line 41_19; ../../classes/ConstructorDeclarations.sdf3/#Annotation line 30_25; ../../classes/EnumDeclarations.sdf3/#Annotation line 31_5, 35_5; ../../classes/FieldDeclarations.sdf3/#Annotation line 39_19, 60_72; ../../classes/MethodDeclarations.sdf3/#Annotation line 37_22, 45_20, 59_40, 60_40, 69_76, 73_22; ../../expressions/ArrayCreation.sdf3/#Annotation line 26_20; ../../expressions/ClassInstanceCreation.sdf3/#Annotation line 24_26, 27_26, 31_33; ../../packages/PackageDeclarations.sdf3/#Annotation line 15_46; ../../types/ParameterizedTypes.sdf3/#Annotation line 20_26, 21_33, 22_31; ../../types/PrimitiveTypes.sdf3/#Annotation line 15_34, 16_34; ../../types/ReferenceTypes.sdf3/#Annotation line 26_45, 27_57, 35_29, 41_33; ../../types/TypeVariable.sdf3/#Annotation line 16_43, 17_43">Annotation</button>.<span class="cons_Constructor"><span id="SingleElemAnno_21_14" title="a definition with no references">SingleElemAnno</span></span> = &lt;<span class="cons_String">@</span>&lt;<a href="../../names/Names.sdf3/#TypeName_11_3" id="TypeName_21_34" title="a reference to a single-file definition">TypeName</a>&gt;<span class="cons_String">(</span>&lt;<a href="#ElementValue_14_3" id="ElementValue_21_45" title="a reference to a single-file definition">ElementValue</a>&gt;<span class="cons_String">)</span>&gt;
  
  <a href="#ElementValuePair_19_36" id="ElementValuePair_23_3" title="a definition with a single reference">ElementValuePair</a>.<span class="cons_Constructor"><span id="ElemValPair_23_20" title="a definition with no references">ElemValPair</span></span> = &lt;&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_23_36" title="a reference to a single-file definition">Id</a>&gt; <span class="cons_String">=</span> &lt;<a href="#ElementValue_14_3" id="ElementValue_23_43" title="a reference to a single-file definition">ElementValue</a>&gt;&gt;
  <button class="modal-open" id="ElementValue_24_3" title="a definition with multiple references" data-urls="#ElementValue line 21_45, 23_43, 28_58, 29_63; ../AnnotationTypes.sdf3/#ElementValue line 44_39">ElementValue</button> = <a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_24_18" title="a reference to a single-file definition">Expression</a>  
  <button class="modal-open" id="ElementValue_25_3" title="a definition with multiple references" data-urls="#ElementValue line 21_45, 23_43, 28_58, 29_63; ../AnnotationTypes.sdf3/#ElementValue line 44_39">ElementValue</button> = <a href="#ElementValueArrayInitializer_15_3" id="ElementValueArrayInitializer_25_18" title="a reference to a single-file definition">ElementValueArrayInitializer</a>
  <button class="modal-open" id="ElementValue_26_3" title="a definition with multiple references" data-urls="#ElementValue line 21_45, 23_43, 28_58, 29_63; ../AnnotationTypes.sdf3/#ElementValue line 44_39">ElementValue</button> = <a href="#Annotation_12_3" id="Annotation_26_18" title="a reference to a single-file definition">Annotation</a>
  
  <a href="#ElementValueArrayInitializer_25_18" id="ElementValueArrayInitializer_28_3" title="a definition with a single reference">ElementValueArrayInitializer</a>.<span class="cons_Constructor"><span id="ElementValArrayInit_28_32" title="a definition with no references">ElementValArrayInit</span></span> = &lt;<span class="cons_String">{</span>&lt;{<a href="#ElementValue_14_3" id="ElementValue_28_58" title="a reference to a single-file definition">ElementValue</a> <span class="cons_Lit">","</span>}*&gt;<span class="cons_String">}</span>&gt;
  <a href="#ElementValueArrayInitializer_25_18" id="ElementValueArrayInitializer_29_3" title="a definition with a single reference">ElementValueArrayInitializer</a>.<span class="cons_Constructor"><span id="ElementValArrayInitComma_29_32" title="a definition with no references">ElementValArrayInitComma</span></span> = &lt;<span class="cons_String">{</span>&lt;{<a href="#ElementValue_14_3" id="ElementValue_29_63" title="a reference to a single-file definition">ElementValue</a> <span class="cons_Lit">","</span>}*&gt;<span class="cons_String">,</span> <span class="cons_String">}</span>&gt;
  
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
