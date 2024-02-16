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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/types/ReferenceTypes_1_8" title="a definition with multiple references" data-urls="../Main.sdf3/#java/types/ReferenceTypes line 7_3; ../ParameterizedTypes.sdf3/#java/types/ReferenceTypes line 6_3; ../TypeVariable.sdf3/#java/types/ReferenceTypes line 6_3; ../../classes/ClassDeclarations.sdf3/#java/types/ReferenceTypes line 9_3; ../../classes/FieldDeclarations.sdf3/#java/types/ReferenceTypes line 8_3; ../../classes/MethodDeclarations.sdf3/#java/types/ReferenceTypes line 6_3; ../../expressions/ArrayCreation.sdf3/#java/types/ReferenceTypes line 6_3; ../../expressions/BinaryOperators.sdf3/#java/types/ReferenceTypes line 13_3; ../../expressions/MethodReference.sdf3/#java/types/ReferenceTypes line 6_3; ../../expressions/UnaryOperators.sdf3/#java/types/ReferenceTypes line 7_3; ../../interfaces/AnnotationTypes.sdf3/#java/types/ReferenceTypes line 10_3; ../../interfaces/InterfaceDeclarations.sdf3/#java/types/ReferenceTypes line 10_3; ../../statements/Statements.sdf3/#java/types/ReferenceTypes line 11_3">java/types/ReferenceTypes</button>

<span class="layout">// 4.3. Reference Types and Values</span>

<span class="keyword">imports</span>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_6_3" title="a reference to a single-file definition">java/lexical/Identifiers</a>
  <a href="../PrimitiveTypes.sdf3/#java/types/PrimitiveTypes_1_8" id="java/types/PrimitiveTypes_7_3" title="a reference to a single-file definition">java/types/PrimitiveTypes</a>
  <a href="../ParameterizedTypes.sdf3/#java/types/ParameterizedTypes_1_8" id="java/types/ParameterizedTypes_8_3" title="a reference to a single-file definition">java/types/ParameterizedTypes</a>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_1_8" id="java/interfaces/Annotations_9_3" title="a reference to a single-file definition">java/interfaces/Annotations</a>

<span class="keyword">context-free sorts</span>

  <button class="modal-open" id="ReferenceType_13_3" title="a definition with multiple references" data-urls="../Main.sdf3/#ReferenceType line 20_10; ../ParameterizedTypes.sdf3/#ReferenceType line 18_18, 21_62, 22_58; ../../expressions/BinaryOperators.sdf3/#ReferenceType line 32_53; ../../expressions/MethodReference.sdf3/#ReferenceType line 14_40; ../../expressions/UnaryOperators.sdf3/#ReferenceType line 23_33">ReferenceType</button>
  <button class="modal-open" id="ClassType_14_3" title="a definition with multiple references" data-urls="#ClassType line 23_19, 27_44, 38_36; ../TypeVariable.sdf3/#ClassType line 17_76; ../../classes/ClassDeclarations.sdf3/#ClassType line 54_37, 56_50; ../../classes/MethodDeclarations.sdf3/#ClassType line 43_22; ../../expressions/ArrayCreation.sdf3/#ClassType line 23_19; ../../expressions/MethodReference.sdf3/#ClassType line 18_39; ../../expressions/UnaryOperators.sdf3/#ClassType line 24_41; ../../interfaces/InterfaceDeclarations.sdf3/#ClassType line 41_52; ../../statements/Statements.sdf3/#ClassType line 108_37">ClassType</button>
  <span id="TypeVariable_15_3" title="a definition with no references">TypeVariable</span>
  <button class="modal-open" id="ArrayType_16_3" title="a definition with multiple references" data-urls="#ArrayType line 24_19; ../../expressions/MethodReference.sdf3/#ArrayType line 19_39">ArrayType</button>
  <button class="modal-open" id="AnnotatedDims_17_3" title="a definition with multiple references" data-urls="#AnnotatedDims line 37_52, 38_48; ../../expressions/ArrayCreation.sdf3/#AnnotatedDims line 21_63">AnnotatedDims</button>
  <button class="modal-open" id="AnnotatedDimsEmpty_18_3" title="a definition with multiple references" data-urls="../../classes/MethodDeclarations.sdf3/#AnnotatedDimsEmpty line 34_34; ../../expressions/ArrayCreation.sdf3/#AnnotatedDimsEmpty line 20_75; ../../interfaces/AnnotationTypes.sdf3/#AnnotatedDimsEmpty line 38_62">AnnotatedDimsEmpty</button>
  <button class="modal-open" id="AnnotatedDim_19_3" title="a definition with multiple references" data-urls="#AnnotatedDim line 39_27, 40_27; ../../classes/FieldDeclarations.sdf3/#AnnotatedDim line 32_39, 65_70, 66_66">AnnotatedDim</button>

