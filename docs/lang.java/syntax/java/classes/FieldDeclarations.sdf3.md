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
<td class="code"><pre><code><span class="keyword">module</span> <a href="../../statements/Statements.sdf3#java/classes/FieldDeclarations_66_96" id="java/classes/FieldDeclarations_7_37" title="Referenced at ../../statements/Statements.sdf3 line 6">java/classes/FieldDeclarations</a>

<span class="layout">// 8.3. Field Declarations</span>

<span class="keyword">imports</span>
  <a href="../../lexical/Identifiers.sdf3#java/lexical/Identifiers_7_31" id="java/lexical/Identifiers_77_101" title="Defined at ../../lexical/Identifiers.sdf3 line 1">java/lexical/Identifiers</a>
  <a href="../../lexical/Modifiers.sdf3#java/lexical/Modifiers_7_29" id="java/lexical/Modifiers_104_126" title="Defined at ../../lexical/Modifiers.sdf3 line 1">java/lexical/Modifiers</a>
  <a href="../../types/ReferenceTypes.sdf3#java/types/ReferenceTypes_7_32" id="java/types/ReferenceTypes_129_154" title="Defined at ../../types/ReferenceTypes.sdf3 line 1">java/types/ReferenceTypes</a>
  <a href="../../types/PrimitiveTypes.sdf3#java/types/PrimitiveTypes_7_32" id="java/types/PrimitiveTypes_157_182" title="Defined at ../../types/PrimitiveTypes.sdf3 line 1">java/types/PrimitiveTypes</a>
  <a href="../../types/ParameterizedTypes.sdf3#java/types/ParameterizedTypes_7_36" id="java/types/ParameterizedTypes_185_214" title="Defined at ../../types/ParameterizedTypes.sdf3 line 1">java/types/ParameterizedTypes</a>
  <a href="../../interfaces/Annotations.sdf3#java/interfaces/Annotations_7_34" id="java/interfaces/Annotations_217_244" title="Defined at ../../interfaces/Annotations.sdf3 line 1">java/interfaces/Annotations</a>
  <a href="../../arrays/ArrayInitializers.sdf3#java/arrays/ArrayInitializers_7_36" id="java/arrays/ArrayInitializers_247_276" title="Defined at ../../arrays/ArrayInitializers.sdf3 line 1">java/arrays/ArrayInitializers</a>
  <a href="../../expressions/Main.sdf3#java/expressions/Main_7_28" id="java/expressions/Main_279_300" title="Defined at ../../expressions/Main.sdf3 line 1">java/expressions/Main</a>

<span class="keyword">context-free sorts</span>

  <a href="../ClassDeclarations.sdf3#FieldDeclaration_1648_1664" id="FieldDeclaration_324_340" title="Referenced at ../ClassDeclarations.sdf3 line 63">FieldDeclaration</a>
  <a href="#VarDeclId_791_800" id="VarDeclId_343_352" title="Referenced at line 34; ../MethodDeclarations.sdf3 line 71; ../../statements/Statements.sdf3 line 128">VarDeclId</a>
  <a href="#VarDecl_582_589" id="VarDecl_355_362" title="Referenced at line 30; ../../interfaces/ConstantDeclarations.sdf3 line 18; ../../statements/LocalVariableDeclarations.sdf3 line 19; ../../statements/Statements.sdf3 line 45">VarDecl</a>
  <a href="#VariableInitializer_737_756" id="VariableInitializer_365_384" title="Referenced at line 33; ../../arrays/ArrayInitializers.sdf3 line 15">VariableInitializer</a>
  <a href="#FieldModifier_547_560" id="FieldModifier_387_400" title="Referenced at line 30">FieldModifier</a>
  <a href="#UnannType_569_578" id="UnannType_403_412" title="Referenced at line 30; ../MethodDeclarations.sdf3 line 71; ../../interfaces/AnnotationTypes.sdf3 line 38; ../../interfaces/ConstantDeclarations.sdf3 line 18; ../../statements/LocalVariableDeclarations.sdf3 line 19; ../../statements/Statements.sdf3 line 128">UnannType</a>
  <a href="#UnannPrimitiveType_1695_1713" id="UnannPrimitiveType_415_433" title="Referenced at line 65">UnannPrimitiveType</a>
  <a href="#UnannReferenceType_1170_1188" id="UnannReferenceType_436_454" title="Referenced at line 51">UnannReferenceType</a>
  <a href="#UnannClassType_1780_1794" id="UnannClassType_457_471" title="Referenced at line 66; ../../statements/Statements.sdf3 line 107">UnannClassType</a>
  <a href="#UnannArrayType_1348_1362" id="UnannArrayType_474_488" title="Referenced at line 57">UnannArrayType</a>

