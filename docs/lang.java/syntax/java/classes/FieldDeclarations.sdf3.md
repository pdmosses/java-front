---
title: FieldDeclarations.sdf3
hide:
  - toc
---

# `FieldDeclarations.sdf3`

:simple-github: [pdmosses/java-front/lang.java/syntax/java/classes/FieldDeclarations.sdf3]

[pdmosses/java-front/lang.java/syntax/java/classes/FieldDeclarations.sdf3]: https://github.com/pdmosses/java-front/blob/master/lang.java/syntax/java/classes/FieldDeclarations.sdf3 "The source file on GitHub"

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
47
48
49
50
51
52
53
54
55
56
57
58
59
60
61
62
63
64
65
66
67
68
</pre></div></td>
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/classes/FieldDeclarations_1_8" title="Multi-file references" data-urls="../ClassDeclarations.sdf3/#java/classes/FieldDeclarations_10_3 line 10; ../Main.sdf3/#java/classes/FieldDeclarations_7_3 line 7; ../MethodDeclarations.sdf3/#java/classes/FieldDeclarations_5_3 line 5; ../../arrays/ArrayInitializers.sdf3/#java/classes/FieldDeclarations_6_3 line 6; ../../interfaces/AnnotationTypes.sdf3/#java/classes/FieldDeclarations_11_3 line 11; ../../interfaces/ConstantDeclarations.sdf3/#java/classes/FieldDeclarations_7_3 line 7; ../../statements/LocalVariableDeclarations.sdf3/#java/classes/FieldDeclarations_6_3 line 6; ../../statements/Statements.sdf3/#java/classes/FieldDeclarations_6_3 line 6">java/classes/FieldDeclarations</button>

<span class="layout">// 8.3. Field Declarations</span>

<span class="keyword">imports</span>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_6_3" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../../lexical/Modifiers.sdf3/#java/lexical/Modifiers_1_8" id="java/lexical/Modifiers_7_3" title="Defined at ../../lexical/Modifiers.sdf3 line 1">java/lexical/Modifiers</a>
  <a href="../../types/ReferenceTypes.sdf3/#java/types/ReferenceTypes_1_8" id="java/types/ReferenceTypes_8_3" title="Defined at ../../types/ReferenceTypes.sdf3 line 1">java/types/ReferenceTypes</a>
  <a href="../../types/PrimitiveTypes.sdf3/#java/types/PrimitiveTypes_1_8" id="java/types/PrimitiveTypes_9_3" title="Defined at ../../types/PrimitiveTypes.sdf3 line 1">java/types/PrimitiveTypes</a>
  <a href="../../types/ParameterizedTypes.sdf3/#java/types/ParameterizedTypes_1_8" id="java/types/ParameterizedTypes_10_3" title="Defined at ../../types/ParameterizedTypes.sdf3 line 1">java/types/ParameterizedTypes</a>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_1_8" id="java/interfaces/Annotations_11_3" title="Defined at ../../interfaces/Annotations.sdf3 line 1">java/interfaces/Annotations</a>
  <a href="../../arrays/ArrayInitializers.sdf3/#java/arrays/ArrayInitializers_1_8" id="java/arrays/ArrayInitializers_12_3" title="Defined at ../../arrays/ArrayInitializers.sdf3 line 1">java/arrays/ArrayInitializers</a>
  <a href="../../expressions/Main.sdf3/#java/expressions/Main_1_8" id="java/expressions/Main_13_3" title="Defined at ../../expressions/Main.sdf3 line 1">java/expressions/Main</a>

