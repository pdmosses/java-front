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
<td class="code"><pre><code><span class="keyword">module</span> <button class="modal-open" id="java/classes/FieldDeclarations_1_8" title="a definition with multiple references" data-urls="../ClassDeclarations.sdf3/#java/classes/FieldDeclarations line 10_3; ../Main.sdf3/#java/classes/FieldDeclarations line 7_3; ../MethodDeclarations.sdf3/#java/classes/FieldDeclarations line 5_3; ../../arrays/ArrayInitializers.sdf3/#java/classes/FieldDeclarations line 6_3; ../../interfaces/AnnotationTypes.sdf3/#java/classes/FieldDeclarations line 11_3; ../../interfaces/ConstantDeclarations.sdf3/#java/classes/FieldDeclarations line 7_3; ../../statements/LocalVariableDeclarations.sdf3/#java/classes/FieldDeclarations line 6_3; ../../statements/Statements.sdf3/#java/classes/FieldDeclarations line 6_3">java/classes/FieldDeclarations</button>

<span class="layout">// 8.3. Field Declarations</span>

<span class="keyword">imports</span>
  <a href="../../lexical/Identifiers.sdf3/#java/lexical/Identifiers_1_8" id="java/lexical/Identifiers_6_3" title="a reference to a single-file definition">java/lexical/Identifiers</a>
  <a href="../../lexical/Modifiers.sdf3/#java/lexical/Modifiers_1_8" id="java/lexical/Modifiers_7_3" title="a reference to a single-file definition">java/lexical/Modifiers</a>
  <a href="../../types/ReferenceTypes.sdf3/#java/types/ReferenceTypes_1_8" id="java/types/ReferenceTypes_8_3" title="a reference to a single-file definition">java/types/ReferenceTypes</a>
  <a href="../../types/PrimitiveTypes.sdf3/#java/types/PrimitiveTypes_1_8" id="java/types/PrimitiveTypes_9_3" title="a reference to a single-file definition">java/types/PrimitiveTypes</a>
  <a href="../../types/ParameterizedTypes.sdf3/#java/types/ParameterizedTypes_1_8" id="java/types/ParameterizedTypes_10_3" title="a reference to a single-file definition">java/types/ParameterizedTypes</a>
  <a href="../../interfaces/Annotations.sdf3/#java/interfaces/Annotations_1_8" id="java/interfaces/Annotations_11_3" title="a reference to a single-file definition">java/interfaces/Annotations</a>
  <a href="../../arrays/ArrayInitializers.sdf3/#java/arrays/ArrayInitializers_1_8" id="java/arrays/ArrayInitializers_12_3" title="a reference to a single-file definition">java/arrays/ArrayInitializers</a>
  <a href="../../expressions/Main.sdf3/#java/expressions/Main_1_8" id="java/expressions/Main_13_3" title="a reference to a single-file definition">java/expressions/Main</a>

<span class="keyword">context-free sorts</span>

  <a href="../ClassDeclarations.sdf3/#FieldDeclaration_63_28" id="FieldDeclaration_17_3" title="a definition with a single reference">FieldDeclaration</a>
  <button class="modal-open" id="VarDeclId_18_3" title="a definition with multiple references" data-urls="#VarDeclId line 33_35, 34_33; ../MethodDeclarations.sdf3/#VarDeclId line 69_99, 71_69; ../../statements/Statements.sdf3/#VarDeclId line 42_67, 106_77, 128_63">VarDeclId</button>
  <button class="modal-open" id="VarDecl_19_3" title="a definition with multiple references" data-urls="#VarDecl line 30_70; ../../interfaces/ConstantDeclarations.sdf3/#VarDecl line 18_43; ../../statements/LocalVariableDeclarations.sdf3/#VarDecl line 19_43; ../../statements/Statements.sdf3/#VarDecl line 45_63">VarDecl</button>
  <button class="modal-open" id="VariableInitializer_20_3" title="a definition with multiple references" data-urls="#VariableInitializer line 33_49; ../../arrays/ArrayInitializers.sdf3/#VariableInitializer line 14_41, 15_41">VariableInitializer</button>
  <a href="#FieldModifier_30_35" id="FieldModifier_21_3" title="a definition with a single reference">FieldModifier</a>
  <button class="modal-open" id="UnannType_22_3" title="a definition with multiple references" data-urls="#UnannType line 30_57; ../MethodDeclarations.sdf3/#UnannType line 39_12, 59_59, 60_59, 69_63, 71_57; ../../interfaces/AnnotationTypes.sdf3/#UnannType line 38_43; ../../interfaces/ConstantDeclarations.sdf3/#UnannType line 18_30; ../../statements/LocalVariableDeclarations.sdf3/#UnannType line 19_30; ../../statements/Statements.sdf3/#UnannType line 42_55, 45_50, 128_51">UnannType</button>
  <button class="modal-open" id="UnannPrimitiveType_23_3" title="a definition with multiple references" data-urls="#UnannPrimitiveType line 50_15, 65_49">UnannPrimitiveType</button>
  <a href="#UnannReferenceType_51_15" id="UnannReferenceType_24_3" title="a definition with a single reference">UnannReferenceType</a>
  <button class="modal-open" id="UnannClassType_25_3" title="a definition with multiple references" data-urls="#UnannClassType line 56_24, 60_54, 66_49; ../../statements/Statements.sdf3/#UnannClassType line 107_27">UnannClassType</button>
  <a href="#UnannArrayType_57_24" id="UnannArrayType_26_3" title="a definition with a single reference">UnannArrayType</a>

