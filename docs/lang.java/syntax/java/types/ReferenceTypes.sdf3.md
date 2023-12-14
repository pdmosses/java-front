---
title: ReferenceTypes.sdf3
hide:
  - toc
---

# `ReferenceTypes.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/types/ReferenceTypes.sdf3]

[pdmosses/java-front/lang.java/syntax/java/types/ReferenceTypes.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/types/ReferenceTypes.sdf3 "The source file on GitHub"

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
39
40
41
42
43
44
45
46
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/types/ReferenceTypes_1_8" title="Multi-file references" data-urls="../Main.sdf3/#java/types/ReferenceTypes_7_3 line 7; ../ParameterizedTypes.sdf3/#java/types/ReferenceTypes_6_3 line 6; ../TypeVariable.sdf3/#java/types/ReferenceTypes_6_3 line 6; ../../classes/ClassDeclarations.sdf3/#java/types/ReferenceTypes_9_3 line 9; ../../classes/FieldDeclarations.sdf3/#java/types/ReferenceTypes_8_3 line 8; ../../classes/MethodDeclarations.sdf3/#java/types/ReferenceTypes_6_3 line 6; ../../expressions/ArrayCreation.sdf3/#java/types/ReferenceTypes_6_3 line 6; ../../expressions/BinaryOperators.sdf3/#java/types/ReferenceTypes_13_3 line 13; ../../expressions/MethodReference.sdf3/#java/types/ReferenceTypes_6_3 line 6; ../../expressions/UnaryOperators.sdf3/#java/types/ReferenceTypes_7_3 line 7; ../../interfaces/AnnotationTypes.sdf3/#java/types/ReferenceTypes_10_3 line 10; ../../interfaces/InterfaceDeclarations.sdf3/#java/types/ReferenceTypes_10_3 line 10; ../../statements/Statements.sdf3/#java/types/ReferenceTypes_11_3 line 11">java/types/ReferenceTypes</button>

<span class="layout">// 4.3. Reference Types and Values</span>

<span class="keyword">imports</span>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_6_3" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../PrimitiveTypes.sdf3/#java/types/PrimitiveTypes_1_8" id="java/types/PrimitiveTypes_7_3" title="Defined at ../PrimitiveTypes.sdf3 line 1">java/types/PrimitiveTypes</a>
  <a href="../ParameterizedTypes.sdf3/#java/types/ParameterizedTypes_1_8" id="java/types/ParameterizedTypes_8_3" title="Defined at ../ParameterizedTypes.sdf3 line 1">java/types/ParameterizedTypes</a>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_1_8" id="java/interfaces/Annotations_9_3" title="Defined at ../../interfaces/Annotations.sdf3 line 1">java/interfaces/Annotations</a>

<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="ReferenceType_13_3" title="Multi-file references" data-urls="../Main.sdf3/#ReferenceType_20_10 line 20; ../ParameterizedTypes.sdf3/#ReferenceType_18_18 line 18, 21, 22; ../../expressions/BinaryOperators.sdf3/#ReferenceType_32_53 line 32; ../../expressions/MethodReference.sdf3/#ReferenceType_14_40 line 14; ../../expressions/UnaryOperators.sdf3/#ReferenceType_23_33 line 23">ReferenceType</button>
  <button class="modal-open" id="ClassType_14_3" title="Multi-file references" data-urls="#ClassType_23_19 line 23, 27, 38; ../TypeVariable.sdf3/#ClassType_17_76 line 17; ../../classes/ClassDeclarations.sdf3/#ClassType_54_37 line 54, 56; ../../classes/MethodDeclarations.sdf3/#ClassType_43_22 line 43; ../../expressions/ArrayCreation.sdf3/#ClassType_23_19 line 23; ../../expressions/MethodReference.sdf3/#ClassType_18_39 line 18; ../../expressions/UnaryOperators.sdf3/#ClassType_24_41 line 24; ../../interfaces/InterfaceDeclarations.sdf3/#ClassType_41_52 line 41; ../../statements/Statements.sdf3/#ClassType_108_37 line 108">ClassType</button>
  <span id="TypeVariable_15_3" title="Not referenced">TypeVariable</span>
  <button class="modal-open" id="ArrayType_16_3" title="Multi-file references" data-urls="#ArrayType_24_19 line 24; ../../expressions/MethodReference.sdf3/#ArrayType_19_39 line 19">ArrayType</button>
  <button class="modal-open" id="AnnotatedDims_17_3" title="Multi-file references" data-urls="#AnnotatedDims_37_52 line 37, 38; ../../expressions/ArrayCreation.sdf3/#AnnotatedDims_21_63 line 21">AnnotatedDims</button>
  <button class="modal-open" id="AnnotatedDimsEmpty_18_3" title="Multi-file references" data-urls="../../classes/MethodDeclarations.sdf3/#AnnotatedDimsEmpty_34_34 line 34; ../../expressions/ArrayCreation.sdf3/#AnnotatedDimsEmpty_20_75 line 20; ../../interfaces/AnnotationTypes.sdf3/#AnnotatedDimsEmpty_38_62 line 38">AnnotatedDimsEmpty</button>
  <button class="modal-open" id="AnnotatedDim_19_3" title="Multi-file references" data-urls="#AnnotatedDim_39_27 line 39, 40; ../../classes/FieldDeclarations.sdf3/#AnnotatedDim_32_39 line 32, 65, 66">AnnotatedDim</button>

<span class="keyword">context-free syntax</span>

  <button class="modal-open" id="ReferenceType_23_3" title="Multi-file references" data-urls="../Main.sdf3/#ReferenceType_20_10 line 20; ../ParameterizedTypes.sdf3/#ReferenceType_18_18 line 18, 21, 22; ../../expressions/BinaryOperators.sdf3/#ReferenceType_32_53 line 32; ../../expressions/MethodReference.sdf3/#ReferenceType_14_40 line 14; ../../expressions/UnaryOperators.sdf3/#ReferenceType_23_33 line 23">ReferenceType</button> = <a href="#ClassType_14_3" id="ClassType_23_19" title="Defined at line 14, 26, 27">ClassType</a>
  <button class="modal-open" id="ReferenceType_24_3" title="Multi-file references" data-urls="../Main.sdf3/#ReferenceType_20_10 line 20; ../ParameterizedTypes.sdf3/#ReferenceType_18_18 line 18, 21, 22; ../../expressions/BinaryOperators.sdf3/#ReferenceType_32_53 line 32; ../../expressions/MethodReference.sdf3/#ReferenceType_14_40 line 14; ../../expressions/UnaryOperators.sdf3/#ReferenceType_23_33 line 23">ReferenceType</button> = <a href="#ArrayType_16_3" id="ArrayType_24_19" title="Defined at line 16, 37, 38">ArrayType</a>

  <button class="modal-open" id="ClassType_26_3" title="Multi-file references" data-urls="#ClassType_23_19 line 23, 27, 38; ../TypeVariable.sdf3/#ClassType_17_76 line 17; ../../classes/ClassDeclarations.sdf3/#ClassType_54_37 line 54, 56; ../../classes/MethodDeclarations.sdf3/#ClassType_43_22 line 43; ../../expressions/ArrayCreation.sdf3/#ClassType_23_19 line 23; ../../expressions/MethodReference.sdf3/#ClassType_18_39 line 18; ../../expressions/UnaryOperators.sdf3/#ClassType_24_41 line 24; ../../interfaces/InterfaceDeclarations.sdf3/#ClassType_41_52 line 41; ../../statements/Statements.sdf3/#ClassType_108_37 line 108">ClassType</button>.<span class="cons_Constructor"><span id="ClassType_26_13" title="Not referenced">ClassType</span></span>                  = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_26_45" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_26_64" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&lt;<a href="../ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_26_68" title="Defined at ../ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>?&gt;&gt;
  <button class="modal-open" id="ClassType_27_3" title="Multi-file references" data-urls="#ClassType_23_19 line 23, 27, 38; ../TypeVariable.sdf3/#ClassType_17_76 line 17; ../../classes/ClassDeclarations.sdf3/#ClassType_54_37 line 54, 56; ../../classes/MethodDeclarations.sdf3/#ClassType_43_22 line 43; ../../expressions/ArrayCreation.sdf3/#ClassType_23_19 line 23; ../../expressions/MethodReference.sdf3/#ClassType_18_39 line 18; ../../expressions/UnaryOperators.sdf3/#ClassType_24_41 line 24; ../../interfaces/InterfaceDeclarations.sdf3/#ClassType_41_52 line 41; ../../statements/Statements.sdf3/#ClassType_108_37 line 108">ClassType</button>.<span class="cons_Constructor"><span id="ClassOrInterfaceTypeMember_27_13" title="Not referenced">ClassOrInterfaceTypeMember</span></span> = &lt;&lt;<a href="#ClassType_14_3" id="ClassType_27_44" title="Defined at line 14, 26, 27">ClassType</a>&gt;<span class="cons_String">.</span>&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_27_57" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_27_76" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&lt;<a href="../ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_27_80" title="Defined at ../ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>?&gt;&gt;
  
  <span class="layout">// The interfaceTypeMember will be ambiguous with ClassTypeMember</span>
  <span class="layout">// ClassType.InterfaceTypeMember = &lt;&lt;InterfaceType&gt;.&lt;{Annotation " "}*&gt; &lt;Id&gt;&lt;TypeArguments?&gt;&gt;</span>
  <span class="layout">// ReferenceType = InterfaceType  </span>
  <span class="layout">// InterfaceType.InterfaceType   = ClassType</span>
  
  <span class="layout">// Ambiguous with ClassType.ClassType</span>
  <span id="TypeVariable_35_3" title="Not referenced">TypeVariable</span>.<span class="cons_Constructor"><span id="TypeVar_35_16" title="Not referenced">TypeVar</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_35_29" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_35_48" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  
  <button class="modal-open" id="ArrayType_37_3" title="Multi-file references" data-urls="#ArrayType_24_19 line 24; ../../expressions/MethodReference.sdf3/#ArrayType_19_39 line 19">ArrayType</button>.<span class="cons_Constructor"><span id="ArrayTypePrimitive_37_13" title="Not referenced">ArrayTypePrimitive</span></span> = &lt;&lt;<a href="../PrimitiveTypes.sdf3/#PrimitiveType_10_3" id="PrimitiveType_37_36" title="Defined at ../PrimitiveTypes.sdf3 line 10, 15, 16">PrimitiveType</a>&gt; &lt;<a href="#AnnotatedDims_17_3" id="AnnotatedDims_37_52" title="Defined at line 17, 39">AnnotatedDims</a>&gt;&gt;
  <button class="modal-open" id="ArrayType_38_3" title="Multi-file references" data-urls="#ArrayType_24_19 line 24; ../../expressions/MethodReference.sdf3/#ArrayType_19_39 line 19">ArrayType</button>.<span class="cons_Constructor"><span id="ArrayTypeClassType_38_13" title="Not referenced">ArrayTypeClassType</span></span> = &lt;&lt;<a href="#ClassType_14_3" id="ClassType_38_36" title="Defined at line 14, 26, 27">ClassType</a>&gt; &lt;<a href="#AnnotatedDims_17_3" id="AnnotatedDims_38_48" title="Defined at line 17, 39">AnnotatedDims</a>&gt;&gt;
  <button class="modal-open" id="AnnotatedDims_39_3" title="Multi-file references" data-urls="#AnnotatedDims_37_52 line 37, 38; ../../expressions/ArrayCreation.sdf3/#AnnotatedDims_21_63 line 21">AnnotatedDims</button>      = &lt;&lt;{<a href="#AnnotatedDim_19_3" id="AnnotatedDim_39_27" title="Defined at line 19, 41">AnnotatedDim</a> <span class="cons_Lit">" "</span>}+&gt;&gt;
  <button class="modal-open" id="AnnotatedDimsEmpty_40_3" title="Multi-file references" data-urls="../../classes/MethodDeclarations.sdf3/#AnnotatedDimsEmpty_34_34 line 34; ../../expressions/ArrayCreation.sdf3/#AnnotatedDimsEmpty_20_75 line 20; ../../interfaces/AnnotationTypes.sdf3/#AnnotatedDimsEmpty_38_62 line 38">AnnotatedDimsEmpty</button> = &lt;&lt;{<a href="#AnnotatedDim_19_3" id="AnnotatedDim_40_27" title="Defined at line 19, 41">AnnotatedDim</a> <span class="cons_Lit">" "</span>}*&gt;&gt;
  <button class="modal-open" id="AnnotatedDim_41_3" title="Multi-file references" data-urls="#AnnotatedDim_39_27 line 39, 40; ../../classes/FieldDeclarations.sdf3/#AnnotatedDim_32_39 line 32, 65, 66">AnnotatedDim</button>.<span class="cons_Constructor"><span id="AnnotateDim_41_16" title="Not referenced">AnnotateDim</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_41_33" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">[]</span>&gt;
  
<span class="keyword">template options</span>

  <span class="keyword">tokenize</span> : "["
  
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