<span class="keyword">context-free sorts</span>

  <a href="../ClassDeclarations.sdf3/#FieldDeclaration_63_28" id="FieldDeclaration_17_3" title="Referenced at ../ClassDeclarations.sdf3 line 63">FieldDeclaration</a>
  <button class="modal-open" id="VarDeclId_18_3" title="Multi-file references" data-urls="#VarDeclId_33_35 line 33, 34; ../MethodDeclarations.sdf3/#VarDeclId_69_99 line 69, 71; ../../statements/Statements.sdf3/#VarDeclId_42_67 line 42, 106, 128">VarDeclId</button>
  <button class="modal-open" id="VarDecl_19_3" title="Multi-file references" data-urls="#VarDecl_30_70 line 30; ../../interfaces/ConstantDeclarations.sdf3/#VarDecl_18_43 line 18; ../../statements/LocalVariableDeclarations.sdf3/#VarDecl_19_43 line 19; ../../statements/Statements.sdf3/#VarDecl_45_63 line 45">VarDecl</button>
  <button class="modal-open" id="VariableInitializer_20_3" title="Multi-file references" data-urls="#VariableInitializer_33_49 line 33; ../../arrays/ArrayInitializers.sdf3/#VariableInitializer_14_41 line 14, 15">VariableInitializer</button>
  <a href="#FieldModifier_30_35" id="FieldModifier_21_3" title="Referenced at line 30">FieldModifier</a>
  <button class="modal-open" id="UnannType_22_3" title="Multi-file references" data-urls="#UnannType_30_57 line 30; ../MethodDeclarations.sdf3/#UnannType_39_12 line 39, 59, 60, 69, 71; ../../interfaces/AnnotationTypes.sdf3/#UnannType_38_43 line 38; ../../interfaces/ConstantDeclarations.sdf3/#UnannType_18_30 line 18; ../../statements/LocalVariableDeclarations.sdf3/#UnannType_19_30 line 19; ../../statements/Statements.sdf3/#UnannType_42_55 line 42, 45, 128">UnannType</button>
  <a href="#UnannPrimitiveType_50_15" id="UnannPrimitiveType_23_3" title="Referenced at line 50, 65">UnannPrimitiveType</a>
  <a href="#UnannReferenceType_51_15" id="UnannReferenceType_24_3" title="Referenced at line 51">UnannReferenceType</a>
  <button class="modal-open" id="UnannClassType_25_3" title="Multi-file references" data-urls="#UnannClassType_56_24 line 56, 60, 66; ../../statements/Statements.sdf3/#UnannClassType_107_27 line 107">UnannClassType</button>
  <a href="#UnannArrayType_57_24" id="UnannArrayType_26_3" title="Referenced at line 57">UnannArrayType</a>