<span class="keyword">context-free syntax</span>

  <button class="modal-open" id="ReferenceType_23_3" title="a definition with multiple references" data-urls="../Main.sdf3/#ReferenceType line 20_10; ../ParameterizedTypes.sdf3/#ReferenceType line 18_18, 21_62, 22_58; ../../expressions/BinaryOperators.sdf3/#ReferenceType line 32_53; ../../expressions/MethodReference.sdf3/#ReferenceType line 14_40; ../../expressions/UnaryOperators.sdf3/#ReferenceType line 23_33">ReferenceType</button> = <a href="#ClassType_14_3" id="ClassType_23_19" title="a reference to a single-file definition">ClassType</a>
  <button class="modal-open" id="ReferenceType_24_3" title="a definition with multiple references" data-urls="../Main.sdf3/#ReferenceType line 20_10; ../ParameterizedTypes.sdf3/#ReferenceType line 18_18, 21_62, 22_58; ../../expressions/BinaryOperators.sdf3/#ReferenceType line 32_53; ../../expressions/MethodReference.sdf3/#ReferenceType line 14_40; ../../expressions/UnaryOperators.sdf3/#ReferenceType line 23_33">ReferenceType</button> = <a href="#ArrayType_16_3" id="ArrayType_24_19" title="a reference to a single-file definition">ArrayType</a>

  <button class="modal-open" id="ClassType_26_3" title="a definition with multiple references" data-urls="#ClassType line 23_19, 27_44, 38_36; ../TypeVariable.sdf3/#ClassType line 17_76; ../../classes/ClassDeclarations.sdf3/#ClassType line 54_37, 56_50; ../../classes/MethodDeclarations.sdf3/#ClassType line 43_22; ../../expressions/ArrayCreation.sdf3/#ClassType line 23_19; ../../expressions/MethodReference.sdf3/#ClassType line 18_39; ../../expressions/UnaryOperators.sdf3/#ClassType line 24_41; ../../interfaces/InterfaceDeclarations.sdf3/#ClassType line 41_52; ../../statements/Statements.sdf3/#ClassType line 108_37">ClassType</button>.<span class="cons_Constructor"><span id="ClassType_26_13" title="a definition with no references">ClassType</span></span>                  = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_26_45" title="a reference to a single-file definition">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_26_64" title="a reference to a single-file definition">Id</a>&gt;&lt;<a href="../ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_26_68" title="a reference to a single-file definition">TypeArguments</a>?&gt;&gt;
  <button class="modal-open" id="ClassType_27_3" title="a definition with multiple references" data-urls="#ClassType line 23_19, 27_44, 38_36; ../TypeVariable.sdf3/#ClassType line 17_76; ../../classes/ClassDeclarations.sdf3/#ClassType line 54_37, 56_50; ../../classes/MethodDeclarations.sdf3/#ClassType line 43_22; ../../expressions/ArrayCreation.sdf3/#ClassType line 23_19; ../../expressions/MethodReference.sdf3/#ClassType line 18_39; ../../expressions/UnaryOperators.sdf3/#ClassType line 24_41; ../../interfaces/InterfaceDeclarations.sdf3/#ClassType line 41_52; ../../statements/Statements.sdf3/#ClassType line 108_37">ClassType</button>.<span class="cons_Constructor"><span id="ClassOrInterfaceTypeMember_27_13" title="a definition with no references">ClassOrInterfaceTypeMember</span></span> = &lt;&lt;<a href="#ClassType_14_3" id="ClassType_27_44" title="a reference to a single-file definition">ClassType</a>&gt;<span class="cons_String">.</span>&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_27_57" title="a reference to a single-file definition">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_27_76" title="a reference to a single-file definition">Id</a>&gt;&lt;<a href="../ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_27_80" title="a reference to a single-file definition">TypeArguments</a>?&gt;&gt;
  
  <span class="layout">// The interfaceTypeMember will be ambiguous with ClassTypeMember</span>
  <span class="layout">// ClassType.InterfaceTypeMember = &lt;&lt;InterfaceType&gt;.&lt;{Annotation " "}*&gt; &lt;Id&gt;&lt;TypeArguments?&gt;&gt;</span>
  <span class="layout">// ReferenceType = InterfaceType  </span>
  <span class="layout">// InterfaceType.InterfaceType   = ClassType</span>
  
  <span class="layout">// Ambiguous with ClassType.ClassType</span>
  <span id="TypeVariable_35_3" title="a definition with no references">TypeVariable</span>.<span class="cons_Constructor"><span id="TypeVar_35_16" title="a definition with no references">TypeVar</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_35_29" title="a reference to a single-file definition">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_35_48" title="a reference to a single-file definition">Id</a>&gt;&gt;
  
  <button class="modal-open" id="ArrayType_37_3" title="a definition with multiple references" data-urls="#ArrayType line 24_19; ../../expressions/MethodReference.sdf3/#ArrayType line 19_39">ArrayType</button>.<span class="cons_Constructor"><span id="ArrayTypePrimitive_37_13" title="a definition with no references">ArrayTypePrimitive</span></span> = &lt;&lt;<a href="../PrimitiveTypes.sdf3/#PrimitiveType_10_3" id="PrimitiveType_37_36" title="a reference to a single-file definition">PrimitiveType</a>&gt; &lt;<a href="#AnnotatedDims_17_3" id="AnnotatedDims_37_52" title="a reference to a single-file definition">AnnotatedDims</a>&gt;&gt;
  <button class="modal-open" id="ArrayType_38_3" title="a definition with multiple references" data-urls="#ArrayType line 24_19; ../../expressions/MethodReference.sdf3/#ArrayType line 19_39">ArrayType</button>.<span class="cons_Constructor"><span id="ArrayTypeClassType_38_13" title="a definition with no references">ArrayTypeClassType</span></span> = &lt;&lt;<a href="#ClassType_14_3" id="ClassType_38_36" title="a reference to a single-file definition">ClassType</a>&gt; &lt;<a href="#AnnotatedDims_17_3" id="AnnotatedDims_38_48" title="a reference to a single-file definition">AnnotatedDims</a>&gt;&gt;
  <button class="modal-open" id="AnnotatedDims_39_3" title="a definition with multiple references" data-urls="#AnnotatedDims line 37_52, 38_48; ../../expressions/ArrayCreation.sdf3/#AnnotatedDims line 21_63">AnnotatedDims</button>      = &lt;&lt;{<a href="#AnnotatedDim_19_3" id="AnnotatedDim_39_27" title="a reference to a single-file definition">AnnotatedDim</a> <span class="cons_Lit">" "</span>}+&gt;&gt;
  <button class="modal-open" id="AnnotatedDimsEmpty_40_3" title="a definition with multiple references" data-urls="../../classes/MethodDeclarations.sdf3/#AnnotatedDimsEmpty line 34_34; ../../expressions/ArrayCreation.sdf3/#AnnotatedDimsEmpty line 20_75; ../../interfaces/AnnotationTypes.sdf3/#AnnotatedDimsEmpty line 38_62">AnnotatedDimsEmpty</button> = &lt;&lt;{<a href="#AnnotatedDim_19_3" id="AnnotatedDim_40_27" title="a reference to a single-file definition">AnnotatedDim</a> <span class="cons_Lit">" "</span>}*&gt;&gt;
  <button class="modal-open" id="AnnotatedDim_41_3" title="a definition with multiple references" data-urls="#AnnotatedDim line 39_27, 40_27; ../../classes/FieldDeclarations.sdf3/#AnnotatedDim line 32_39, 65_70, 66_66">AnnotatedDim</button>.<span class="cons_Constructor"><span id="AnnotateDim_41_16" title="a definition with no references">AnnotateDim</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_41_33" title="a reference to a single-file definition">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">[]</span>&gt;
  
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
