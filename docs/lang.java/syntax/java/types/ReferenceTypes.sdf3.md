---
title: ReferenceTypes.sdf3
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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../TypeVariable.sdf3#java/types/ReferenceTypes_66_91" id="java/types/ReferenceTypes_7_32" title="Referenced at ../TypeVariable.sdf3 line 6">java/types/ReferenceTypes</a>

<span class="layout">// 4.3. Reference Types and Values</span>

<span class="keyword">imports</span>
  <a href="../../lexical/Identifiers.sdf3#java/lexical/Identifiers_7_31" id="java/lexical/Identifiers_80_104" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../PrimitiveTypes.sdf3#java/types/PrimitiveTypes_7_32" id="java/types/PrimitiveTypes_107_132" title="Defined at ../PrimitiveTypes.sdf3 line 1">java/types/PrimitiveTypes</a>
  <a href="../ParameterizedTypes.sdf3#java/types/ParameterizedTypes_7_36" id="java/types/ParameterizedTypes_135_164" title="Defined at ../ParameterizedTypes.sdf3 line 1">java/types/ParameterizedTypes</a>
  <a href="../../interfaces/Annotations.sdf3#java/interfaces/Annotations_7_34" id="java/interfaces/Annotations_167_194" title="Defined at ../../interfaces/Annotations.sdf3 line 1">java/interfaces/Annotations</a>

<span class="keyword">context-free sorts</span>

  <a href="../Main.sdf3#ReferenceType_254_267" id="ReferenceType_218_231" title="Referenced at ../Main.sdf3 line 20; ../ParameterizedTypes.sdf3 line 22; ../../expressions/BinaryOperators.sdf3 line 32; ../../expressions/MethodReference.sdf3 line 14; ../../expressions/UnaryOperators.sdf3 line 23">ReferenceType</a>
  <a href="#ClassType_1033_1042" id="ClassType_234_243" title="Referenced at line 38; ../TypeVariable.sdf3 line 17; ../../classes/ClassDeclarations.sdf3 line 56; ../../classes/MethodDeclarations.sdf3 line 43; ../../expressions/ArrayCreation.sdf3 line 23; ../../expressions/MethodReference.sdf3 line 18; ../../expressions/UnaryOperators.sdf3 line 24; ../../interfaces/InterfaceDeclarations.sdf3 line 41; ../../statements/Statements.sdf3 line 108">ClassType</a>
  <span id="TypeVariable_246_258" title="Not referenced locally, nor via imports">TypeVariable</span>
  <a href="#ArrayType_391_400" id="ArrayType_261_270" title="Referenced at line 24; ../../expressions/MethodReference.sdf3 line 19">ArrayType</a>
  <a href="#AnnotatedDims_1045_1058" id="AnnotatedDims_273_286" title="Referenced at line 38; ../../expressions/ArrayCreation.sdf3 line 21">AnnotatedDims</a>
  <a href="../../classes/MethodDeclarations.sdf3#AnnotatedDimsEmpty_661_679" id="AnnotatedDimsEmpty_289_307" title="Referenced at ../../classes/MethodDeclarations.sdf3 line 34; ../../expressions/ArrayCreation.sdf3 line 20; ../../interfaces/AnnotationTypes.sdf3 line 38">AnnotatedDimsEmpty</a>
  <a href="#AnnotatedDim_1134_1146" id="AnnotatedDim_310_322" title="Referenced at line 40; ../../classes/FieldDeclarations.sdf3 line 66">AnnotatedDim</a>