<span class="keyword">context-free syntax</span>
  
  <a href="../ClassDeclarations.sdf3/#FieldDeclaration_63_28" id="FieldDeclaration_30_3" title="a definition with a single reference">FieldDeclaration</a>.<span class="cons_Constructor"><span id="FieldDecl_30_20" title="a definition with no references">FieldDecl</span></span> = &lt;&lt;{<a href="#FieldModifier_21_3" id="FieldModifier_30_35" title="a reference to a single-file definition">FieldModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="#UnannType_22_3" id="UnannType_30_57" title="a reference to a single-file definition">UnannType</a>&gt; &lt;{<a href="#VarDecl_19_3" id="VarDecl_30_70" title="a reference to a single-file definition">VarDecl</a> <span class="cons_Lit">", "</span>}+&gt;<span class="cons_String">;</span>&gt;
  <button class="modal-open" id="VarDeclId_31_3" title="a definition with multiple references" data-urls="#VarDeclId line 33_35, 34_33; ../MethodDeclarations.sdf3/#VarDeclId line 69_99, 71_69; ../../statements/Statements.sdf3/#VarDeclId line 42_67, 106_77, 128_63">VarDeclId</button>.<span class="cons_Constructor"><span id="VariableDecl_31_13" title="a definition with no references">VariableDecl</span></span>      = <a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_31_33" title="a reference to a single-file definition">Id</a>
  <button class="modal-open" id="VarDeclId_32_3" title="a definition with multiple references" data-urls="#VarDeclId line 33_35, 34_33; ../MethodDeclarations.sdf3/#VarDeclId line 69_99, 71_69; ../../statements/Statements.sdf3/#VarDeclId line 42_67, 106_77, 128_63">VarDeclId</button>.<span class="cons_Constructor"><span id="VariableDeclArray_32_13" title="a definition with no references">VariableDeclArray</span></span> = &lt;&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_32_35" title="a reference to a single-file definition">Id</a>&gt;&lt;<a href="../../types/ReferenceTypes.sdf3/#AnnotatedDim_19_3" id="AnnotatedDim_32_39" title="a reference to a single-file definition">AnnotatedDim</a>+&gt;&gt;
  <button class="modal-open" id="VarDecl_33_3" title="a definition with multiple references" data-urls="#VarDecl line 30_70; ../../interfaces/ConstantDeclarations.sdf3/#VarDecl line 18_43; ../../statements/LocalVariableDeclarations.sdf3/#VarDecl line 19_43; ../../statements/Statements.sdf3/#VarDecl line 45_63">VarDecl</button>.<span class="cons_Constructor"><span id="VariableDeclInit_33_11" title="a definition with no references">VariableDeclInit</span></span>    = &lt;&lt;<a href="#VarDeclId_18_3" id="VarDeclId_33_35" title="a reference to a single-file definition">VarDeclId</a>&gt; <span class="cons_String">=</span> &lt;<a href="#VariableInitializer_20_3" id="VariableInitializer_33_49" title="a reference to a single-file definition">VariableInitializer</a>&gt;&gt;
  <button class="modal-open" id="VarDecl_34_3" title="a definition with multiple references" data-urls="#VarDecl line 30_70; ../../interfaces/ConstantDeclarations.sdf3/#VarDecl line 18_43; ../../statements/LocalVariableDeclarations.sdf3/#VarDecl line 19_43; ../../statements/Statements.sdf3/#VarDecl line 45_63">VarDecl</button>                     = <a href="#VarDeclId_18_3" id="VarDeclId_34_33" title="a reference to a single-file definition">VarDeclId</a>
  
  <button class="modal-open" id="VariableInitializer_36_3" title="a definition with multiple references" data-urls="#VariableInitializer line 33_49; ../../arrays/ArrayInitializers.sdf3/#VariableInitializer line 14_41, 15_41">VariableInitializer</button> = <a href="../../expressions/Main.sdf3/#Expression_21_3" id="Expression_36_25" title="a reference to a single-file definition">Expression</a>
  <button class="modal-open" id="VariableInitializer_37_3" title="a definition with multiple references" data-urls="#VariableInitializer line 33_49; ../../arrays/ArrayInitializers.sdf3/#VariableInitializer line 14_41, 15_41">VariableInitializer</button> = <a href="../../arrays/ArrayInitializers.sdf3/#ArrayInitializer_10_3" id="ArrayInitializer_37_25" title="a reference to a single-file definition">ArrayInitializer</a>
  
  <a href="#FieldModifier_30_35" id="FieldModifier_39_3" title="a definition with a single reference">FieldModifier</a> = <a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_39_19" title="a reference to a single-file definition">Annotation</a>
  <a href="#FieldModifier_30_35" id="FieldModifier_40_3" title="a definition with a single reference">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Public_14_3" id="Public_40_19" title="a reference to a single-file definition">Public</a>
  <a href="#FieldModifier_30_35" id="FieldModifier_41_3" title="a definition with a single reference">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Protected_13_3" id="Protected_41_19" title="a reference to a single-file definition">Protected</a>
  <a href="#FieldModifier_30_35" id="FieldModifier_42_3" title="a definition with a single reference">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Private_12_3" id="Private_42_19" title="a reference to a single-file definition">Private</a>
  <a href="#FieldModifier_30_35" id="FieldModifier_43_3" title="a definition with a single reference">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Static_15_3" id="Static_43_19" title="a reference to a single-file definition">Static</a>
  <a href="#FieldModifier_30_35" id="FieldModifier_44_3" title="a definition with a single reference">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Final_10_3" id="Final_44_19" title="a reference to a single-file definition">Final</a>
  <a href="#FieldModifier_30_35" id="FieldModifier_45_3" title="a definition with a single reference">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Transient_18_3" id="Transient_45_19" title="a reference to a single-file definition">Transient</a>
  <a href="#FieldModifier_30_35" id="FieldModifier_46_3" title="a definition with a single reference">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3/#Volatile_19_3" id="Volatile_46_19" title="a reference to a single-file definition">Volatile</a>
  
<span class="keyword">context-free syntax</span>  
  
  <button class="modal-open" id="UnannType_50_3" title="a definition with multiple references" data-urls="#UnannType line 30_57; ../MethodDeclarations.sdf3/#UnannType line 39_12, 59_59, 60_59, 69_63, 71_57; ../../interfaces/AnnotationTypes.sdf3/#UnannType line 38_43; ../../interfaces/ConstantDeclarations.sdf3/#UnannType line 18_30; ../../statements/LocalVariableDeclarations.sdf3/#UnannType line 19_30; ../../statements/Statements.sdf3/#UnannType line 42_55, 45_50, 128_51">UnannType</button> = <a href="#UnannPrimitiveType_23_3" id="UnannPrimitiveType_50_15" title="a reference to a single-file definition">UnannPrimitiveType</a>
  <button class="modal-open" id="UnannType_51_3" title="a definition with multiple references" data-urls="#UnannType line 30_57; ../MethodDeclarations.sdf3/#UnannType line 39_12, 59_59, 60_59, 69_63, 71_57; ../../interfaces/AnnotationTypes.sdf3/#UnannType line 38_43; ../../interfaces/ConstantDeclarations.sdf3/#UnannType line 18_30; ../../statements/LocalVariableDeclarations.sdf3/#UnannType line 19_30; ../../statements/Statements.sdf3/#UnannType line 42_55, 45_50, 128_51">UnannType</button> = <a href="#UnannReferenceType_24_3" id="UnannReferenceType_51_15" title="a reference to a single-file definition">UnannReferenceType</a>
  
  <button class="modal-open" id="UnannPrimitiveType_53_3" title="a definition with multiple references" data-urls="#UnannPrimitiveType line 50_15, 65_49">UnannPrimitiveType</button>.<span class="cons_Constructor"><span id="NumericType_53_22" title="a definition with no references">NumericType</span></span> = <a href="../../types/PrimitiveTypes.sdf3/#NumericType_11_3" id="NumericType_53_36" title="a reference to a single-file definition">NumericType</a>
  <button class="modal-open" id="UnannPrimitiveType_54_3" title="a definition with multiple references" data-urls="#UnannPrimitiveType line 50_15, 65_49">UnannPrimitiveType</button>.<span class="cons_Constructor"><span id="BooleanType_54_22" title="a definition with no references">BooleanType</span></span> = <span class="cons_Lit">"boolean"</span>
  
  <a href="#UnannReferenceType_51_15" id="UnannReferenceType_56_3" title="a definition with a single reference">UnannReferenceType</a> = <a href="#UnannClassType_25_3" id="UnannClassType_56_24" title="a reference to a single-file definition">UnannClassType</a>
  <a href="#UnannReferenceType_51_15" id="UnannReferenceType_57_3" title="a definition with a single reference">UnannReferenceType</a> = <a href="#UnannArrayType_26_3" id="UnannArrayType_57_24" title="a reference to a single-file definition">UnannArrayType</a>
  
  <button class="modal-open" id="UnannClassType_59_3" title="a definition with multiple references" data-urls="#UnannClassType line 56_24, 60_54, 66_49; ../../statements/Statements.sdf3/#UnannClassType line 107_27">UnannClassType</button>.<span class="cons_Constructor"><span id="ClassType_59_18" title="a definition with no references">ClassType</span></span>                       = &lt;&lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_59_54" title="a reference to a single-file definition">Id</a>&gt;&lt;<a href="../../types/ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_59_58" title="a reference to a single-file definition">TypeArguments</a>?&gt;&gt;
  <button class="modal-open" id="UnannClassType_60_3" title="a definition with multiple references" data-urls="#UnannClassType line 56_24, 60_54, 66_49; ../../statements/Statements.sdf3/#UnannClassType line 107_27">UnannClassType</button>.<span class="cons_Constructor"><span id="UnannClassOrInterfaceTypeMember_60_18" title="a definition with no references">UnannClassOrInterfaceTypeMember</span></span> = &lt;&lt;<a href="#UnannClassType_25_3" id="UnannClassType_60_54" title="a reference to a single-file definition">UnannClassType</a>&gt;<span class="cons_String">.</span>&lt;{<a href="../../interfaces/Annotations.sdf3/#Annotation_12_3" id="Annotation_60_72" title="a reference to a single-file definition">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3/#Id_15_3" id="Id_60_91" title="a reference to a single-file definition">Id</a>&gt;&lt;<a href="../../types/ParameterizedTypes.sdf3/#TypeArguments_11_3" id="TypeArguments_60_95" title="a reference to a single-file definition">TypeArguments</a>?&gt;&gt;
  
<span class="layout">//  ambiguous with UnannClassType.ClassType</span>
<span class="layout">//  UnannTypeVariable.TypeVar            = Id</span>
  
  <a href="#UnannArrayType_57_24" id="UnannArrayType_65_3" title="a definition with a single reference">UnannArrayType</a>.<span class="cons_Constructor"><span id="UnannArrayTypePrimitive_65_18" title="a definition with no references">UnannArrayTypePrimitive</span></span>    = &lt;&lt;<a href="#UnannPrimitiveType_23_3" id="UnannPrimitiveType_65_49" title="a reference to a single-file definition">UnannPrimitiveType</a>&gt; &lt;<a href="../../types/ReferenceTypes.sdf3/#AnnotatedDim_19_3" id="AnnotatedDim_65_70" title="a reference to a single-file definition">AnnotatedDim</a>+&gt;&gt;
  <a href="#UnannArrayType_57_24" id="UnannArrayType_66_3" title="a definition with a single reference">UnannArrayType</a>.<span class="cons_Constructor"><span id="UnannArrayTypeClassType_66_18" title="a definition with no references">UnannArrayTypeClassType</span></span>    = &lt;&lt;<a href="#UnannClassType_25_3" id="UnannClassType_66_49" title="a reference to a single-file definition">UnannClassType</a>&gt; &lt;<a href="../../types/ReferenceTypes.sdf3/#AnnotatedDim_19_3" id="AnnotatedDim_66_66" title="a reference to a single-file definition">AnnotatedDim</a>+&gt;&gt;
  
  
</code></pre></td></tr></tbody></table></div>

<div id="modal">
  <div id="modal-content">
    <span id="modal-close">&times;</span>
    <h2 id="modal-h2"></h2>
    <p  id="modal-p"></p>
    <ul id="modal-ul"></ul>
  </div>
</div>