<span class="keyword">context-free syntax</span>
  
  <a href="../ClassDeclarations.sdf3/#FieldDeclaration_63_28" id="FieldDeclaration_30_3" title="Referenced at ../ClassDeclarations.sdf3 line 63">FieldDeclaration</a>.<span class="cons_Constructor"><span id="FieldDecl_30_20" title="Not referenced">FieldDecl</span></span> = &lt;&lt;{<a href="#FieldModifier_21_3" id="FieldModifier_30_35" title="Defined at line 21, 39, 40, 41, 42, 43, 44, 45, 46">FieldModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="#UnannType_22_3" id="UnannType_30_57" title="Defined at line 22, 50, 51">UnannType</a>&gt; &lt;{<a href="#VarDecl_19_3" id="VarDecl_30_70" title="Defined at line 19, 33, 34">VarDecl</a> <span class="cons_Lit">", "</span>}+&gt;<span class="cons_String">;</span>&gt;
  <button class="modal-open" id="VarDeclId_31_3" title="Multi-file references" data-urls="#VarDeclId_33_35 line 33, 34; ../MethodDeclarations.sdf3/#VarDeclId_69_99 line 69, 71; ../../statements/Statements.sdf3/#VarDeclId_42_67 line 42, 106, 128">VarDeclId</button>.<span class="cons_Constructor"><span id="VariableDecl_31_13" title="Not referenced">VariableDecl</span></span>      = <a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_31_33" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>
  <button class="modal-open" id="VarDeclId_32_3" title="Multi-file references" data-urls="#VarDeclId_33_35 line 33, 34; ../MethodDeclarations.sdf3/#VarDeclId_69_99 line 69, 71; ../../statements/Statements.sdf3/#VarDeclId_42_67 line 42, 106, 128">VarDeclId</button>.<span class="cons_Constructor"><span id="VariableDeclArray_32_13" title="Not referenced">VariableDeclArray</span></span> = &lt;&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_32_35" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&lt;<a href="../../types/ReferenceTypes.sdf3/#AnnotatedDim_19_3" id="AnnotatedDim_32_39" title="Defined at ../../types/ReferenceTypes.sdf3 line 19, 41">AnnotatedDim</a>+&gt;&gt;
  <button class="modal-open" id="VarDecl_33_3" title="Multi-file references" data-urls="#VarDecl_30_70 line 30; ../../interfaces/ConstantDeclarations.sdf3/#VarDecl_18_43 line 18; ../../statements/LocalVariableDeclarations.sdf3/#VarDecl_19_43 line 19; ../../statements/Statements.sdf3/#VarDecl_45_63 line 45">VarDecl</button>.<span class="cons_Constructor"><span id="VariableDeclInit_33_11" title="Not referenced">VariableDeclInit</span></span>    = &lt;&lt;<a href="#VarDeclId_18_3" id="VarDeclId_33_35" title="Defined at line 18, 31, 32">VarDeclId</a>&gt; <span class="cons_String">=</span> &lt;<a href="#VariableInitializer_20_3" id="VariableInitializer_33_49" title="Defined at line 20, 36, 37">VariableInitializer</a>&gt;&gt;
  <button class="modal-open" id="VarDecl_34_3" title="Multi-file references" data-urls="#VarDecl_30_70 line 30; ../../interfaces/ConstantDeclarations.sdf3/#VarDecl_18_43 line 18; ../../statements/LocalVariableDeclarations.sdf3/#VarDecl_19_43 line 19; ../../statements/Statements.sdf3/#VarDecl_45_63 line 45">VarDecl</button>                     = <a href="#VarDeclId_18_3" id="VarDeclId_34_33" title="Defined at line 18, 31, 32">VarDeclId</a>
  
  <button class="modal-open" id="VariableInitializer_36_3" title="Multi-file references" data-urls="#VariableInitializer_33_49 line 33; ../../arrays/ArrayInitializers.sdf3/#VariableInitializer_14_41 line 14, 15">VariableInitializer</button> = <a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_36_25" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>
  <button class="modal-open" id="VariableInitializer_37_3" title="Multi-file references" data-urls="#VariableInitializer_33_49 line 33; ../../arrays/ArrayInitializers.sdf3/#VariableInitializer_14_41 line 14, 15">VariableInitializer</button> = <a href="../../arrays/ArrayInitializers.sdf3/#ArrayInitializer_10_3" id="ArrayInitializer_37_25" title="Defined at ../../arrays/ArrayInitializers.sdf3 line 10, 14, 15">ArrayInitializer</a>
  
  <a href="#FieldModifier_30_35" id="FieldModifier_39_3" title="Referenced at line 30">FieldModifier</a> = <a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_39_19" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a>
  <a href="#FieldModifier_30_35" id="FieldModifier_40_3" title="Referenced at line 30">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Public_14_3" id="Public_40_19" title="Defined at ../../lexical/Modifiers.sdf3 line 14, 29">Public</a>
  <a href="#FieldModifier_30_35" id="FieldModifier_41_3" title="Referenced at line 30">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Protected_13_3" id="Protected_41_19" title="Defined at ../../lexical/Modifiers.sdf3 line 13, 28">Protected</a>
  <a href="#FieldModifier_30_35" id="FieldModifier_42_3" title="Referenced at line 30">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Private_12_3" id="Private_42_19" title="Defined at ../../lexical/Modifiers.sdf3 line 12, 27">Private</a>
  <a href="#FieldModifier_30_35" id="FieldModifier_43_3" title="Referenced at line 30">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Static_15_3" id="Static_43_19" title="Defined at ../../lexical/Modifiers.sdf3 line 15, 30">Static</a>
  <a href="#FieldModifier_30_35" id="FieldModifier_44_3" title="Referenced at line 30">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Final_10_3" id="Final_44_19" title="Defined at ../../lexical/Modifiers.sdf3 line 10, 25">Final</a>
  <a href="#FieldModifier_30_35" id="FieldModifier_45_3" title="Referenced at line 30">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Transient_18_3" id="Transient_45_19" title="Defined at ../../lexical/Modifiers.sdf3 line 18, 32">Transient</a>
  <a href="#FieldModifier_30_35" id="FieldModifier_46_3" title="Referenced at line 30">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Volatile_19_3" id="Volatile_46_19" title="Defined at ../../lexical/Modifiers.sdf3 line 19, 33">Volatile</a>
  
<span class="keyword">context-free syntax</span>  
  
  <button class="modal-open" id="UnannType_50_3" title="Multi-file references" data-urls="#UnannType_30_57 line 30; ../MethodDeclarations.sdf3/#UnannType_39_12 line 39, 59, 60, 69, 71; ../../interfaces/AnnotationTypes.sdf3/#UnannType_38_43 line 38; ../../interfaces/ConstantDeclarations.sdf3/#UnannType_18_30 line 18; ../../statements/LocalVariableDeclarations.sdf3/#UnannType_19_30 line 19; ../../statements/Statements.sdf3/#UnannType_42_55 line 42, 45, 128">UnannType</button> = <a href="#UnannPrimitiveType_23_3" id="UnannPrimitiveType_50_15" title="Defined at line 23, 53, 54">UnannPrimitiveType</a>
  <button class="modal-open" id="UnannType_51_3" title="Multi-file references" data-urls="#UnannType_30_57 line 30; ../MethodDeclarations.sdf3/#UnannType_39_12 line 39, 59, 60, 69, 71; ../../interfaces/AnnotationTypes.sdf3/#UnannType_38_43 line 38; ../../interfaces/ConstantDeclarations.sdf3/#UnannType_18_30 line 18; ../../statements/LocalVariableDeclarations.sdf3/#UnannType_19_30 line 19; ../../statements/Statements.sdf3/#UnannType_42_55 line 42, 45, 128">UnannType</button> = <a href="#UnannReferenceType_24_3" id="UnannReferenceType_51_15" title="Defined at line 24, 56, 57">UnannReferenceType</a>
  
  <a href="#UnannPrimitiveType_50_15" id="UnannPrimitiveType_53_3" title="Referenced at line 50, 65">UnannPrimitiveType</a>.<span class="cons_Constructor"><span id="NumericType_53_22" title="Not referenced">NumericType</span></span> = <a href="../../types/PrimitiveTypes.sdf3/#NumericType_11_3" id="NumericType_53_36" title="Defined at ../../types/PrimitiveTypes.sdf3 line 11, 17, 18, 19, 20, 21, 22, 23">NumericType</a>
  <a href="#UnannPrimitiveType_50_15" id="UnannPrimitiveType_54_3" title="Referenced at line 50, 65">UnannPrimitiveType</a>.<span class="cons_Constructor"><span id="BooleanType_54_22" title="Not referenced">BooleanType</span></span> = <span class="cons_Lit">"boolean"</span>
  
  <a href="#UnannReferenceType_51_15" id="UnannReferenceType_56_3" title="Referenced at line 51">UnannReferenceType</a> = <a href="#UnannClassType_25_3" id="UnannClassType_56_24" title="Defined at line 25, 59, 60">UnannClassType</a>
  <a href="#UnannReferenceType_51_15" id="UnannReferenceType_57_3" title="Referenced at line 51">UnannReferenceType</a> = <a href="#UnannArrayType_26_3" id="UnannArrayType_57_24" title="Defined at line 26, 65, 66">UnannArrayType</a>
  
  <button class="modal-open" id="UnannClassType_59_3" title="Multi-file references" data-urls="#UnannClassType_56_24 line 56, 60, 66; ../../statements/Statements.sdf3/#UnannClassType_107_27 line 107">UnannClassType</button>.<span class="cons_Constructor"><span id="ClassType_59_18" title="Not referenced">ClassType</span></span>                       = &lt;&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_59_54" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&lt;<a href="../../types/ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_59_58" title="Defined at ../../types/ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>?&gt;&gt;
  <button class="modal-open" id="UnannClassType_60_3" title="Multi-file references" data-urls="#UnannClassType_56_24 line 56, 60, 66; ../../statements/Statements.sdf3/#UnannClassType_107_27 line 107">UnannClassType</button>.<span class="cons_Constructor"><span id="UnannClassOrInterfaceTypeMember_60_18" title="Not referenced">UnannClassOrInterfaceTypeMember</span></span> = &lt;&lt;<a href="#UnannClassType_25_3" id="UnannClassType_60_54" title="Defined at line 25, 59, 60">UnannClassType</a>&gt;<span class="cons_String">.</span>&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_60_72" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_60_91" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&lt;<a href="../../types/ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_60_95" title="Defined at ../../types/ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>?&gt;&gt;
  
<span class="layout">//  ambiguous with UnannClassType.ClassType</span>
<span class="layout">//  UnannTypeVariable.TypeVar            = Id</span>
  
  <a href="#UnannArrayType_57_24" id="UnannArrayType_65_3" title="Referenced at line 57">UnannArrayType</a>.<span class="cons_Constructor"><span id="UnannArrayTypePrimitive_65_18" title="Not referenced">UnannArrayTypePrimitive</span></span>    = &lt;&lt;<a href="#UnannPrimitiveType_23_3" id="UnannPrimitiveType_65_49" title="Defined at line 23, 53, 54">UnannPrimitiveType</a>&gt; &lt;<a href="../../types/ReferenceTypes.sdf3/#AnnotatedDim_19_3" id="AnnotatedDim_65_70" title="Defined at ../../types/ReferenceTypes.sdf3 line 19, 41">AnnotatedDim</a>+&gt;&gt;
  <a href="#UnannArrayType_57_24" id="UnannArrayType_66_3" title="Referenced at line 57">UnannArrayType</a>.<span class="cons_Constructor"><span id="UnannArrayTypeClassType_66_18" title="Not referenced">UnannArrayTypeClassType</span></span>    = &lt;&lt;<a href="#UnannClassType_25_3" id="UnannClassType_66_49" title="Defined at line 25, 59, 60">UnannClassType</a>&gt; &lt;<a href="../../types/ReferenceTypes.sdf3/#AnnotatedDim_19_3" id="AnnotatedDim_66_66" title="Defined at ../../types/ReferenceTypes.sdf3 line 19, 41">AnnotatedDim</a>+&gt;&gt;
  
  
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