<span class="keyword">context-free syntax</span>

  <a href="../Main.sdf3#ReferenceType_254_267" id="ReferenceType_347_360" title="Referenced at ../Main.sdf3 line 20; ../ParameterizedTypes.sdf3 line 22; ../../expressions/BinaryOperators.sdf3 line 32; ../../expressions/MethodReference.sdf3 line 14; ../../expressions/UnaryOperators.sdf3 line 23">ReferenceType</a> = <a href="#ClassType_234_243" id="ClassType_363_372" title="Defined at line 14, 26, 27">ClassType</a>
  <a href="../Main.sdf3#ReferenceType_254_267" id="ReferenceType_375_388" title="Referenced at ../Main.sdf3 line 20; ../ParameterizedTypes.sdf3 line 22; ../../expressions/BinaryOperators.sdf3 line 32; ../../expressions/MethodReference.sdf3 line 14; ../../expressions/UnaryOperators.sdf3 line 23">ReferenceType</a> = <a href="#ArrayType_261_270" id="ArrayType_391_400" title="Defined at line 16, 37, 38">ArrayType</a>

  <a href="#ClassType_1033_1042" id="ClassType_404_413" title="Referenced at line 38; ../TypeVariable.sdf3 line 17; ../../classes/ClassDeclarations.sdf3 line 56; ../../classes/MethodDeclarations.sdf3 line 43; ../../expressions/ArrayCreation.sdf3 line 23; ../../expressions/MethodReference.sdf3 line 18; ../../expressions/UnaryOperators.sdf3 line 24; ../../interfaces/InterfaceDeclarations.sdf3 line 41; ../../statements/Statements.sdf3 line 108">ClassType</a>.<span class="cons_Constructor"><span id="ClassType_414_423" title="Not referenced locally, nor via imports">ClassType</span></span>                  = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3#Annotation_158_168" id="Annotation_446_456" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_465_467" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&lt;<a href="../ParameterizedTypes.sdf3#TypeArguments_157_170" id="TypeArguments_469_482" title="Defined at ../ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>?&gt;&gt;
  <a href="#ClassType_1033_1042" id="ClassType_488_497" title="Referenced at line 38; ../TypeVariable.sdf3 line 17; ../../classes/ClassDeclarations.sdf3 line 56; ../../classes/MethodDeclarations.sdf3 line 43; ../../expressions/ArrayCreation.sdf3 line 23; ../../expressions/MethodReference.sdf3 line 18; ../../expressions/UnaryOperators.sdf3 line 24; ../../interfaces/InterfaceDeclarations.sdf3 line 41; ../../statements/Statements.sdf3 line 108">ClassType</a>.<span class="cons_Constructor"><span id="ClassOrInterfaceTypeMember_498_524" title="Not referenced locally, nor via imports">ClassOrInterfaceTypeMember</span></span> = &lt;&lt;<a href="#ClassType_234_243" id="ClassType_529_538" title="Defined at line 14, 26, 27">ClassType</a>&gt;<span class="cons_String">.</span>&lt;{<a href="../../interfaces/Annotations.sdf3#Annotation_158_168" id="Annotation_542_552" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_561_563" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&lt;<a href="../ParameterizedTypes.sdf3#TypeArguments_157_170" id="TypeArguments_565_578" title="Defined at ../ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>?&gt;&gt;
  
  <span class="layout">// The interfaceTypeMember will be ambiguous with ClassTypeMember</span>
  <span class="layout">// ClassType.InterfaceTypeMember = &lt;&lt;InterfaceType&gt;.&lt;{Annotation " "}*&gt; &lt;Id&gt;&lt;TypeArguments?&gt;&gt;</span>
  <span class="layout">// ReferenceType = InterfaceType  </span>
  <span class="layout">// InterfaceType.InterfaceType   = ClassType</span>
  
  <span class="layout">// Ambiguous with ClassType.ClassType</span>
  <span id="TypeVariable_878_890" title="Not referenced locally, nor via imports">TypeVariable</span>.<span class="cons_Constructor"><span id="TypeVar_891_898" title="Not referenced locally, nor via imports">TypeVar</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3#Annotation_158_168" id="Annotation_904_914" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_923_925" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&gt;
  
  <a href="#ArrayType_391_400" id="ArrayType_933_942" title="Referenced at line 24; ../../expressions/MethodReference.sdf3 line 19">ArrayType</a>.<span class="cons_Constructor"><span id="ArrayTypePrimitive_943_961" title="Not referenced locally, nor via imports">ArrayTypePrimitive</span></span> = &lt;&lt;<a href="../PrimitiveTypes.sdf3#PrimitiveType_131_144" id="PrimitiveType_966_979" title="Defined at ../PrimitiveTypes.sdf3 line 10, 15, 16">PrimitiveType</a>&gt; &lt;<a href="#AnnotatedDims_273_286" id="AnnotatedDims_982_995" title="Defined at line 17, 39">AnnotatedDims</a>&gt;&gt;
  <a href="#ArrayType_391_400" id="ArrayType_1000_1009" title="Referenced at line 24; ../../expressions/MethodReference.sdf3 line 19">ArrayType</a>.<span class="cons_Constructor"><span id="ArrayTypeClassType_1010_1028" title="Not referenced locally, nor via imports">ArrayTypeClassType</span></span> = &lt;&lt;<a href="#ClassType_234_243" id="ClassType_1033_1042" title="Defined at line 14, 26, 27">ClassType</a>&gt; &lt;<a href="#AnnotatedDims_273_286" id="AnnotatedDims_1045_1058" title="Defined at line 17, 39">AnnotatedDims</a>&gt;&gt;
  <a href="#AnnotatedDims_1045_1058" id="AnnotatedDims_1063_1076" title="Referenced at line 38; ../../expressions/ArrayCreation.sdf3 line 21">AnnotatedDims</a>      = &lt;&lt;{<a href="#AnnotatedDim_310_322" id="AnnotatedDim_1087_1099" title="Defined at line 19, 41">AnnotatedDim</a> <span class="cons_Lit">" "</span>}+&gt;&gt;
  <a href="../../classes/MethodDeclarations.sdf3#AnnotatedDimsEmpty_661_679" id="AnnotatedDimsEmpty_1110_1128" title="Referenced at ../../classes/MethodDeclarations.sdf3 line 34; ../../expressions/ArrayCreation.sdf3 line 20; ../../interfaces/AnnotationTypes.sdf3 line 38">AnnotatedDimsEmpty</a> = &lt;&lt;{<a href="#AnnotatedDim_310_322" id="AnnotatedDim_1134_1146" title="Defined at line 19, 41">AnnotatedDim</a> <span class="cons_Lit">" "</span>}*&gt;&gt;
  <a href="#AnnotatedDim_1134_1146" id="AnnotatedDim_1157_1169" title="Referenced at line 40; ../../classes/FieldDeclarations.sdf3 line 66">AnnotatedDim</a>.<span class="cons_Constructor"><span id="AnnotateDim_1170_1181" title="Not referenced locally, nor via imports">AnnotateDim</span></span> = &lt;&lt;{<a href="../../interfaces/Annotations.sdf3#Annotation_158_168" id="Annotation_1187_1197" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; <span class="cons_String">[]</span>&gt;
  
<span class="keyword">template options</span>

  <span class="keyword">tokenize</span> : "["
  
</code></pre></td></tr></tbody></table></div>