<span class="keyword">context-free syntax</span>
  
  <a href="../ClassDeclarations.sdf3#FieldDeclaration_1648_1664" id="FieldDeclaration_515_531" title="Referenced at ../ClassDeclarations.sdf3 line 63">FieldDeclaration</a>.<span class="cons_Constructor"><span id="FieldDecl_532_541" title="Not referenced locally, nor via imports">FieldDecl</span></span> = &lt;&lt;{<a href="#FieldModifier_387_400" id="FieldModifier_547_560" title="Defined at line 21, 39, 40, 41, 42, 43, 44, 45, 46">FieldModifier</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="#UnannType_403_412" id="UnannType_569_578" title="Defined at line 22, 50, 51">UnannType</a>&gt; &lt;{<a href="#VarDecl_355_362" id="VarDecl_582_589" title="Defined at line 19, 33, 34">VarDecl</a> <span class="cons_Lit">", "</span>}+&gt;<span class="cons_String">;</span>&gt;
  <a href="#VarDeclId_791_800" id="VarDeclId_602_611" title="Referenced at line 34; ../MethodDeclarations.sdf3 line 71; ../../statements/Statements.sdf3 line 128">VarDeclId</a>.<span class="cons_Constructor"><span id="VariableDecl_612_624" title="Not referenced locally, nor via imports">VariableDecl</span></span>      = <a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_632_634" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>
  <a href="#VarDeclId_791_800" id="VarDeclId_637_646" title="Referenced at line 34; ../MethodDeclarations.sdf3 line 71; ../../statements/Statements.sdf3 line 128">VarDeclId</a>.<span class="cons_Constructor"><span id="VariableDeclArray_647_664" title="Not referenced locally, nor via imports">VariableDeclArray</span></span> = &lt;&lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_669_671" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&lt;<a href="../../types/ReferenceTypes.sdf3#AnnotatedDim_310_322" id="AnnotatedDim_673_685" title="Defined at ../../types/ReferenceTypes.sdf3 line 19, 41">AnnotatedDim</a>+&gt;&gt;
  <a href="#VarDecl_582_589" id="VarDecl_691_698" title="Referenced at line 30; ../../interfaces/ConstantDeclarations.sdf3 line 18; ../../statements/LocalVariableDeclarations.sdf3 line 19; ../../statements/Statements.sdf3 line 45">VarDecl</a>.<span class="cons_Constructor"><span id="VariableDeclInit_699_715" title="Not referenced locally, nor via imports">VariableDeclInit</span></span>    = &lt;&lt;<a href="#VarDeclId_343_352" id="VarDeclId_723_732" title="Defined at line 18, 31, 32">VarDeclId</a>&gt; <span class="cons_String">=</span> &lt;<a href="#VariableInitializer_365_384" id="VariableInitializer_737_756" title="Defined at line 20, 36, 37">VariableInitializer</a>&gt;&gt;
  <a href="#VarDecl_582_589" id="VarDecl_761_768" title="Referenced at line 30; ../../interfaces/ConstantDeclarations.sdf3 line 18; ../../statements/LocalVariableDeclarations.sdf3 line 19; ../../statements/Statements.sdf3 line 45">VarDecl</a>                     = <a href="#VarDeclId_343_352" id="VarDeclId_791_800" title="Defined at line 18, 31, 32">VarDeclId</a>
  
  <a href="#VariableInitializer_737_756" id="VariableInitializer_806_825" title="Referenced at line 33; ../../arrays/ArrayInitializers.sdf3 line 15">VariableInitializer</a> = <a href="../../expressions/Main.sdf3#Expression_459_469" id="Expression_828_838" title="Defined at ../../expressions/Main.sdf3 line 21">Expression</a>
  <a href="#VariableInitializer_737_756" id="VariableInitializer_841_860" title="Referenced at line 33; ../../arrays/ArrayInitializers.sdf3 line 15">VariableInitializer</a> = <a href="../../arrays/ArrayInitializers.sdf3#ArrayInitializer_133_149" id="ArrayInitializer_863_879" title="Defined at ../../arrays/ArrayInitializers.sdf3 line 10, 14, 15">ArrayInitializer</a>
  
  <a href="#FieldModifier_547_560" id="FieldModifier_885_898" title="Referenced at line 30">FieldModifier</a> = <a href="../../interfaces/Annotations.sdf3#Annotation_158_168" id="Annotation_901_911" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a>
  <a href="#FieldModifier_547_560" id="FieldModifier_914_927" title="Referenced at line 30">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3#Public_201_207" id="Public_930_936" title="Defined at ../../lexical/Modifiers.sdf3 line 14, 29">Public</a>
  <a href="#FieldModifier_547_560" id="FieldModifier_939_952" title="Referenced at line 30">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3#Protected_189_198" id="Protected_955_964" title="Defined at ../../lexical/Modifiers.sdf3 line 13, 28">Protected</a>
  <a href="#FieldModifier_547_560" id="FieldModifier_967_980" title="Referenced at line 30">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3#Private_179_186" id="Private_983_990" title="Defined at ../../lexical/Modifiers.sdf3 line 12, 27">Private</a>
  <a href="#FieldModifier_547_560" id="FieldModifier_993_1006" title="Referenced at line 30">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3#Static_210_216" id="Static_1009_1015" title="Defined at ../../lexical/Modifiers.sdf3 line 15, 30">Static</a>
  <a href="#FieldModifier_547_560" id="FieldModifier_1018_1031" title="Referenced at line 30">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3#Final_162_167" id="Final_1034_1039" title="Defined at ../../lexical/Modifiers.sdf3 line 10, 25">Final</a>
  <a href="#FieldModifier_547_560" id="FieldModifier_1042_1055" title="Referenced at line 30">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3#Transient_245_254" id="Transient_1058_1067" title="Defined at ../../lexical/Modifiers.sdf3 line 18, 32">Transient</a>
  <a href="#FieldModifier_547_560" id="FieldModifier_1070_1083" title="Referenced at line 30">FieldModifier</a> = <a href="../../lexical/Modifiers.sdf3#Volatile_257_265" id="Volatile_1086_1094" title="Defined at ../../lexical/Modifiers.sdf3 line 19, 33">Volatile</a>
  
<span class="keyword">context-free syntax</span>  
  
  <a href="#UnannType_569_578" id="UnannType_1125_1134" title="Referenced at line 30; ../MethodDeclarations.sdf3 line 71; ../../interfaces/AnnotationTypes.sdf3 line 38; ../../interfaces/ConstantDeclarations.sdf3 line 18; ../../statements/LocalVariableDeclarations.sdf3 line 19; ../../statements/Statements.sdf3 line 128">UnannType</a> = <a href="#UnannPrimitiveType_415_433" id="UnannPrimitiveType_1137_1155" title="Defined at line 23, 53, 54">UnannPrimitiveType</a>
  <a href="#UnannType_569_578" id="UnannType_1158_1167" title="Referenced at line 30; ../MethodDeclarations.sdf3 line 71; ../../interfaces/AnnotationTypes.sdf3 line 38; ../../interfaces/ConstantDeclarations.sdf3 line 18; ../../statements/LocalVariableDeclarations.sdf3 line 19; ../../statements/Statements.sdf3 line 128">UnannType</a> = <a href="#UnannReferenceType_436_454" id="UnannReferenceType_1170_1188" title="Defined at line 24, 56, 57">UnannReferenceType</a>
  
  <a href="#UnannPrimitiveType_1695_1713" id="UnannPrimitiveType_1194_1212" title="Referenced at line 65">UnannPrimitiveType</a>.<span class="cons_Constructor"><span id="NumericType_1213_1224" title="Not referenced locally, nor via imports">NumericType</span></span> = <a href="../../types/PrimitiveTypes.sdf3#NumericType_147_158" id="NumericType_1227_1238" title="Defined at ../../types/PrimitiveTypes.sdf3 line 11, 17, 18, 19, 20, 21, 22, 23">NumericType</a>
  <a href="#UnannPrimitiveType_1695_1713" id="UnannPrimitiveType_1241_1259" title="Referenced at line 65">UnannPrimitiveType</a>.<span class="cons_Constructor"><span id="BooleanType_1260_1271" title="Not referenced locally, nor via imports">BooleanType</span></span> = <span class="cons_Lit">"boolean"</span>
  
  <a href="#UnannReferenceType_1170_1188" id="UnannReferenceType_1289_1307" title="Referenced at line 51">UnannReferenceType</a> = <a href="#UnannClassType_457_471" id="UnannClassType_1310_1324" title="Defined at line 25, 59, 60">UnannClassType</a>
  <a href="#UnannReferenceType_1170_1188" id="UnannReferenceType_1327_1345" title="Referenced at line 51">UnannReferenceType</a> = <a href="#UnannArrayType_474_488" id="UnannArrayType_1348_1362" title="Defined at line 26, 65, 66">UnannArrayType</a>
  
  <a href="#UnannClassType_1780_1794" id="UnannClassType_1368_1382" title="Referenced at line 66; ../../statements/Statements.sdf3 line 107">UnannClassType</a>.<span class="cons_Constructor"><span id="ClassType_1383_1392" title="Not referenced locally, nor via imports">ClassType</span></span>                       = &lt;&lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_1419_1421" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&lt;<a href="../../types/ParameterizedTypes.sdf3#TypeArguments_157_170" id="TypeArguments_1423_1436" title="Defined at ../../types/ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>?&gt;&gt;
  <a href="#UnannClassType_1780_1794" id="UnannClassType_1442_1456" title="Referenced at line 66; ../../statements/Statements.sdf3 line 107">UnannClassType</a>.<span class="cons_Constructor"><span id="UnannClassOrInterfaceTypeMember_1457_1488" title="Not referenced locally, nor via imports">UnannClassOrInterfaceTypeMember</span></span> = &lt;&lt;<a href="#UnannClassType_457_471" id="UnannClassType_1493_1507" title="Defined at line 25, 59, 60">UnannClassType</a>&gt;<span class="cons_String">.</span>&lt;{<a href="../../interfaces/Annotations.sdf3#Annotation_158_168" id="Annotation_1511_1521" title="Defined at ../../interfaces/Annotations.sdf3 line 12, 19, 20, 21">Annotation</a> <span class="cons_Lit">" "</span>}*&gt; &lt;<a href="../../lexical/Identifiers.sdf3#Id_141_143" id="Id_1530_1532" title="Defined at ../../lexical/Identifiers.sdf3 line 15, 23">Id</a>&gt;&lt;<a href="../../types/ParameterizedTypes.sdf3#TypeArguments_157_170" id="TypeArguments_1534_1547" title="Defined at ../../types/ParameterizedTypes.sdf3 line 11, 17">TypeArguments</a>?&gt;&gt;
  
<span class="layout">//  ambiguous with UnannClassType.ClassType</span>
<span class="layout">//  UnannTypeVariable.TypeVar            = Id</span>
  
  <a href="#UnannArrayType_1348_1362" id="UnannArrayType_1649_1663" title="Referenced at line 57">UnannArrayType</a>.<span class="cons_Constructor"><span id="UnannArrayTypePrimitive_1664_1687" title="Not referenced locally, nor via imports">UnannArrayTypePrimitive</span></span>    = &lt;&lt;<a href="#UnannPrimitiveType_415_433" id="UnannPrimitiveType_1695_1713" title="Defined at line 23, 53, 54">UnannPrimitiveType</a>&gt; &lt;<a href="../../types/ReferenceTypes.sdf3#AnnotatedDim_310_322" id="AnnotatedDim_1716_1728" title="Defined at ../../types/ReferenceTypes.sdf3 line 19, 41">AnnotatedDim</a>+&gt;&gt;
  <a href="#UnannArrayType_1348_1362" id="UnannArrayType_1734_1748" title="Referenced at line 57">UnannArrayType</a>.<span class="cons_Constructor"><span id="UnannArrayTypeClassType_1749_1772" title="Not referenced locally, nor via imports">UnannArrayTypeClassType</span></span>    = &lt;&lt;<a href="#UnannClassType_457_471" id="UnannClassType_1780_1794" title="Defined at line 25, 59, 60">UnannClassType</a>&gt; &lt;<a href="../../types/ReferenceTypes.sdf3#AnnotatedDim_310_322" id="AnnotatedDim_1797_1809" title="Defined at ../../types/ReferenceTypes.sdf3 line 19, 41">AnnotatedDim</a>+&gt;&gt;
  
  
</code></pre></td></tr></tbody></table></div>