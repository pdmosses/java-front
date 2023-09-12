---
title: Annotations.sdf3
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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../../types/TypeVariable.sdf3#java/interfaces/Annotations_121_148" id="java/interfaces/Annotations_7_34" title="Referenced at ../../types/TypeVariable.sdf3 line 8">java/interfaces/Annotations</a>

<span class="layout">// 9.7. Annotations</span>

<span class="keyword">imports</span>
  <a href="../../names/Names.sdf3#java/names/Names_7_23" id="java/names/Names_67_83" title="Defined at ../../names/Names.sdf3 line 1">java/names/Names</a>
  <a href="../../lexical/Identifiers.sdf3#java/lexical/Identifiers_7_31" id="java/lexical/Identifiers_86_110" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../../expressions/Main.sdf3#java/expressions/Main_7_28" id="java/expressions/Main_113_134" title="Defined at ../../expressions/Main.sdf3 line 1">java/expressions/Main</a>

<span class="keyword">context-free sorts</span>

  <a href="#Annotation_571_581" id="Annotation_158_168" title="Referenced at line 26; ../AnnotationTypes.sdf3 line 40; ../ConstantDeclarations.sdf3 line 20; ../InterfaceDeclarations.sdf3 line 33; ../InterfaceMethodDeclarations.sdf3 line 20; ../../classes/ClassDeclarations.sdf3 line 41; ../../classes/ConstructorDeclarations.sdf3 line 30; ../../classes/EnumDeclarations.sdf3 line 35; ../../classes/FieldDeclarations.sdf3 line 60; ../../classes/MethodDeclarations.sdf3 line 73; ../../expressions/ArrayCreation.sdf3 line 26; ../../expressions/ClassInstanceCreation.sdf3 line 31; ../../packages/PackageDeclarations.sdf3 line 15; ../../types/ParameterizedTypes.sdf3 line 22; ../../types/PrimitiveTypes.sdf3 line 16; ../../types/ReferenceTypes.sdf3 line 41; ../../types/TypeVariable.sdf3 line 17">Annotation</a>
  <a href="#ElementValuePair_291_307" id="ElementValuePair_171_187" title="Referenced at line 19">ElementValuePair</a>
  <a href="#ElementValue_726_738" id="ElementValue_190_202" title="Referenced at line 29; ../AnnotationTypes.sdf3 line 44">ElementValue</a>
  <a href="#ElementValueArrayInitializer_525_553" id="ElementValueArrayInitializer_205_233" title="Referenced at line 25">ElementValueArrayInitializer</a>

<span class="keyword">context-free syntax</span>

  <a href="#Annotation_571_581" id="Annotation_258_268" title="Referenced at line 26; ../AnnotationTypes.sdf3 line 40; ../ConstantDeclarations.sdf3 line 20; ../InterfaceDeclarations.sdf3 line 33; ../InterfaceMethodDeclarations.sdf3 line 20; ../../classes/ClassDeclarations.sdf3 line 41; ../../classes/ConstructorDeclarations.sdf3 line 30; ../../classes/EnumDeclarations.sdf3 line 35; ../../classes/FieldDeclarations.sdf3 line 60; ../../classes/MethodDeclarations.sdf3 line 73; ../../expressions/ArrayCreation.sdf3 line 26; ../../expressions/ClassInstanceCreation.sdf3 line 31; ../../packages/PackageDeclarations.sdf3 line 15; ../../types/ParameterizedTypes.sdf3 line 22; ../../types/PrimitiveTypes.sdf3 line 16; ../../types/ReferenceTypes.sdf3 line 41; ../../types/TypeVariable.sdf3 line 17">Annotation</a>.<span class="cons_Constructor"><span id="Anno_269_273" title="Not referenced locally, nor via imports">Anno</span></span> = &lt;<span class="cons_String">@</span>&lt;<a href="../../names/Names.sdf3#TypeName_145_153" id="TypeName_279_287" title="Defined at ../../names/Names.sdf3 line 11, 21, 22">TypeName</a>&gt;<span class="cons_String">(</span>&lt;{<a href="#ElementValuePair_171_187" id="ElementValuePair_291_307" title="Defined at line 13, 23">ElementValuePair</a> <span class="cons_Lit">", "</span>}*&gt;<span class="cons_String">)</span>&gt;
  <a href="#Annotation_571_581" id="Annotation_320_330" title="Referenced at line 26; ../AnnotationTypes.sdf3 line 40; ../ConstantDeclarations.sdf3 line 20; ../InterfaceDeclarations.sdf3 line 33; ../InterfaceMethodDeclarations.sdf3 line 20; ../../classes/ClassDeclarations.sdf3 line 41; ../../classes/ConstructorDeclarations.sdf3 line 30; ../../classes/EnumDeclarations.sdf3 line 35; ../../classes/FieldDeclarations.sdf3 line 60; ../../classes/MethodDeclarations.sdf3 line 73; ../../expressions/ArrayCreation.sdf3 line 26; ../../expressions/ClassInstanceCreation.sdf3 line 31; ../../packages/PackageDeclarations.sdf3 line 15; ../../types/ParameterizedTypes.sdf3 line 22; ../../types/PrimitiveTypes.sdf3 line 16; ../../types/ReferenceTypes.sdf3 line 41; ../../types/TypeVariable.sdf3 line 17">Annotation</a>.<span class="cons_Constructor"><span id="MarkerAnno_331_341" title="Not referenced locally, nor via imports">MarkerAnno</span></span> = &lt;<span class="cons_String">@</span>&lt;<a href="../../names/Names.sdf3#TypeName_145_153" id="TypeName_347_355" title="Defined at ../../names/Names.sdf3 line 11, 21, 22">TypeName</a>&gt;&gt;
  <a href="#Annotation_571_581" id="Annotation_360_370" title="Referenced at line 26; ../AnnotationTypes.sdf3 line 40; ../ConstantDeclarations.sdf3 line 20; ../InterfaceDeclarations.sdf3 line 33; ../InterfaceMethodDeclarations.sdf3 line 20; ../../classes/ClassDeclarations.sdf3 line 41; ../../classes/ConstructorDeclarations.sdf3 line 30; ../../classes/EnumDeclarations.sdf3 line 35; ../../classes/FieldDeclarations.sdf3 line 60; ../../classes/MethodDeclarations.sdf3 line 73; ../../expressions/ArrayCreation.sdf3 line 26; ../../expressions/ClassInstanceCreation.sdf3 line 31; ../../packages/PackageDeclarations.sdf3 line 15; ../../types/ParameterizedTypes.sdf3 line 22; ../../types/PrimitiveTypes.sdf3 line 16; ../../types/ReferenceTypes.sdf3 line 41; ../../types/TypeVariable.sdf3 line 17">Annotation</a>.<span class="cons_Constructor"><span id="SingleElemAnno_371_385" title="Not referenced locally, nor via imports">SingleElemAnno</span></span> = &lt;<span class="cons_String">@</span>&lt;<a href="../../names/Names.sdf3#TypeName_145_153" id="TypeName_391_399" title="Defined at ../../names/Names.sdf3 line 11, 21, 22">TypeName</a>&gt;<span class="cons_String">(</span>&lt;<a href="#ElementValue_190_202" id="ElementValue_402_414" title="Defined at line 14, 24, 25, 26">ElementValue</a>&gt;<span class="cons_String">)</span>&gt;
  
  <a href="#ElementValuePair_291_307" id="ElementValuePair_423_439" title="Referenced at line 19">ElementValuePair</a>.<span class="cons_Constructor"><span id="ElemValPair_440_451" title="Not referenced locally, nor via imports">ElemValPair</span></span> = &lt;&lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_456_458" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt; <span class="cons_String">=</span> &lt;<a href="#ElementValue_190_202" id="ElementValue_463_475" title="Defined at line 14, 24, 25, 26">ElementValue</a>&gt;&gt;
  <a href="#ElementValue_726_738" id="ElementValue_480_492" title="Referenced at line 29; ../AnnotationTypes.sdf3 line 44">ElementValue</a> = <a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_495_505" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>  
  <a href="#ElementValue_726_738" id="ElementValue_510_522" title="Referenced at line 29; ../AnnotationTypes.sdf3 line 44">ElementValue</a> = <a href="#ElementValueArrayInitializer_205_233" id="ElementValueArrayInitializer_525_553" title="Defined at line 15, 28, 29">ElementValueArrayInitializer</a>
  <a href="#ElementValue_726_738" id="ElementValue_556_568" title="Referenced at line 29; ../AnnotationTypes.sdf3 line 44">ElementValue</a> = <a href="#Annotation_158_168" id="Annotation_571_581" title="Defined at line 12, 19, 20, 21">Annotation</a>
  
  <a href="#ElementValueArrayInitializer_525_553" id="ElementValueArrayInitializer_587_615" title="Referenced at line 25">ElementValueArrayInitializer</a>.<span class="cons_Constructor"><span id="ElementValArrayInit_616_635" title="Not referenced locally, nor via imports">ElementValArrayInit</span></span> = &lt;<span class="cons_String">{</span>&lt;{<a href="#ElementValue_190_202" id="ElementValue_642_654" title="Defined at line 14, 24, 25, 26">ElementValue</a> <span class="cons_Lit">","</span>}*&gt;<span class="cons_String">}</span>&gt;
  <a href="#ElementValueArrayInitializer_525_553" id="ElementValueArrayInitializer_666_694" title="Referenced at line 25">ElementValueArrayInitializer</a>.<span class="cons_Constructor"><span id="ElementValArrayInitComma_695_719" title="Not referenced locally, nor via imports">ElementValArrayInitComma</span></span> = &lt;<span class="cons_String">{</span>&lt;{<a href="#ElementValue_190_202" id="ElementValue_726_738" title="Defined at line 14, 24, 25, 26">ElementValue</a> <span class="cons_Lit">","</span>}*&gt;<span class="cons_String">,</span> <span class="cons_String">}</span>&gt;
  
</code></pre></td></tr></tbody></table></div>